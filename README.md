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
   "ADMIN": "your_admin_user_id"
}
```
```
WEBHOOK = Your channel webhook to send message logs on
USERNAME_PASS = Your account details on hanime.tv
TIMEOUT = Leave it as is
ADMIN = Your user id on discord, used for pinging you when an error occurs on the program. You can leave it empty as well.
```

Run:
```
chmod +x coincollectorV1.X
./coincollectorV1.x
```
