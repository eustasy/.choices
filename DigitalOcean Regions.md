## DigitalOcean Regions

### Worldwide served from a single region

As both **Load Balancers** and **Private Networking** are only shared within regions, you may wish to serve worldwide from a single location. This is common for pairs of load balanced droplets providing redundancy for an application, while being able to share data over the internal network.

Selection in this case is usually based on where the majority of your end users reside, as latency is the largest detriment to the setup and scaling across regions may require additional, and frequently costly, services outside of DigitalOcean.

- NYC3
- AMS3

### Worldwide served from multiple regions for low latency

Sometimes coverage may be required across regions to keep latency low. In that case, covering major areas only once is usually sufficient, especially as areas with multiple regions available are served by a fast backbone.

- NYC3
- AMS3
- SGP1
- BLR1

### Region-specific legal requirements

Applications may wish to split regions by legality when handling sensitive data. You should always consult local law when processing a regions data.

- NYC3 for US, Canada, & Mexico
- AMS3 for GDPR Europe
- LON1 for non-GDPR Europe

### Region Locations

| Area           | Region Code   | Lacks  |
| -------------- | ------------- | ------ |
| US / Worldwide | NYC3          |        |
| US Alternate   | NYC1          | Spaces |
| US East Coast  | SFO2          |        |
| EU             | AMS3          |        |
| EU Alternate   | FRA1          |        |
| UK (Non-EU)    | LON1^         | Spaces |
| Asia / Oceania | SGP1*         |        |
| South America  | BLR1*         | Spaces, some Droplets |

_^ Not recommended unless there is a legal need for the region._  
_* Not recommended unless there is a strong penalty for latency._

### References
- [Regional Availability Matrix](https://www.digitalocean.com/docs/platform/availability-matrix/)
