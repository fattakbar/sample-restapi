# Sample GO Lang RESTful API

> Sample RESTful API to create, read, update and delete books. No database implementation yet

## Quick Start


``` bash
# Install mux router
go get -u github.com/gorilla/mux
```

``` bash
go build
./go_restapi
```

## Endpoints

### Get All Books
``` bash
GET api/books
```
### Get Single Book
``` bash
GET api/books/{id}
```

### Delete Book
``` bash
DELETE api/books/{id}
```

### Create Book
``` bash
POST api/books

# Request sample
# {
#   "isbn":"1984934724",
#   "title":"Learn Go Programming Language From Scratch",
#   "author":{"firstname":"Alban",  "lastname":"Andahi"}
# }
```

### Update Book
``` bash
PUT api/books/{id}

# Request sample
# {
#   "isbn":"1984934724",
#   "title":"Updated Title",
#   "author":{"firstname":"Updated First Name",  "lastname":"Updated Last Name"}
# }

```