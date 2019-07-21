# WMSCommerce Public API (Beta)

### List API
```
/API/WebService.asmx
```

## Sandbox

### Token
```
CAD81A2F-8A0E-44E0-91FD-3A0C1D8D7E5A
```

### IDWMSStore
```
96220AC7-7CE3-41F7-A159-2E2E64A3A9BA
```

### IDWMSTempat
```
5E3AEAA1-C632-4D59-9D5D-3F75056C9FF6
```

### IDTempat
```
1
```

## EnumWebService
```
Success = 1
Failed = 2
Exception = 3
Warning = 4
NoAction = 5
NoData = 6
```

## API Version 1.0.0
Function | Description 
--- | --- 
AtributProduk_Data | Menampikan data master atribut produk
JenisPembayaran_Data | Menampilkan data master jenis pembayaran
KombinasiProdukTempat_Data | Menampilkan kombinasi produk berdasarkan tempat
KombinasiProduk_Data | Menampilkan data master kombinasi produk
PemilikProduk_Data | Menampilkan data master pemilik produk
ProdukKategori_Data | Menampilkan data master kategori produk
Produk_Data | Menampilkan data master produk
StokProduk | Menampilkan stok produk
StokProdukTempat_Data | Menampilkan data master stok produk berdasarkan tempat
StokProduk_Data | Menampilkan data master stok produk
Warna_Data | Menampilkan data master warna

## API Version 1.1.0

Function | Description | Documentation
--- | --- | --- 
Produk_List | Menampilkan list produk | [View](https://github.com/rendyherdiawan/WMSCommerce-API/blob/master/Produk_List.md#produk_list)
StokProduk_List | Menampilkan list stok produk | [View](https://github.com/rendyherdiawan/WMSCommerce-API/blob/master/StokProduk_List.md#stokproduk_list)

## Kamus Bahasa
Istilah | Penjelasan
--- | --- 
Store | Store merupakan data client dari WIT. Indonesia
Tempat | Satu Store dapat memiliki banyak Tempat. Contoh : Cabang 1, Cabang 2, Event 1, Gudang, dll
Pemilik Produk | Jika Store menjual barang dari beberapa Brand maka Brand tersebut diisi pada bagian Pemilik Produk
Produk | Produk produk yang dijual oleh Store
Atribut Produk | Produk memiliki Atribut Produk. Contoh : S, M, L, 37 - Hitam, 38 - Hitam
Kombinasi Produk | Kombinasi Produk adalah gabungan dari Produk dan Atribut Produk. Contoh : Sepatu A (37 - Hitam)
Stok Produk | Stok Produk adalah gabungan dari Kombinasi Produk dan Tempat. Contoh : Sepatu A (37 - Hitam) di Gudang Quantity 10

# EXAMPLE

## AtributProduk_Data
```
/API/WebService.asmx?op=AtributProduk_Data
```

Parameter | Value 
--- | --- 
Token | [Token Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#token-sandbox)
IDWMSStore | [IDWMSStore Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#id-wms-store-sandbox)

### HTTP GET
```
GET /API/WebService.asmx/AtributProduk_Data?Token=string&IDWMSStore=string
```

### HTTP POST
```
POST /API/WebService.asmx/AtributProduk_Data
Content-Type: application/x-www-form-urlencoded
Content-Length: length

Token=string&IDWMSStore=string
```

### RESULT SUCCESS
```json
{
  "AtributProduk": [
    {
      "IDAtributProduk": 1000,
      "Nama": ""
    },
    {
      "IDAtributProduk": 1001,
      "Nama": "35"
    },
    {
      "IDAtributProduk": 1089,
      "Nama": "Merah - 40"
    }
  ],
  "Result": {
    "EnumWebService": 1,
    "Count": 0,
    "Pesan": ""
  }
}
```

### RESULT FAILED
```json
{
  "AtributProduk": null,
  "Result": {
    "EnumWebService": 2,
    "Count": 0,
    "Pesan": "Token Invalid"
  }
}
```
