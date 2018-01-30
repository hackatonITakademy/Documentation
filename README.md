# Documentation API

## Token

Get token :
`GET : api/token`

## Donations

Get All donations : 
`GET : api/donation`

Create donation : 
```javascript
// Return 201 | 422 | 403
// POST : api/donation
{
	"user_id":1,
	"currency_id": 1,
	"amount": 100,
	"_token": "token"
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

Get donations for an user : 
`GET : api/donation/user/{user}`

## Reports

Get All report : 
`GET : api/report`

Create or Update report :
```javascript
// Return 201 | 422
// POST : api/report
{
	"user_id": 1, // Non obligatoire.
	"git_repository": "test2", // Unique
	"_token": "token"
}

// Return 422 errors example
{
    "git_repository": [
        "The git repository may not be greater than 191 characters."
    ],
    "user_id": [
        "The user id must be an integer."
    ]
}
```

Get reports for an user :
`GET : api/report/user/{user}`

## Users

Create user :
```javascript
// Return 201 | 422
// POST : api/user
{
	"name": "test",
	"email": "test@test.com",
	"password": "test",
	"password_confirmation": "test",
    	"_token": "token"
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
## Currencies

Get currencies 
`GET : api/currency`
