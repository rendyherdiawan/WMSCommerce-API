# StokProduk_List
Method StokProduk_List digunakan untuk mendapatkan list stok produk

## Request

### Url
```
/API/WebService.asmx?op=StokProduk_List
```

### HTTP GET
```
GET /API/WebService.asmx/StokProduk_List?Token=string&IDWMSStore=string&IDTempat=string&IDProduk=string
```

### HTTP POST
```
POST /API/WebService.asmx/StokProduk_List
Content-Type: application/x-www-form-urlencoded
Content-Length: length

Token=string&IDWMSStore=string&IDTempat=string&IDProduk=string
```

### PARAMETER
Parameter | Wajib | Keterangan 
--- | --- | --- 
Token | Ya | [Token Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#sandbox)
IDWMSStore | Ya | [IDWMSStore Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#sandbox)
IDTempat | Tidak | ID untuk pencarian berdasarkan IDTempat
IDProduk | Tidak | ID untuk pencarian berdasarkan IDProduk
