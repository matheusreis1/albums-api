# Albums API

API to create and retrieve albums.

### Running

1. First, you need to install dependencies
```
go get .
```
2. To initialize, you hust have to run
```
go run .
```

### Requests

1. Get albums
```curl
curl http://localhost:8080/albums
```

2. Get album by ID
```curl
curl http://localhost:8080/albums/2
```

3. Create new album
```curl
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```
