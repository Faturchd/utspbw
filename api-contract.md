# __API Perusahaan Kecil__

## owner

<details>
<summary> Click to extend </summary>

### Create owner
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/owner </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "Fatur",
    "alamat" : "Bogor",

}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data owner Berhasil diinput",
    "data" : {
        "id" : 1,
        "nama" : "Fatur",
        "alamat" : "Bogor"

    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama owner Telah digunakan",
    "data" : {
        "value" : "Fatur",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read owner By Id
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/owner </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/owner?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
        "id" : 1,
        "nama" : "Fatur",
        "alamat" : "Bogor",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID owner tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read owner All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/owner </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "id" : 1,
            "nama" : "Fatur",
            "alamat" : "Bogor",
          
        }
    ]
}    
```

</td>
</tr>
</table>

### Update owner
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/owner </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "id" : 1,
    "nama" : "Faturachman",
    "alamat" : "Cijeruk",
    
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data owner Berhasil diubah",
    "data" : {
        "id" : 1,
        "nama" : "Faturachman",
        "alamat" : "Cijeruk",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama owner Telah digunakan",
    "data" : {
        "value" : "Faturachman",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID owner tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete owner
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/owner </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/owner?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID owner tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>

## Manajer keuangan
<details>
<summary> click to extend </summary>

### Create Manajer keuangan
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "Agus",
    "alamat" : "Bekasi",
    
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Manajer keuangan Berhasil diinput",
    "data" : {
        "id" : 1,
        "nama" : "Agus",
        "alamat" : "Bekasi",
    
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Manajer keuangan Telah digunakan",
    "data" : {
        "value" : "Agus",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read Manajer keuangan By Id
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
        "id" : 1,
        "nama" : "Agus",
        "alamat" : "Bekasi",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Manajer keuangan tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read Manajer keuangan All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "id" : 1,
            "nama" : "Agus",
            "alamat" : "Bekasi",
            
        },
        {
            "id" : 1,
            "nama" : "Agung",
            "alamat" : "Surabaya",
        }
    ]
}    
```

</td>
</tr>
</table>

### Update Manajer keuangan
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "id" : 1,
    "nama" : "Agus daulay",
    "alamat" : "Cibinong",
    
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data Manajer keuangan Berhasil diubah",
    "data" : {
        "id" : 1,
        "nama" : "Agus daulay",
        "alamat" : "Cibinong",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Manajer keuangan Telah digunakan",
    "data" : {
        "value" : "Agus daulay",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Manajer keuangan tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete Manajer keuangan
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/Manajer_keuangan?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID Manajer keuangan tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>

## Manager Operasional

<details>
<summary> Click to extend </summary>

### Create Manager Operasional
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_op </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "Ruslan",
    "alamat" : "Bandung",

}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data manager op Berhasil diinput",
    "data" : {
        "id" : 1,
        "nama" : "Ruslan",
        "alamat" : "Bandung"

    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama manager op Telah digunakan",
    "data" : {
        "value" : "Ruslan",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read manager operasional By Id
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/manager_op </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/manager_op?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
        "id" : 1,
        "nama" : "Ruslan",
        "alamat" : "Bandung",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager op tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read manager operasional All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/manager_op </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "id" : 1,
            "nama" : "Ruslan",
            "alamat" : "Bandung",
          
        },
        {
            "id" : 2,
            "nama" : "Rizik",
            "alamat" : "Banten",
            
        }
    ]
}    
```

</td>
</tr>
</table>

### Update manager operasional
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/manager_op </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "id" : 1,
    "nama" : "Jihan fachrani",
    "alamat" : "NTB",
    
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data manager op Berhasil diubah",
    "data" : {
        "id" : 1,
        "nama" : "Jihan fachrani",
        "alamat" : "NTB",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama manager op Telah digunakan",
    "data" : {
        "value" : "Jihan fachrani",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager op tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete manager operasional
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/manager_op </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/manager_op?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager op tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>

## Manager pemasaran
<details>
<summary> Click to extend </summary>

### Create Manager pemasaran
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "Tifany",
    "alamat" : "Bandung",

}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data manager pemasaran Berhasil diinput",
    "data" : {
        "id" : 1,
        "nama" : "Tifany",
        "alamat" : "Bandung"

    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama manager pemasaran Telah digunakan",
    "data" : {
        "value" : "Tifany",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>


### Read manager pemasaran By Id
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
        "id" : 1,
        "nama" : "Tifany",
        "alamat" : "Bandung",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager pemasaran tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>


### Read manager pemasaran All
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> GET </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : [
        {
            "id" : 1,
            "nama" : "Tifany",
            "alamat" : "Bandung",
          
        },
        {
            "id" : 2,
            "nama" : "Bastian",
            "alamat" : "Bogor",
            
        }
    ]
}    
```

</td>
</tr>
</table>

### Update manager pemasaran
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> PUT </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "id" : 1,
    "nama" : "Tifany carla",
    "alamat" : "Balik papan",
    
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data manager pemasaran Berhasil diubah",
    "data" : {
        "id" : 1,
        "nama" : "Tifany carla",
        "alamat" : "Balik papan",
        
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama manager pemasaran Telah digunakan",
    "data" : {
        "value" : "Tifany carla",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager pemasaran tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>

### Delete manager pemasaran
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran </td>
</tr>
<tr>
    <td> <b>Example</b> </td>
    <td> {{baseURL}}/api/v1/Manager_pemasaran?id=1 </td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> DELETE </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>
<tr>
<td> <b>Query</b> </td>
<td> id=1 </td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 200,
    "message" : "Sukses dihapus",
    "data" : [] 
}    
```

</td>
</tr>
<tr>
<td> <b>Respon Not Found</b> </td>
<td>

``` json
{
    "code" : 404,
    "message" : "ID manager pemasaran tidak ditemukan",
    "data" : {
        "value" : 1,
        "property" : "id",
        "location" : "query"
    } 
}    
```

</td>
</tr>
</table>
</details>