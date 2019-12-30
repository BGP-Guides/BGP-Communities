# Operational Communities

| Group | Action | BGP Standard Community (RFC 1997) | 	BGP Extended Community (RFC 4360) | 	BGP Large Community (RFC 8092) | Comment |
|---|---|---|---|---|---|
| Continent based | Identify the continent from where the route is originated | $YOUR_AS:$M49_CONTINENT_ID | rt:$YOUR_AS:$M49_CONTINENT_ID | N/A | |
| Country based | Identify the country from where the route is originated | $YOUR_AS:$M49_COUNTRY_ID | rt:$YOUR_AS:$M49_COUNTRY_ID | N/A | |
| Metro based | Identify the metropolitan area from where the route is originated | $YOUR_AS:$METRO_ID | rt:$YOUR_AS:$METRO_ID | N/A | |