
----------

# Data Mappings

GBIF Terms | Vernon Fields |Notes| Example
------------ | -------------|-------|--------|
dcterms:references	| URI - Collections Online Link|
occurrenceID| 	Occurrence|Must be a GUID or an identifier that is near globally unique. Integer identifiers are not allowed.|"HAMAARAG:T0_L_049:6199"
dcterms:modified	| Last Update|
catalogNumber| 	Accession No|
typeStatus	| Classification Type Status|
verbatimEventDate	| Field Coll Date|If the original value has to be converted into ISO 8601 verbatimEventDate should be filled in with the original value.
recordedBy| 	Field Collector name only|The full names of each person acting in the event (e.g. collecting, observing, etc) should be entered in recordedBy using the vertical bar as a separator. Note there is a separate field for capturing the person(s) making the identification (see below).
maximumDepthInMeters	| Field Coll Depth to|
minimumDepthInMeters	| Field Coll Depth from|
verbatimDepth	| Field Coll Altitude to|
verbatimElevation| 	Field Coll Altitude from|
verbatimLocality| 	Ecological District|
decimalLatitude| 	Latitude export|The point location coordinates should be entered in decimal degrees in `decimalLatitude` and `decimalLongitude`. The spatial reference system upon which the coordinates are based must be entered in `geodeticDatum` using the EPSG code if known, e.g. "EPSG:4326". Otherwise use a controlled vocabulary for the name or code of the `geodeticDatum` if known, e.g. "WGS84". If none of these is known, use the value "unknown".|
decimalLongitude	| Longitude export|
geodeticDatum	| Datum|
scientificName	| Classification for GBIF|The full scientific name with authorship and date information if known must be entered in scientificName. To prevent ambiguity, the taxonRank of the scientific name should be supplied as per the GBIF Taxonomic Rank Vocabulary. Also to prevent ambiguity, as much higher taxonomy as possible should be filled in: kingdom, phylum, class, order, family, genus.|"Canis aureus Linnaeus, 1758"
taxonRank	| Taxon Rank| Must match [GBIF Taxon Rank Vocabulary](http://rs.gbif.org/vocabulary/gbif/rank_2015-04-24.xml) |"species"
order| 	Taxon - Order|Must be the full scientific name of the order in which the taxon is classified.|"Carnivora"
family| 	Taxon - Family|Must be the full scientific name of the family in which the taxon is classified.|  "Canidae"|
genus	| Taxon - Genus|Must be the full scientific name of the genus in which the taxon is classified|"Canis Linnaeus, 1758"
specificEpithet	| Taxon - Species|
infraspecificEpithet	| Taxon - Subname|
associatedMedia	| API image Link|
fieldNumber	| Field Coll Ref|
higherGeography	| Field Coll Place|
eventDate	| Field Collection Earliest|The date, date-time, date range, or date-time range during which the Event occurred should be entered in eventDate in ISO 8601 format. Partial dates can be provided if they have at least a year and month, e.g. "2007-03".|2007-03-20
institutionCode||A name or acronym of the institution acting in the event may be entered in institutionCode and ownerInstitutionCode. These can be different hence institutionCode can have physical custody of a specimen and ownerInstitutionCode can have legal ownership of the specimen.

## Mappings

1.	Add a Darwin core occurrence 
2.	Select source - should be the CSV exported from Vernon.
3.	The system should Auto fill 22 fields based on the field names.
4.	You need to add a few static fields
	- Basis of record = Preserved Specimen
	- type = PhysicalObject
	- Language = en
	- institutionCode = AK
	- collectionCode = AK
5.	Save
6.	Click resource title to return to main page
7.	Publish


## Todo

- [x] This is a complete item
- [ ] This is an incomplete item



