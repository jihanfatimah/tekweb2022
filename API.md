**API POINT USER**
**Jihan**


**Users**
GET: /users/[id]

response:
[
{
  "id"          : "",
  "title"        : "",
  "des"  : "",

},
...
]

GET: /users

response:
[
{
 "id"          : "",
  "title"        : "",
  "des"  : "",
},
...
]

POST: /users
data:
{
  "id"          : "",
  "title"        : "",
  "des"  : "",
}

response:
true    // if success
false   // if failure


PUT: /users/[id]
data:
{ 
   "id"          : "",
  "title"        : "",
  "des"  : "",
}

response:
true    // if success
false   // if failure



DELETE: /users/[id]
response:
true    // if success
false   // if failure

*Artikel*
GET: /Artikel/[id]
[
{
  "id"          : "",
  "title"        : "",
  "des"  : "",

},
...
]


GET: /Artikel
[
{
  "id"          : "",
  "title"        : "",
  "des"  : "",

},
...
]


POST: /Artikel 
data: 
[
{
  "id"          : "",
  "title"        : "",
  "des"  : "",

},
...
]



PUT: /Artikel/[id] 
data: 
[
{
  "id"          : "",
  "title"        : "",
  "des"  : "",

},
...
]
response: 
true // if success 
false // if failure

DELETE: /Artikel/[id] 
response: 
true // if success 
false // if failure

Desain database dari API Point yang telah saya buat adalah sebagai berikut:


classDiagram
    class Users{
        # id: int
        + title: varchar
        + des: varchar
        + getAllUsers()
        + getUsersById()
        + updateUsers()
        + createUsers()
        + deleteUsers()
    },
    class Artikel{
        # id: int
        + title: varchar
        + des: tex
        + gambar: varchar
        + getAllArtikel()
        + getArtikelById()
        + updateArtikel()
        + createArtikel()
        + deleteArtikel()
    }
