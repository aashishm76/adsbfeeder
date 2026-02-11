# ADS-B Feeder
ADS-B Feeder Project

Leverages SDR-Enthusiasts Ultrafeeder docker image to feed ADS-B flight data to various flight data exchanges (FlightAware, FlightRadar24, etc). 

## Active Feeds
| Site          | Feeding Data? |
| ------------- | ------------- | 
| FlightAware   | Yes           |
| FlightRadar24 | Yes           |
| ADSB Exchange | Yes           |

## Docker Images
Ultrafeeder - https://github.com/sdr-enthusiasts/docker-adsb-ultrafeeder?tab=readme-ov-file#mlat-configuration

PiAware - https://github.com/sdr-enthusiasts/docker-piaware

FlightRadar24 - https://github.com/sdr-enthusiasts/docker-flightradar24

## Metrics Monitoring

NOTE: Ultrafeeder image does not come with telegraf, must use the `telegraf` image tag to get the docker image with telegraf installed.

Metrics sent to Prometheus, using Grafana for visualization and monitoring

## URLs

- Main Map: http://your-server-ip:8080
- Graphs1090: http://your-server-ip:8080/graphs1090/
- Heatmap: http://your-server-ip:8080/?heatmap
- Replay: http://your-server-ip:8080/?replay
- PiAware Stats: http://your-server-ip:8081
- FR24 Stats: http://your-server-ip:8754
- Grafana: http://your-server-ip:3000 (login: admin/admin)
- Prometheus: http://your-server-ip:9090