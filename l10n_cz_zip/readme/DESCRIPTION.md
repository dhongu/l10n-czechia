Loads the Czech localities (obce) with their postal code and region, and fills in the
city and the region of Czech addresses from the postal code.

- Ships the list of Czech localities with their postal code, linked to the regions of Czechia. The data
  comes from [GeoNames](https://www.geonames.org) (Creative Commons Attribution 4.0).
- Czechia is set to *enforce cities*: the city of a Czech address is chosen from the list.
- On the contact form, typing the postal code (PSČ) of a Czech address sets the city and the
  region. A postal code shared by several localities sets only the region; the city name, when it matches
  one of them (without accents and case), picks the locality.
- The action *Czechia: set city from ZIP* on contacts links the Czech contacts to the city of their postal
  code and fills in the region.
- At install, the Czech contacts are linked: directly on a small database, by the scheduled action
  *Czechia: link contacts to the city of their ZIP* in batches on a large one (it deactivates itself when done).
- Every form that runs the postal code rules of the contact (for example the delivery details of an AWB)
  gets the region filled in, so the shipment can be sent to Czechia without looking it up by hand.
