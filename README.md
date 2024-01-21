# Lokasyon Entity

Bu proje, uçak bilet rezervasyon sistemi için temel bir LokasyonEntity sınıfını içerir.

## LokasyonEntity Özellikleri

- **Id:** Lokasyonun benzersiz kimliğini temsil eden bir tamsayı.
- **Ulke:** Lokasyonun bulunduğu ülkeyi ifade eden bir metin.
- **Sehir:** Lokasyonun bulunduğu şehri ifade eden bir metin.
- **Havaalani:** Lokasyonun havaalanını ifade eden bir metin.
- **AktifMi:** Lokasyonun aktif olup olmadığını belirten bir boolean değeri.

## Kullanım

LokasyonEntity sınıfını kullanarak yeni bir lokasyon eklemek için aşağıdaki örneği inceleyebilirsiniz:

```csharp
LocationEntity newLocation = new LocationEntity
{
    Ulke = "Turkey",
    Sehir = "Istanbul",
    Havaalani = "Ataturk Airport",
    AktifMi = true
};

// Lokasyon ekleme işlemi
locationService.AddLocation(newLocation);
