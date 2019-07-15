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

## EnumWebService
```
Success = 1
Failed = 2
Exception = 3
Warning = 4
NoAction = 5
NoData = 6
```

## API Version 1.0
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
