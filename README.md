# WMSCommerce Public API (Beta)

### List API
```
/API/WebService.asmx
```

### ID WMS Store Sandbox
```
96220ac7-7ce3-41f7-a159-2e2e64a3a9ba
```

### Token Sandbox
```
CAD81A2F-8A0E-44E0-91FD-3A0C1D8D7E5A
```

### EnumWebService
```
Success = 1
Failed = 2
Exception = 3
Warning = 4
NoAction = 5
NoData = 6
```

### API Version 1.0
```
KombinasiProdukTempat_Data
KombinasiProduk_Data
PemilikProduk_Data
ProdukKategori_Data
Produk_Data
StokProduk
StokProdukTempat_Data
StokProduk_Data
Warna_Data
```

# AtributProduk_Data
```
/API/WebService.asmx?op=AtributProduk_Data
```

Parameter | Value 
--- | --- 
Token | IDWMSStore

### HTTP GET
```
GET /API/WebService.asmx/AtributProduk_Data?Token=string&IDWMSStore=string HTTP/1.1
```

### HTTP POST
```
POST /API/WebService.asmx/AtributProduk_Data HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Content-Length: length

Token=string&IDWMSStore=string
```
