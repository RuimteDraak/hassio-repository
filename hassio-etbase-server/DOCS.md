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
