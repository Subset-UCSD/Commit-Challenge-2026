user adds a new game to track
```
POST /tracknew
request
{
    "game_name": "string"
}
response
{
    "status": "string"
}
```

user submit game results
```
POST /submit
request
{
    "user_id": "string",
    "game_name": "string",
    "game_results": "string"
}
response
{
    "status": "string"
}
```

user views stats page
```
GET /stats
response
[  
    {
        "user_id": "string",
        "game_name": "string",
        "game_results": "string",
        "date": "string" (?)
    }
]
```

user views stats page for specific game
```
GET /stats/<game_name>
response
[  
    {
        "user_id": "string",
        "game_results": "string",
        "date": "string" (?)
    }
]
```