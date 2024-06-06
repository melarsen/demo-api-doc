# Shipment.yaml
- Er sporingsnummer og sendingsnummer det samme? Men kollinummer er noe annet. Se Shipment objektet + Parcel. Kollinummer + sporingsnummer på parcel. Sendingsnummer + sporingsnummer på Shipment?
- LBH cm verdier som integer, ja!
- lastemeter, 
- weightGrams som integer, ja!
- 
- Er forskjell på Shipment og Parcel i requesten og Shipment og Parcel i responsen. Navngi disse slik at det gjenspeiler om de er i request eller response? (ParcelGoodsItem er bare i requesten)
  - ShipmentResponse.Shipment eller ShipmentBookingResponse.ShipmentResponse (inkl. ParcelResponse, )
  - AddressParty object - naming and content. Actor?
  - Alert eller "Feedback"? 
  - Regler for hvert produkt, skal vi uttrykke dette på noe vis i responsen eller ikke... Har ikke lagt det inn nå.
  - Har startet på Customer API også (tror vi trenger det), med tanke på fraktsalg-kunder vil vil kunne hente ut informasjon om disse + deres avtaler. Tror vi selv har behov for det, men kanskje ikke direkte ifm med frakt-booking.

- Hvis correlationId + data feiler.
  - Bruk samme correlationId + nye data. 
  - Må ha logikk for å håndtere feiling slik at disse faktisk blir booket på nytt.

- ValutaVerdi som integer i 100 øre (100dels)
- ValutaKode som string

- Har lagt inn commercial invoice info
- Har lagt inn fortollingsinfo
- Har lagt til pickup booking