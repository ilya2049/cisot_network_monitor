# CISOT Network Monitor
Service is implemented with Ryu framework.

## Features
- Link delay measurement

## Launching
Debug mode: `ryu-manager --verbose --observe-links network_monitor.py `
Production mode: `ryu-manager --observe-links network_monitor.py `

## REST API
| method |          url          | Response Example                                   |
|--------|:---------------------:|----------------------------------------------------|
| GET    | /networkmonitor/links | [{"src_dpid": 1, "delay_ms": 1.8, "dst_dpid": 2}] |

## References
- Ryu framework home page is `https://osrg.github.io/ryu/`
- The link delay measurement approach is described in `https://ieeexplore.ieee.org/document/6727820`