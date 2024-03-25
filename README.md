# J0123P3-Build

Server >> Storing certain book data >> User Register >> Subscriber

This is a book record management API Server/ Backend for the library system or management of records or manuals or books

Fine System:
User: 18/03/2024 - 18/06/2024
21/06/2024 => 50\*3=150/-

## Subscription Types

3 months (Basic)
6 months (Advance)
12 months (Premium)

If the subscription type is standard && if the subscription date is 18/03/2024
=> then subscription valid till 18/09/2024

within subscription date >> if we miss the renewal >> 50/- day
subscription date is also been missed >> and also missed the renewal >> 100 + 50/- day

> > book1
> > basic
> > 18/03/2024 -> subscription date
> > 19/03/2024 => borrowed a book from library
> > book1 renewal date is on 04/04/2024
> > 06/04/2024 => we need to pay a fine of 50\*2=100/-

> > book1
> > basic
> > 18/03/2024 -> subscription date
> > 19/03/2024 => borrowed a book from library
> > book1 renewal date is on 04/04/2024
> > 06/06/2024 => we need to pay a fine of 100+50

missed by renewal date >> 50/-
missed by subscription date >> 100/-
missed by renewal && subscription date >> 150/-

# Routes and Endpoints

## /users

POST: Create a new user
GET: Get all the users

## /users/{id}

GET: Get user by id
PUT: Updating a user by their ID
DELETE: Delete a user by id (chk if he/she still have an issued book) && (is there any fine to paid)

## /users/subscription-details/{id}

GET: Get user subscription details >> Date of subscription >> Valid till >> Is there any fine

## /books

GET: Get all the books
POST: Create/Add a new book

## /books/{id}

GET: Get a book by id
PUT: Update a book by id

## /books/issued

GET: Get all issued books

## /books/issued/withFine

GET: Get all issued books with their fine

## npm init

## npm i nodemon --save-dev

## npm run dev

...each
"name": "Jane",
"surname": "Doe",
"email": "user@email.com",
"subscriptionType": "Premium",
"subscriptionDate": "03/01/2024"

...data
"data": {
"name": "pradeepa",
"surname": "sundaram"
}

const index = users.indexOf(user);
users.splice(index,1)

var class = {"six", "seven", "eight"};
indexOf()
class.indexOf("seven")
1
