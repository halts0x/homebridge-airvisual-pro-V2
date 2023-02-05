1. Improve initialisation of AirQuality values into homekit on startup 
2.Set custom AQ trigger levels in config

# homebridge-airvisual-pro

[AirVisual Pro](https://www.airvisual.com/air-quality-monitor) plugin for [Homebridge](https://github.com/nfarina/homebridge).

# Installation

1. Install Homebridge using: `[sudo] npm install -g homebridge`
2. Install this plugin using: `[sudo] npm install -g homebridge-airvisual-pro-v2`
3. Update your configuration file. See the sample below.

# Updating

- `[sudo] npm install -g homebridge-airvisual-pro-v2`

# Configuration

## Sample Configuration

```json
"accessories": [
        {
    "accessory": "AirVisualPro",
    "name": "AirVisualPro",
    "ip": "192.168.1.101",
    "user": "airvisual",
    "pass": "passw0rd",
    "co2_critical": 1000,
    "AQExcellent": 11,
    "AQGood": 24,
    "AQFair": 45,
    "AQinf": 65,
    "logging": false,
        }
]
```

## Workaround
smbclient package is required. `sudo apt-get install smbclient`

#Credits
Based on the great work of [macnow/homebridge-airvisual-node](https://github.com/macnow/homebridge-airvisual-node).
