# TO-DO

## Implement a single pipeline, going straight through.

I'm going to do one GET pipe, one POST pipe, and one PUT pipe.

GET: query-book
POST: loan-book / return-book (basically identical)
PUT: add-user

I need to define a basic schema to iterate on.

In SQL, we have Book, User, Borrowed.
In ES, we have simply Book.

SQL Book
Columns: ISBN, num-borrowed, num-available

ES Book {
  -id: ISBN
  obj: {
    author,
    title,
    pub-year
  }
}

SQL User
Columns: uid, fname, lname, date-joined

SQL Borrow
Columns: uid, ISBN, date-borrowed, date-due

