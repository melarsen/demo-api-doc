# Shipment.yaml
- Er sporingsnummer og sendingsnummer det samme? Men kollinummer er noe annet. Se Shipment objektet + Parcel. Kollinummer + sporingsnummer på parcel. Sendingsnummer + sporingsnummer på Shipment?
- LBH verdier som integer, ja?
- weightKG som integer, ja?
- Er forskjell på Shipment og Parcel i requesten og Shipment og Parcel i responsen. Navngi disse slik at det gjenspeiler om de er i request eller response? (ParcelGoodsItem er bare i requesten)
  - ShipmentResponse.Shipment eller ShipmentBookingResponse.ShipmentResponse (inkl. ParcelResponse, )
  - AddressParty object - naming and content
  - Alert eller "Feedback"? 
  - Regler for hvert produkt, skal vi uttrykke dette på noe vis i responsen eller ikke... Har ikke lagt det inn nå.