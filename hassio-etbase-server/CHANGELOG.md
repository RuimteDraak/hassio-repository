Version 2023.04.1
- Exit setup scripts on error

There is a transient error where calls to home assistant sometimes fail unexpected. This change will stop the addon if this happens. Use the watchdog to restart the addon automatically.
