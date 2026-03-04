# Basic Bootcamp Projesi 

ASP.NET Core MVC ile geliştirilmiş, öğrenci ve bootcamp yönetim sistemi. Identity kütüphanesi ile kullanıcı kayıt ve giriş işlemleri yapılabilmektedir.

## Özellikler

- ✅ Öğrenci CRUD işlemleri (resim yükleme dahil)
- ✅ Bootcamp CRUD işlemleri (resim yükleme dahil)
- ✅ Öğrenci - Bootcamp kayıt işlemleri
- ✅ Kimlik doğrulama (Register/Login/Logout)
- ✅ Rol tabanlı yetkilendirme (Identity)
- ✅ SQLite veritabanı
- ✅ Entity Framework Core (Code First)
- ✅ Bootstrap 5 ile responsive tasarım

## Kullanılan Teknolojiler

- **.NET 9.0**
- **ASP.NET Core MVC 9.0**
- **Entity Framework Core 9.0**
- **Microsoft SQLite**
- **Microsoft Identity**
- **Bootstrap 5**
- **HTML5/CSS3**

## Gerekli Paketler - Terminale yazınız.

- **dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore --version 9.0.1**
- **dotnet add package Microsoft.EntityFrameworkCore --version 9.0.1**
- **dotnet add package Microsoft.EntityFrameworkCore.Sqlite --version 9.0.1**
- **dotnet add package Microsoft.EntityFrameworkCore.Tools --version 9.0.1**
- **dotnet add package Microsoft.EntityFrameworkCore.Design --version 9.0.1**

## Proje Yapısı

Basic/
├── Controllers/          # MVC Controller'lar
│   ├── AccountController.cs
│   ├── OgrenciController.cs
│   ├── BootcampController.cs
│   └── BootcampKayitController.cs
├── Data/                 # Veritabanı katmanı
│   ├── DataContext.cs
│   ├── Bootcamp.cs
│   ├── Ogrenci.cs
│   └── BootcampKayit.cs
├── Models/               # ViewModeller
│   ├── ApplicationUser.cs
│   ├── RegisterVm.cs
│   └── LoginVm.cs
├── Views/                # View dosyaları
│   ├── Account/
│   ├── Ogrenci/
│   ├── Bootcamp/
│   └── BootcampKayit/
├── wwwroot/              # Statik dosyalar
│   └── img/              # Yüklenen resimler
├── appsettings.json      # Uygulama ayarları
└── Program.cs            # Uygulama giriş noktası

## Kullanım
Öğrenci İşlemleri
/Ogrenci - Tüm öğrencileri listeler
/Ogrenci/Create - Yeni öğrenci ekler
/Ogrenci/Edit/{id} - Öğrenci düzenler
/Ogrenci/Profile/{id} - Öğrenci detayı

Bootcamp İşlemleri
/Bootcamp - Tüm bootcamp'leri listeler
/Bootcamp/Create - Yeni bootcamp ekler
/Bootcamp/Edit/{id} - Bootcamp düzenler
/Bootcamp/Profile/{id} - Bootcamp detayı

Kayıt İşlemleri
/BootcampKayit - Tüm kayıtları listeler
/BootcampKayit/Create - Öğrenciyi bootcamp'e kaydeder

Hesap İşlemleri
/Account/Register - Yeni hesap oluşturur
/Account/Login - Hesaba giriş yapar
/Account/Logout - Çıkış yapar

Varsayılan Kullanıcı Bilgileri
İlk kullanıcıyı kendiniz oluşturmalısınız.