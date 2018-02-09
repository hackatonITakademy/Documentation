# Documentation API

## Donations

Create donation with access_token : 
```javascript
// Return 201 | 422 | 403
// POST : api/donation
{
	"currency_id": 1,
	"amount": 100
}

// Return 422 errors example
{
    "amount": [
        "The amount must be a number."
    ],
    "currency_id": [
        "The currency id field is required."
    ]
}
```

Get donations for a user with access_token : 
`GET : api/donation/user`

## Reports

Get All report : 
`GET : api/report`

Create or Update report :
```javascript
// Return 201 | 422
// POST : api/report
{
	"git_repository": "test2", // Unique
	"email": "email"
}

// Return 422 errors example
{
    "git_repository": [
        "The git repository may not be greater than 191 characters."
    ],
}
```

get a html report :
```js
// return the html if the queue is done and the git exist in database
{
    "git_repository": "test2", // Unique
}
```

Get reports for a user with access_token :
`GET : api/report/user`

## Users

Create user :
```javascript
// Return 201 with access_token | 422 with access_token
// POST : api/register
{
	"name": "test",
	"email": "test@test.com",
	"password": "test",
	"password_confirmation": "test",
}

// Return 422 errors example :
{
    "name": [
        "The name may not be greater than 191 characters."
    ],
    "email": [
        "The email must be a valid email address."
    ],
    "password": [
        "The password confirmation does not match."
    ]
}
```

Login user : 
```javascript
// Return 200 with access_token
{
	"email": "email",
	"password": "mdp"
}
```
## Currencies

Get currencies 
`GET : api/currency`
