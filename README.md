Arcanus Otel – Karar Destek Sistemi (KDS)
Proje Açıklaması
Bu proje, Arcanus Otel işletmesi için geliştirilmiş web tabanlı bir Karar Destek Sistemidir (KDS).
Sistem, otelcilik sektöründe karar alma süreçlerini desteklemek amacıyla; doluluk oranlarını, misafir analizlerini, hizmet kullanım istatistiklerini ve gelir eğilimlerini görselleştirerek yöneticilere anlık ve geçmiş dönem karşılaştırmalı raporlar sunar.
Senaryo Tanımı
Arcanus Otel yönetimi, farklı dönemlerdeki doluluk oranlarını, misafir tercihlerini ve hizmet kullanım sıklıklarını manuel olarak takip etmekte zorlanmaktadır.
Bu sistem sayesinde yöneticiler;
•  Aylık ve mevsimsel doluluk oranlarını,
•  Misafir yaş ve ırk bazlı dağılımlarını,
•  En çok kullanılan hizmetleri,
•  Sezonsal gelir eğilimlerini
tek bir panelden analiz edebilmektedir.
Sistem Özellikleri
•  12 aylık doluluk oranı çizgi grafiği
•  Oda tipi bazlı doluluk analizi (Standart, Aile Odası, Süit)
•  Misafir ırk ve yaş dağılımı (örn: Rus, Türk, Alman, İngiliz)
•  Hizmet kullanım sıklığı (Restoran, Havuz, Spa, Oda Servisi)
•  Mevsimsel doluluk oranları (Yaz, Kış, İlkbahar, Sonbahar)
•  Yönetici girişi ile güvenli erişim
Kullanılan Teknolojiler
Frontend
•  HTML / CSS / JavaScript
•  Chart.js (grafikler)
Backend
•  Node.js
•  Express.js
Veritabanı
•  MySQL
Veritabanı Yapısı (arcanus.sql)
•  aylar: 12 ayın sıralama ve isim bilgisi
•  doluluk: Aylık doluluk oranları
•  hizmetler: Aylara göre hizmet kullanım sayıları
•  misafir_analizi: Irk ve aya göre misafir sayıları
•  irklar: Misafir ırk türleri
•  oda_tipi_doluluk: Oda türlerine göre doluluk oranları
•  sezonsal_doluluk: Mevsimlere göre doluluk oranları
•  yas: Aylara göre çocuk ve yetişkin misafir sayıları
•  kullanicilar: Yönetici giriş bilgileri
API Endpoint Listesi
•  GET /api/doluluk → Aylık doluluk oranları
•  GET /api/hizmetler → Hizmet kullanım istatistikleri
•  GET /api/misafirler → Irk ve yaş dağılımı
•  GET /api/mevsim → Sezonsal doluluk oranları
•  POST /api/login → Yönetici girişi
Kurulum Adımları
1.  Projeyi Klonla
git clone https://github.com/arauf4815-gif/kds-rauf
2.  MySQL Veritabanı Kurulumu
mysql -u root -p
CREATE DATABASE arcanus;
USE arcanus;
SOURCE arcanus.sql;
3.  Backend Bağımlılıklarını Yükle
npm install
4.  Uygulamayı Başlat
node app.js
5.  Tarayıcıda Aç
http://localhost:3000/login.html
----
Ekranlar
•  Giriş Ekranı → login.html
•  Ana Panel → dashboard.html
•  Hizmet Analizi → hizmetanalizi.html
•  Misafir Analizi → misafirler.html
•  Oda Doluluk Analizi → odalar.html
Bu proje, Dokuz Eylül Üniversitesi Sunucu Tabanlı Programlama dersi kapsamında geliştirilmiştir.
