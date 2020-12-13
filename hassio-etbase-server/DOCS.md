# Etebase server

## Example config
```yaml
ssl: true
certfile: fullchain.pem
keyfile: privkey.pem
backups: 3
```

| Setting | Type | Description |
| - | - | - |
| ssl | bool | Set true in order to enable SSL, *Highly recommended* |
| certfile | str | name of the public cert file in /ssl folder |
| keyfile | str | name of the private key file in /ssl folder |
| backups | int | Amount of backups to keep. Set to 0 to disable backups |

## Default admin account
The first time the addon is started, an admin account is generated. Please change this password.
```
username: admin
password: admin
```

the admin panel can be found at `https://host:port/admin`

## Creating new account(s)
For self hosted EteSync solutions, the accounts have to be made in advance before using the sign up function. After logging into the admin panel, use the `Add` button next to `Users` to create a new account. After this user has been created, you can use any of the EteSync apps to signup with the same username in order to set up the account. The password used at that point will be used to setup the account. Don't forget to set your custom server address under "Advanced".
