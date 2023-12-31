# CoinCollector-Release
CoinCollector for Hanime.tv. 

Create config.json
```json
{
    "WEBHOOK": [
      "https://discord.com/api/webhooks/*/*"
    ],
    "USERNAME_PASS": [
      {"username": "usernameHere", "password": "passwordHere"},
      {"username": "Account2", "password": "passwordHere"}
    ],
   "TIMEOUT": {
        "ERROR": 3600,
        "COIN": 10800
    },
   "ADMIN": "your user discord id for pinging during error or can leave empty"
}
```

Run:
```
chmod +x coincollectorV1.X
./coincollectorV1.x
```
