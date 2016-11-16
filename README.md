#Chirp API
##`GET /tweets`
**Response:**

- Status Code: 200

Sample Response:

```json
[
	{
		"id":1,
		"content":"This is a tweet blah blah",
		"bird_id":3,
		"created_at":"2016-11-16T22:36:04.427Z",
		"updated_at":"2016-11-16T22:36:04.427Z"
	},
	{
		"id":2,
		"content":"This is a tweet blah blah",
		"bird_id":2,
		"created_at":"2016-11-16T22:36:04.431Z",
		"updated_at":"2016-11-16T22:36:04.431Z"
	},
	{
		"id":3,
		"content":"This is a tweet blah blah",
		"bird_id":1,
		"created_at":"2016-11-16T22:36:04.434Z",
		"updated_at":"2016-11-16T22:36:04.434Z"
	}]
```

##`POST /tweets`
**Body Parameters:**

- content: *Text*
- bird_id: *Integer*

**Response:**

- Status Code: 201

Sample Response:

```json
{
	"id":2,
	"content":"This is a tweet blah blah",
	"bird_id":2,
	"created_at":"2016-11-16T22:36:04.431Z",
	"updated_at":"2016-11-16T22:36:04.431Z"
}
```

##`PUT /tweets/:id`
**Body Parameters:**

- content: *Text*
- bird_id: *Integer*


**Response:**

- Status Code: 200

Sample Response:
```json
{
	"id":2,
	"content":"This is a tweet blah blah",
	"bird_id":2,
	"created_at":"2016-11-16T22:36:04.431Z",
	"updated_at":"2016-11-16T22:36:04.431Z"
}
```

##`DELETE /tweets/:id`
**Response:**

- Status Code: 200


##`GET /birds`
**Response:**

- Status Code: 200

Sample Response:

```json
[
	{
		"id"1,
		"email":"fake@gmail.com",
		"name":"Karen",
		"created_at":"2016-11-16T22:36:03.936Z",
		"updated_at":"2016-11-16T22:36:03.936Z",
		"auth_token":null
	},
	{
		"id"2,
		"email":"fake1@gmail.com",
		"name":"Sam",
		"created_at":"2016-11-16T22:36:04.096Z",
		"updated_at":"2016-11-16T22:36:04.096Z",
		"auth_token":null
	}
]
	
```

##`GET /birds/:id/tweets`
**Response:**

- Status Code: 200

Sample Response:

```json
[
	{
		"id":1,
		"content":"This is a tweet blah blah",
		"bird_id":3,
		"created_at":"2016-11-16T22:36:04.427Z",
		"updated_at":"2016-11-16T22:36:04.427Z"
	},
	{
		"id":2,
		"content":"This is a tweet blah blah",
		"bird_id":2,
		"created_at":"2016-11-16T22:36:04.431Z",
		"updated_at":"2016-11-16T22:36:04.431Z"
	}	
]
	
```


##`POST /birds/:id/tweets`
**Body Parameters:**

- content: *Text*

**Response:**

- Status Code: 201

Sample Response:

```json
{
		"id":1,
		"content":"This is a tweet blah blah",
		"bird_id":3,
		"created_at":"2016-11-16T22:36:04.427Z",
		"updated_at":"2016-11-16T22:36:04.427Z"
}
```

##`PUT birds/:bird_id/tweets/:tweet_id`
**Body Parameters:**

- content: *Text*


**Response:**

- Status Code: 200

Sample Response:
```json
{
	"id":2,
	"content":"This is a tweet blah blah",
	"bird_id":2,
	"created_at":"2016-11-16T22:36:04.431Z",
	"updated_at":"2016-11-16T22:36:04.431Z"
}
```

##`DELETE birds/bird_id/tweets/:tweet_id`
**Response:**

- Status Code: 200
