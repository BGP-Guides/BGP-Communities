# Well-Known and Common Communities

| Group | Action | BGP Standard Community (RFC 1997) | 	BGP Extended Community (RFC 4360) | 	BGP Large Community (RFC 8092) | Comment |
|---|---|---|---|---|---|
| Well-Known | Well-known NO_EXPORT | 65535:65281 | rt:65535:65281 | N/A | |
| Well-Known | Well-known NO_ADVERTISE | 65535:65282 | rt:65535:65282 | N/A | |
| Well-Known | Well-known NO_EXPORT_SUBCONFED | 65535:65283 | rt:65535:65283 | N/A | not widely used, not implemented in all software |
| Well-Known | Well-known NO_PEER | 65535:65284 | rt:65535:65284 | N/A | not widely used, not implemented in all software |
| Common ASN based | Do not redistribute to $PEER-AS | 0:$PEER-AS | rt:0:$PEER-AS | $YOUR_AS:0:$PEER_AS | |
| Common ASN based | Redistribute to $PEER-AS | $YOUR_AS:$PEER-AS | rt:$YOUR_AS:$PEER-AS | $YOUR_AS:1:$PEER_AS | |
| Common general | Do not redistribute | 0:$YOUR_AS | rt:0:$YOUR_AS | $YOUR_AS:0:0 | |
| Common general | Redistribute to all (default) | $YOUR_AS:$YOUR_AS | rt:$YOUR_AS:$YOUR_AS | $YOUR_AS:1:0 | |
| Blackhole | Blackhole traffic for this annoncement | 65000:666 / 65535:666 | N/A | N/A | |
