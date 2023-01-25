# Home Assistant Configuration
My personal config - based on [Mattias's config](https://github.com/matt8707/hass-config)


![image](https://user-images.githubusercontent.com/93126880/203490436-2ed45a66-965b-4289-9b4a-26de1685903d.png)


## Features

* [Dashboard (Lovelace)](https://www.home-assistant.io/lovelace/) using custom [button-card](https://github.com/custom-cards/button-card) and [layout-card](https://github.com/thomasloven/lovelace-layout-card)
* Portrait, landscape and mobile view
* Less cluttered interface by displaying more information in a popup

### Sidebar

* Time and date with greeting based on time of day.
* Entities that are on.
* Temperature with emoji based on weather conditions.
* Waste notification. Displays what kind of waste is picked up, and when.
* Occasions info. Shows important dates so you don't forget.
* Other conditional alerts.

### Home Modes

HA is put into different modes throughout the day, based on what's happening - or not happening in the home.

Automations and scripts looks at the state of the Home Mode and takes actions based on that.

![image](https://user-images.githubusercontent.com/93126880/203490547-8f40a480-aaac-48d8-bfe5-6a2f7b0563b2.png)

Mode | Purpose
--- | ---
Comfort | Mood lighting with lower brightness.
Occupied | The home is occupied and nothing special is happening. Normal light levels during the day.
Sleep | Low light brightness levels, and some lights do not turn on from motion.
Empty | Home is unoccupied and entities are updated automatically.


### Media

Conditional media card. Displays currently active media player. If none is active, displays recent items from Plex.

![media-tilt](https://user-images.githubusercontent.com/93126880/187746806-00f313c0-fbc9-4904-882f-1ecf25f144b7.gif)


### Sliders

Shader position controls with [cover-popup-card](https://github.com/DBuit/cover-popup-card).

Media and volume controls with [media_player-popup-card](https://github.com/DBuit/media_player-popup-card).

Light brightness and color [light-popup-card](https://github.com/DBuit/light-popup-card).



| Blinds position | Media controls | Light brightness |
| --- | --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/204550984-306a3894-c852-439b-ad6f-56b16b64ca17.png) | ![image](https://user-images.githubusercontent.com/93126880/187842555-1fc1cdb0-3374-4ee3-afb8-d8e616404404.png) | ![image](https://user-images.githubusercontent.com/93126880/204550834-c943a0fb-70cc-4d98-8d81-bb3679fa7887.png) |


Circle slider which also shows previous value

![2023-01-25_12-03-03](https://user-images.githubusercontent.com/93126880/214547461-44479bc2-6b9e-405e-99cf-880ed61a9e4a.gif)



### Rooms

Room entities are grouped under one card.

![image](https://user-images.githubusercontent.com/93126880/202784390-46e0f1df-f8a6-4474-a3e9-265d5dbb2f72.png)

Example: All the Office entities are displayed as a popup with new button cards.

![image](https://user-images.githubusercontent.com/93126880/214548519-f42ce5fb-5ec0-4567-aca0-6aa32be3f43b.png)



### Footers

Popups that supports notifications.

![image](https://user-images.githubusercontent.com/93126880/187744558-fc281be5-af49-4433-976f-ce3af5bd7b0d.png)

#### RSS Feed

Using [feedparser](https://github.com/custom-components/feedparser) to gather data and displaying RSS feed with custom icons.

![image](https://user-images.githubusercontent.com/93126880/204553130-9de404bd-6636-4549-9709-ee061a96ac73.png)

#### Radarr

![image](https://user-images.githubusercontent.com/93126880/214549632-9c0178a7-8914-41b8-8e0a-03351034a9ef.png)



### Security

Cameras (Screenshots edited and blurred)

Displays all cameras with static images.

![image](https://user-images.githubusercontent.com/93126880/187852782-e32aeb7b-368b-4520-97f1-9728dc9a2a42.png)

Single camera with live feed.

![image](https://user-images.githubusercontent.com/93126880/187852631-e04fad27-f6d2-4a45-aa56-4c44dc55c58a.png)


### Screenshots

| PC | Plex |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/187849501-16c440c1-dbdb-49c0-ab6a-e8554dbd5d7b.png) | ![image](https://user-images.githubusercontent.com/93126880/187849560-74835322-65e7-49f2-9699-9714372aa02b.png) |

| Home Assistant | Tablet |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/187849727-56a42be2-40e4-4055-9e51-931e7264fc7c.png) | ![image](https://user-images.githubusercontent.com/93126880/187849789-7001698c-1e5d-4a31-9c44-4f53833ee6f6.png) |

| Network | WiFi QR code |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/214550581-b1b7b843-7e3d-4863-bc2b-7b4e8be99e14.png) | ![image](https://user-images.githubusercontent.com/93126880/214550628-0c0f5099-6b88-417b-bf6a-4c769ac97c33.png) |



| Climate | Electrical |
| --- | --- |
| ![image](https://user-images.githubusercontent.com/93126880/214549825-0ee3c5ad-524d-4697-aef0-307b1e791c38.png) | ![image](https://user-images.githubusercontent.com/93126880/187849966-bb4b5cdb-bcbb-4b33-bd05-d0225a4c0ba1.png) |

## Hardware

| Vendor | Product | Integration | Description |
|---|---|---|---|
| Samsung | Galaxy Tab A7 | [custom](https://github.com/cgarwood/homeassistant-fullykiosk) | Wall-mounted tablet |
| Ubiquiti | UniFi Dream Machine Pro | [unifi](https://www.home-assistant.io/integrations/unifi/) | Router, controller, firewall, switch |
| Synology | DiskStation RS1221+ | [synology_dsm](https://www.home-assistant.io/integrations/synology_dsm/) | 55TB NAS |
| Electrolama | zzh CC2652R1 | [zha](https://www.home-assistant.io/integrations/zha/) | 1 ZigBee Coordinator + 1 Router |
| Apple | TV 4K | [apple_tv](https://www.home-assistant.io/integrations/apple_tv/) | 2x set-top-boxes that streams content from Plex |
| NVIDIA | SHIELD Pro | [androidtv](https://www.home-assistant.io/integrations/androidtv/) | 1x set-top-box that streams lossless content from Plex |
