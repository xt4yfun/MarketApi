# Proje Adı: Stok Yönetim Sistemi

## Proje Açıklaması

Bu proje, **.NET 8** ve **Entity Framework** kullanılarak geliştirilmiş bir Stok Yönetim Sistemi API'sidir. Bu API, çeşitli bölgeler, şehirlere bağlı marketler ve depolar içeren bir yapıya sahiptir. Proje, ürün ve kategorilerle birlikte ürünlerin stoklarının yönetimini sağlar. Ayrıca minimum stok seviyeleri dikkate alınarak otomatik stok talep etme ve bu taleplerin üst depo tarafından karşılanması fonksiyonlarını da içermektedir.

## Özellikler

- **Bölgeler ve Şehirler**: API, farklı bölgeleri ve bu bölgelere bağlı şehirleri yönetir.
- **Marketler ve Depolar**: Şehirlere bağlı marketler ve depolar bulunmaktadır.
- **Ürün ve Kategoriler**: API, çeşitli ürün ve kategorileri yönetir.
- **Stok Yönetimi**: Ürün stokları ayrı bir tabloda tutulur ve minimum stok seviyeleri belirlenir.
- **Otomatik Stok Talebi**: Minimum stok seviyesinin altına düşen ürünler için depolar yeni ürün talep edebilir ve bu talepler üst depo tarafından karşılanabilir.
- **Rol ve Yetkilendirme**: Site üzerinde farklı roller ve bu rollere bağlı yetkilendirme mekanizması bulunmaktadır.

## Kullanılan Teknolojiler

- **.NET 8**: Projenin ana geliştirme ortamıdır.
- **Entity Framework**: Veri kaynağına bağlanmak ve veri işlemlerini gerçekleştirmek için kullanılmıştır.
- **MS SQL**: Veritabanı olarak kullanılmıştır.
- **JWT Authentication**: Kullanıcı doğrulaması ve yetkilendirme için JSON Web Token (JWT) kullanılmıştır.

## Kurulum

Projeyi yerel ortamınıza kurmak için aşağıdaki adımları izleyin:

1. **Proje Deposunu Klonlayın**:
   ```sh
   git clone https://github.com/xt4yfun/MarketApi.git
   cd MarketApi
   ```

2. **Gerekli Paketleri Yükleyin**:
   ```sh
   dotnet restore
   ```

3. **Veritabanı Ayarlarını Yapın**:
   - `appsettings.json` dosyasındaki veritabanı bağlantı ayarlarını güncelleyin.

4. **Veritabanını Güncelleyin**:
   ```sh
   dotnet ef database update
   ```

5. **Uygulamayı Çalıştırın**:
   ```sh
   dotnet run
   ```


## Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.

---
