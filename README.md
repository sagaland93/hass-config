# Home Assistant Configuration
My personal config - based on [Mattias's config](https://github.com/matt8707/hass-config)


![image](https://user-images.githubusercontent.com/93126880/187745637-cb682c44-f131-493d-945b-cee3a064f1ea.png)


## Features

* [Dashboard (Lovelace)](https://www.home-assistant.io/lovelace/) using custom [button-card](https://github.com/custom-cards/button-card) and [layout-card](https://github.com/thomasloven/lovelace-layout-card)
* Portrait, landscape and mobile view
* Less cluttered interface by displaying more information in a popup

#### Sidebar

* Time and date with greeting based on time of day.
* Entities that are on.
* Temperature with emoji based on weather conditions.
* Waste notification. Displays what kind of waste is picked up, and when.
* Occasions info. Shows important dates so you don't forget.
* Other conditional alerts.

#### Home Modes

HA is put into different modes throughout the day, based on what's happening - or not happening in the home.

Automations and scripts looks at the state of the Home Mode and takes actions based on that.

![image](https://user-images.githubusercontent.com/93126880/187847146-6289ec27-e0dd-427d-bd6e-2243af6035e2.png)

Mode | Purpose
--- | ---
Comfort | Mood lighting with lower brightness.
Occupied | The home is occupied and nothing special is happening. Normal light levels during the day.
Sleep | Low light brightness levels, and some lights do not turn on from motion.
Empty | Home is unoccupied and entities are updated automatically.

#### Media

Conditional media card. Displays currently active media player. If none is active, displays recent items from Plex.

![media-tilt](https://user-images.githubusercontent.com/93126880/187746806-00f313c0-fbc9-4904-882f-1ecf25f144b7.gif)

Volume controls with [media_player-popup-card](https://github.com/DBuit/media_player-popup-card).

![image](https://user-images.githubusercontent.com/93126880/187842555-1fc1cdb0-3374-4ee3-afb8-d8e616404404.png)



#### Blinds

Shader position controls with [cover-popup-card](https://github.com/DBuit/cover-popup-card).

![blinds-control](https://user-images.githubusercontent.com/93126880/187845173-4da0fdb6-bb24-4528-8b2e-3b738a38b60a.gif)


#### Rooms

Room entities are grouped under one card.

![rooms2-short](https://user-images.githubusercontent.com/93126880/187751467-eb873846-452c-4334-acda-2f9a05e6d7ba.gif)

Example: All the Office entities are displayed as a popup with new button cards.

![office](https://user-images.githubusercontent.com/93126880/187751207-17268f49-a907-4b35-93ea-35258e6d93eb.gif)


#### Footers

Popups that supports notifications.

![image](https://user-images.githubusercontent.com/93126880/187744558-fc281be5-af49-4433-976f-ce3af5bd7b0d.png)

RSS Feed

Using [feedparser](https://github.com/custom-components/feedparser) to gather data and displaying RSS feed with custom icons.

![rss-feed](https://user-images.githubusercontent.com/93126880/187744661-00a74549-344d-466e-98e1-6982ed8e24dc.gif)


Popup displayed when the RSS footer is clicked.

![image](https://user-images.githubusercontent.com/93126880/187751839-4a3b5f65-8a5f-4bf8-92eb-0ff0ec3fba01.png)

## Security

Cameras (Screenshots edited and blurred)

Displays all cameras with static images.

![image](https://user-images.githubusercontent.com/93126880/187852782-e32aeb7b-368b-4520-97f1-9728dc9a2a42.png)

Single camera with live feed.

![image](https://user-images.githubusercontent.com/93126880/187852631-e04fad27-f6d2-4a45-aa56-4c44dc55c58a.png)


## Screenshots

| PC | Plex |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/187849501-16c440c1-dbdb-49c0-ab6a-e8554dbd5d7b.png) | ![image](https://user-images.githubusercontent.com/93126880/187849560-74835322-65e7-49f2-9699-9714372aa02b.png) |

| Home Assistant | Tablet |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/187849727-56a42be2-40e4-4055-9e51-931e7264fc7c.png) | ![image](https://user-images.githubusercontent.com/93126880/187849789-7001698c-1e5d-4a31-9c44-4f53833ee6f6.png) |

| Climate | Electrical |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/187849936-98bba209-2aa5-4aef-9640-08688a58970e.png) | ![image](https://user-images.githubusercontent.com/93126880/187849966-bb4b5cdb-bcbb-4b33-bd05-d0225a4c0ba1.png) |

## Hardware

| Vendor | Product | Integration | Description |
|---|---|---|---|
| Samsung | Galaxy Tab A7 | [custom](https://github.com/cgarwood/homeassistant-fullykiosk) | Wall-mounted tablet |
| Ubiquiti | UniFi Dream Machine Pro | [unifi](https://www.home-assistant.io/integrations/unifi/) | Router, controller, firewall, switch |
| Synology | DiskStation RS1221+ | [synology_dsm](https://www.home-assistant.io/integrations/synology_dsm/) | 55TB NAS |
| Electrolama | zzh CC2652R1 | [zha](https://www.home-assistant.io/integrations/zha/) | 1 ZigBee Coordinator + 1 Router |
| Apple | TV 4K | [apple_tv](https://www.home-assistant.io/integrations/apple_tv/) | 2x set-top-boxes that streams content from Plex |
| NVIDIA | SHIELD Pro | [androidtv](https://www.home-assistant.io/integrations/androidtv/) | 1x set-top-box that streams lossless content from Plex |
