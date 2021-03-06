# homebridge-hydrawise
[Hydrawise sprinkler system](https://hydrawise.com) plugin for [HomeBridge](https://github.com/nfarina/homebridge)

This repository contains the Hydrawise sprinkler system plugin for homebridge. 

# Installation


1. Install homebridge using: npm install -g homebridge
2. Install this plugin using: npm install -g homebridge-hydrawise
3. Update your configuration file. See sample-config.json snippet below. 

# Configuration

Configuration sample:

 ```
"platforms": [
		{
			"platform": "Hydrawise",
			"name": "Hydrawise",
			"api_key": "your API key",
			"default_runtime": "600",
			"polling_interval": "5000"
		}
	],

```

Fields: 

* "platform": Must always be "Hydrawise" (required)
* "name": Can be anything (required)
* "api_key": Can be found when going to 'My Account' on https://app.hydrawise.com (required)
* "default_runtime": Fallback duration in seconds if not able to detect the duration from Hydrawise (default 600)
* "polling_interval": Interval in ms between background status updates (default 5000)