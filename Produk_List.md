# Produk_List
Method Produk_List digunakan untuk mendapatkan list produk

## Request

### Url
```
/API/WebService.asmx?op=Produk_List
```

### HTTP GET
```
The following is a sample HTTP GET request and response. The placeholders shown need to be replaced with actual values.

GET /API/WebService.asmx/Produk_List?Token=string&IDWMSStore=string&Nama=string&KodeProduk=string
```

### HTTP POST
```
The following is a sample HTTP POST request and response. The placeholders shown need to be replaced with actual values.

POST /API/WebService.asmx/Produk_List
Content-Type: application/x-www-form-urlencoded
Content-Length: length

Token=string&IDWMSStore=string&Nama=string&KodeProduk=string
```

Parameter | Wajib | Keterangan 
Token | Ya | [Token Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#sandbox)
IDWMSStore | Ya | [IDWMSStore Sandbox](https://github.com/rendyherdiawan/WMSCommerce-API#sandbox)
Nama | Tidak | Keyword untuk pencarian berdasarkan Nama Produk 
KodeProduk | Tidak | Keyword untuk pencarian berdasarkan Kode Produk 
