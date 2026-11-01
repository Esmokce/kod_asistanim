# kod_asistanim
**Proje Yazarı:** Esma Ökçe

# Projenin Adı: Kod-Asistan v0.1

## Projenin Amacı
Kullanıcılara günlük işlerinde (hesaplama, selamlama vb.) yardımcı olacak bir dijital asistan tasarlamak.

## Projenin Hedefleri
- v0.1: Temel selamlama ve dört işlem hesaplama
- v1.0: Akıllı Menü (kullanıcı seçimine göre yönlendirme)
- v2.0: Veri Saklama (kullanıcı adı ve geçmiş işlemlerin kaydı)

## Projenin Kapsamı
Asistan, kullanıcıdan aldığı girdiyi kontrol eder. Kritik eşik mantığı:

BAŞLA
  HATA_SAYISI ← 0
  EŞİK ← 3
  TEKRARLA
    Kullanıcıdan işlem seçimini al
    EĞER seçim geçerli DEĞİLSE
      HATA_SAYISI ← HATA_SAYISI + 1
      "Geçersiz seçim, tekrar deneyin" yaz
    DEĞİLSE
      Seçilen işlemi yap
      HATA_SAYISI ← 0
  HATA_SAYISI >= EŞİK olana kadar
  "Çok fazla hatalı giriş, asistan kapatılıyor" yaz
BİTİR

## Kaynakça
- Milli Eğitim Bakanlığı. *Algoritmik Düşünme ve Tasarım* [Ders Kitabı]. (Yayınevi, yıl)