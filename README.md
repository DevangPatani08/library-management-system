# library-management-system

    This is a library management api backend for the management of users and books.

# Routes and the endpoints

## /users

GET: This is used to get all the list of users in the system.
POST: Create/Register a new user.

## /users/{id}

GET: This is used to get a user in the system by their id.
PUT: Updating the user by their id.
DELETE: Deleting a user by their id ({check if the user still has an issued book} && {is there a fine to be collected}).

## users/subscription-details/{id}

GET: Get a users subscription details by their id.

    >> Date of subscription
    >> valid till?
    >> Fine if any?

## /books
GET: This is used to get all the list of books in the system.
POST: add a new book to the system.

## /books/{id}
GET: This is used to get a book in the system by it's id.
PUT: Updating the book by it's id.
DELETE: Deleting a book by it's id.

## /books/issued
GET: This is used to get all issued books.

## /books/issued/withFine
GET: This is used to get all issued books with a fine amount to them.

### Subscription Types
    >> Basic (3 months)
    >> Standard (6 months)
    >> Premium (12 months)
    >> if a user misses the book renewal date, then user should be charged with fine Rs.100/-.
    >> if a user misses the subscription renewal date, then user should be charged with fine Rs.100/-.
    >> if a user misses both, then user should be charged with fine Rs.300/-.

# Commands 

    npm init
    npm i express
    npm i nodemon --save-dev
    
    npm run dev

