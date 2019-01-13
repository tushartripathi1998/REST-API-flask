This service will run of port:5000, defaultport for Flask application.

## Ways of making REST requests:
The request is made using 'curl', a command line too for transferring of data, and performing REST operations.

### `GET` :
curl -i http://localhost:5000/todo/api/v1.0/tasks
curl -i http://localhost:5000/todo/api/v1.0/tasks/2

### `POST`:
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book", "description":"whatever"}' http://localhost:5000/todo/api/v1.0/tasks

### `PUT`:
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2

### `DELETE`:
curl -i -H "Content-Type: application/json" -X DELETE-d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2
