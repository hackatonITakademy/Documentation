# Documentation API

Get All donations : 
`GET : api/donation`

create donation : 
```javascript
// POST : api/donation
{
	"user_id":1,
	"currency_id":1,
	"amount":100,
	"_token":"TaMxNlW7WpQKSz3qQAGCBP7Q7ONkCIcgCikO2vJU"
}
```

Get donations for an user : 
`GET : api/donation/user/{user}`
