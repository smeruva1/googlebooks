# googlebooks

Created a React based Google Books search app. 


I have used google books api to search books by title and save books to my list, the data is stored in Mongo. 


The application is deployed in Heroku. Also used Node, Express for backend api development. 


The Application has two pages:
1. Search Page
2. Saved Books page


1. Search Page: One can search for books via Google Books API and book information is rendered in cards, 4 in each row. The card also has a button which shows the latest state of book - if it is saved in user list or not. The data is saved in Mongo

2. Saved Page: Displays books stored in users list reading from Mongo DB. The cards have a delete button, in case user is no longer interested to read the book.


The application uses Mongoose to create the Book schema and manage read and write.

Book schema has Title, Authors which is an array, description, image url, links.

The application is a Single Page Application (SPA) even though users will see two pages - that is because of use of react-router-dom to naviage.

The application supports below express routes:
1. /api/books - get - all saved books as JSON
2. /api/books - post - to save a new book into Mongo
3. /api/books/:id - delete - to delete a saved book from users list.
 


