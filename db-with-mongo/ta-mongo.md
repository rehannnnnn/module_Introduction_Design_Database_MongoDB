# Soal 1
Data aplikasi Skiljek 
- Full Name
- Email
- Phone Number

Relasi One to One

``` javascript
    {
        "_id": "ObjectId('AAAA')",
        "fullName": "Raihan Zhaky Al-hafizh",
        "email": "hannn9491@gmail.com",
        "phoneNumber": "082288224741"
    }
```

# Soal 2
Relasi Skilshop and Schema

- Full Name
- Phone Number
- Address (Max 2)

Relasi : one to few
 ```javascript
     {
        "_id": "ObjectId('AAAA')",
        "fullName": "Raihan Zhaky Al-hafizh",
        "email": "hannn9491@gmail.com",
        "phoneNumber": "082288224741",
        "address" : [
            {
                "street" : "Jalan Pengibu no 39",
                "city" : "Tanjungpinang"
            },
            {
                "street" : "Jalan Subi no 39",
                "city" : "Batam"
            } 
        ]
    }
 ```


# Soal 3
Relasi Skilshop dan Schema
Relasi One to Many

```javascript
    {
        "_id": "ObjectId('AAAA')",
        "productName": "Kaos Polos",
        "brandName": "SkilShirt",
        "variants": [
            {
            "variantName": "Kaos Polos Hitam",
            "color": "Hitam",
            "quantity": 12,
            "price": "Rp 99.000"
            },
            {
            "variantName": "Kaos Polos Navy",
            "color": "Navy",
            "quantity": 10,
            "price": "Rp 99.000"
            }
        ]
    }
```

# Soal 4
Relasi SkilFlix dan Schema
Relasi : Many to Many

Film Schema

```javascript
    {
        "_id": ObjectId("AAAA1"),
        "filmName": "Venom 2"
    },
    {
        "_id": ObjectId("AAAA2"),
        "filmName": "Spiderman No Way Home"
    }

```

Cinema Schema 

```javascript 
    {
        "_id": "ObjectId('CCC1')",
        "cinemaName": "CGF",
        "location": "Pondok Indah Mall",
        "films": [
            "ObjectId('AAAA1')", 
            "ObjectId('AAAA2')"
        ]
    },
    {
        "_id": "ObjectId('CCC2')",
        "cinemaName": "Cinema31",
        "location": "Mall Kelapa Gading",
        "films": [
            "ObjectId('AAAA1')",
            "ObjectId('AAAA2')"
        ]
    }

```