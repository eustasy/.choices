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

#### Additional regions for larger deployments

More American: Add SFO2  
More European: Add FRA1

### Worldwide served from multiple regions for capacity

Large-file storage is common for downloads, and such a network will benefit little from latency improvements, but more local distribution can still be noticeably faster and more stable. These are typically built on the smallest droplets availabe, as larger systems see no improvement on link speed or bandwidth allocation.

1. NYC3
2. AMS3
3. SFO2
4. FRA1
5. SGP1
6. BLR1

### Region-specific legal requirements

Applications may wish to split regions by legality when handling sensitive data. You should always consult local law when processing a regions data.

- NYC3 for US, Canada, & Mexico
- AMS3 for GDPR Europe
- LON1 for non-GDPR Europe

### PCI-DSS Compliance

All regions are PCI-DSS compliant.

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
| Asia / Oceania | BLR1*         | Spaces, some Droplets |

_^ Not recommended unless there is a legal need for the region, or a strong regional presence._  
_* Not recommended unless there is a strong penalty for latency, or a strong regional presence._  

### References
- [Regional Availability Matrix](https://docs.digitalocean.com/products/platform/availability-matrix/)
- [Datacenter Security & Privacy Certifications](https://www.digitalocean.com/trust/certification-reports/)
