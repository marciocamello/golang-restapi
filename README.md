# GoLang RestApi with Gorilla Mux

## Install GO

* https://golang.org/dl/

## Windows

```bash
go build && ./golang-restapi.exe
```

## Unix

```bash
go build && ./golang-restapi
```

## Books

#### Sample in main.go
```json
[{
    "id": "1",
    "isbn": "448743",
    "title": "Book One",
    "author": {
        "firstname": "Marcio",
        "lastname": "Andre"
    }
}, {
    "id": "2",
    "isbn": "847564",
    "title": "Book Two",
    "author": {
        "firstname": "Rayane",
        "lastname": "Lima"
    }
}]
```
## Get all books

```bash
[GET]http://localhost:8000/api/books
```

## Get single book

```bash
[GET]http://localhost:8000/api/books/{id}
```

## Create book

```bash
[POST]http://localhost:8000/api/books
```

#### POST data

* Content-type: applicatin/json

```json
{
    "isbn": "6456365",
    "title": "Book Three",
    "author": {
        "firstname": "John",
        "lastname": "B"
    }
}
```

## Update book by ID

```bash
[PUT]http://localhost:8000/api/books/{id}
```

#### PUT data

* Content-type: applicatin/json

```json
{
    "id": "3",
    "isbn": "6456365",
    "title": "Book Thre",
    "author": {
        "firstname": "John",
        "lastname": "B"
    }
}
```

### Delete book by ID

```bash
[DELETE]http://localhost:8000/api/books/{id}
```
