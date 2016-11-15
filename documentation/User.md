# User API

## `GET /users`

**Authentication:**

- Authorization: Token token={your token}

**Response:**

- Status Code: 200

Sample Response:

```json
[{
	"first_name": "Bob",
	"last_name": "Jones",
	"username": "bjones",
	"email": "bjones@gmail.com"
}]
```

## `POST /users`

**Authentication:**

- Authorization: Token token={your token}

**Body Parameters:**

- first_name: *String*
- last_name: *String*
- username: *String*
- email: *String*

**Response:**

- Status Code: 201

Sample Response:

```json
{
	"first_name": "Bob",
	"last_name": "Jones",
	"username": "bjones",
	"email": "bjones@gmail.com"
}
```

## `GET /users/:id`

**Authentication:**

- Authorization: Token token={your token}

**Response:**

- Status Code: 200

Sample Response:

```json
{
	"first_name": "Bob",
	"last_name": "Jones",
	"username": "bjones",
	"email": "bjones@gmail.com"
}
```

## `PUT /users/:id`

**Authentication:**

- Authorization: Token token={your token}

**Body Parameters:**

- first_name: *String*
- last_name: *String*
- username: *String*
- email: *String*

**Response:**

- Status Code: 204

## `DELETE /users/:id`

**Authentication:**

- Authorization: Token token={your token}

**Response:**

- Status Code: 200