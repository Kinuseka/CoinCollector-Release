# Old Releases for CoinCollector

These are archived version from when this project was still private. 

**v1.0 [04/22/2023]** 

config.json template
```json
{
    "WEBHOOK": [
      "https://discord.com/api/webhooks/*/*"
    ],
    "USERNAME_PASS": [
      {"username": "usernameHere", "password": "passwordHere"},
      {"username": "Account2", "password": "passwordHere"}
    ]
}
```
> First release

**v1.2 [04/22/2023]**
> * Added names per each process

**v1.3 [04/22/2023]**
> * Handle ratelimiting and retry again

**v1.4 [04/23/2023]**
> * Increased resiliency to login errors
> * [might be buggy fallback to v1.3 if ever it fails the 24 hour test]

**v1.5 [04/23/2023]**

New config
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
        "ERROR": 3600, // Enter how long it restarts in seconds
        "COIN": 10800 //Not implemented as of V1.5
    },
   "ADMIN": "your_admin_user_id"
}
```
> * You can now customize the length of refresh incase an error occurs. Be sure to update config.json if u are upgrading from the older version.
> * Customizable user. Add USER ID only

**v1.6 [05/28/2023]**
> * Added self checking and error mitigation codes
> * Program will no longer close abruptly when an error occurs.
> * ~~Source code~~

**v1.7 [06/23/2023]**
> * fixed error on systems running on container (openVZ)
> * added arg -n to enable this feature

**1.8 [07/02/2023]**
> * Enabled logging you can now view output on stdout
> * Fixed zombified processes
> * Fixed issue where errors would make processes wait for longer 
