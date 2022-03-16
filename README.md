**Registration**

POST https://kata.academy:8021/api/users
content-type: application/json

`{
    "user": {
    "username": "nk",
    "email": "meowmeowmoore@gmail.com",
    "password": "goodbye111"
    } 
}`

Response

`{
    "user": {
    "username": "nk",
    "email": "meowmeowmoore@gmail.com",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzBhY2Y5ZmQyMTFjMjEwMGRiMmFmOSIsInVzZXJuYW1lIjoibmsiLCJleHAiOjE2NTI1OTkyMTQsImlhdCI6MTY0NzQxNTIxNH0.Bm-lwL-PBq9TVjo9XrTwhf_fmLJXarNYWH5GwDBcUZk"
    }
}`


**Authentication**

POST https://kata.academy:8021/api/users/login
content-type: application/json

`{
    "user": {
    "email": "meowmeowmoore@gmail.com",
    "password": "goodbye111"
    }
}`

Response

`{
    "user": {
    "username": "nk",
    "email": "meowmeowmoore@gmail.com",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzBhY2Y5ZmQyMTFjMjEwMGRiMmFmOSIsInVzZXJuYW1lIjoibmsiLCJleHAiOjE2NTI1OTkzNzEsImlhdCI6MTY0NzQxNTM3MX0.HpcwiKTjhv1ZjWw2FIkXrDlQAtUM4M1NbwsmAMbpeR0"
    }
}
`

**Get Current User**

GET https://kata.academy:8021/api/user
content-type: application/json
Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzBhY2Y5ZmQyMTFjMjEwMGRiMmFmOSIsInVzZXJuYW1lIjoibmsiLCJleHAiOjE2NTI1OTkzNzEsImlhdCI6MTY0NzQxNTM3MX0.HpcwiKTjhv1ZjWw2FIkXrDlQAtUM4M1NbwsmAMbpeR0

Response 

`{
    "user": {
    "username": "nk",
    "email": "meowmeowmoore@gmail.com",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyMzBhY2Y5ZmQyMTFjMjEwMGRiMmFmOSIsInVzZXJuYW1lIjoibmsiLCJleHAiOjE2NTI1OTk1MjgsImlhdCI6MTY0NzQxNTUyOH0.Elm8Ytw4ewNXX5H0LhyqXeIpA79xPA8ZRDfhzZuE8Gw"
    }
}`