## Bookstore API 

## Overview 

## **The Bookstore API is a RESTful service built using Go and the Gorilla Mux router. It provides endpoints to manage books, allowing users to create, retrieve, update, and delete book records stored in a MySQL database.** ##

1.Features 

2.Add new books

3.Retrieve all books

4.Get details of a specific book by ID

5.Update book details

6.Delete a book

## Project Structure 


bookstore-api/

├── main.go

├── pkg/

│   ├── config/

│   │   ├── app.go

│   ├── controllers/

│   │   ├── bookController.go
│   ├── models/

│   │   ├── book.go

│   ├── routes/

│   │   ├── bookRoutes.go

│   ├── utils/

│       ├── utils.go

└── go.mod

## Installation & Setup

##  Prerequisites

Go 1.22.2
MySQL
Steps
## Clone the repository:
#  git clone https://github.com/amar/go-bookstore.git
cd go-bookstore
## Install dependencies:
go mod tidy
##  Update database credentials in pkg/config/app.go:

d, err := gorm.Open("mysql", "root:root@tcp(127.0.0.1:3306)/simplerest?charset=utf8&parseTime=True&loc=Local")

## Run the application:

go run main.go

## API Endpoints

## Method

Endpoint

Description

POST
/book/

Create a new book
GET

/book/
Get all books
GET

/book/{id}
Get a book by ID
PUT

/book/{id}

Update a book
DELETE

/book/{id}
Delete a book

## Dependencies

## The project uses the following Go packages:

Gorilla Mux (Router) - github.com/gorilla/mux v1.8.1

GORM (ORM for MySQL) - github.com/jinzhu/gorm v1.9.16

MySQL Driver - github.com/go-sql-driver/mysql v1.5.0

Inflection (Singular/plural conversion) - github.com/jinzhu/inflection v1.0.0

## License

This project is open source api project you can use it and modified it.
