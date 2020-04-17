## Import Book data into your mongoDB database.

Make sure MongoDB is running with the command `mongod` then run `mongo bookAPI < booksJson.js` from the command line.

## Routes
| Route                    | What does it do?                                |
| ------------------------ | ----------------------------------------------- |
| /api/books               | Show All books                                  |
| /api/books?genre=Fantasy | Filter books of a genre, "Fantasy" in this case |