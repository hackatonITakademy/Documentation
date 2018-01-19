# Documentation API

## Donations

Get All donations : 
`GET : api/donation`

Create donation : 
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

## Reports

Get All report : 
`GET : api/report`

Create report :
```javascript
{
	"user_id": 1, // Non obligatoire.
	"git_repository": "test2", // Unique
	"_token":"SD0oDUpAFPSqqNDtQT1CsygkViD62oI3RImJEDDP"
}
```

Get reports for an user :
`GET : api/report/user/{user}
