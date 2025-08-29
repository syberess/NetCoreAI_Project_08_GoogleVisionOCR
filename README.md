# 👁️ NetCoreAI Project 08 - Google Cloud Vision OCR

Bu proje, **.NET Console Application** ile **Google Cloud Vision API** kullanılarak resimlerden metin tanıma (OCR) işlemi yapmaktadır.  
Kullanıcıdan resim dosyası yolu alınır, Google Vision API servisine gönderilir ve dönen metin konsola yazdırılır.  

---

## 🛠️ Kullanılan Teknolojiler
- .NET 8 / 9 Console Application  
- [Google Cloud Vision API](https://cloud.google.com/vision)  
- `Google.Cloud.Vision.V1` NuGet paketi  

---

## 📂 Proje Yapısı
- `Program.cs` → Konsoldan resim yolu alır, Google Vision API’ye gönderir, dönen metni ekrana yazdırır.  
- `.csproj` → Proje bağımlılıkları  

---

## ⚙️ Kurulum ve Çalıştırma
1. Repo’yu klonla:
   git clone https://github.com/kullaniciadiniz/NetCoreAI_Project_08_GoogleVisionOCR.git
   cd NetCoreAI_Project_08_GoogleVisionOCR
Google Cloud servis hesabı oluştur ve JSON credentials dosyasını indir.

Program.cs içinde credentialPath değişkenini ayarla:
string credentialPath = @"C:\Users\monster\google-vision-service.json";
Environment.SetEnvironmentVariable("GOOGLE_APPLICATION_CREDENTIALS", credentialPath);
Uygulamayı çalıştır:
dotnet run
Konsolda resim yolu gir:
Resim yolunu giriniz:
> C:\Users\monster\Desktop\ocr.png

Resimdeki metin:
Hello World from Google Vision OCR!

✨ Özellikler
✔️ Resimden metin tanıma (OCR)

✔️ Google Cloud Vision entegrasyonu

✔️ Birden fazla dil desteği

✔️ Hata yakalama

