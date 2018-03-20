# Where we send our data

## GBIF
GBIF—the Global Biodiversity Information Facility—is an international network and research infrastructure funded by the world’s governments and aimed at providing anyone, anywhere, open access to data about all types of life on Earth.
[View AM records](https://www.gbif.org/publisher/32e82a64-c9b4-4b2f-9fbd-d446309b973f)
## ALA
The ALA is Australia’s national biodiversity database. Founded on the principle of data sharing – collect it once, share it, use it many times – the ALA provides free, online access to millions of occurrence records to form the most comprehensive and accessible data set on Australia’s biodiversity ever produced.  
[View AM records](https://collections.ala.org.au/public/show/co249)

## Virtual Herbarium
Australian and New Zealand herbaria house over eight million plant, algae and fungi specimens. Herbarium specimens are an important resource for research on the Australasian flora and provide a permanent record of the occurrence of a species at a particular place and time. The AVH provides access to the collecting data associated with these specimens.


----------

# Data Mappings

GBIF Terms | Vernon Fields
------------ | -------------
dcterms:references	| URI - Collections Online Link
occurrenceID| 	Occurrence
dcterms:modified	| Last Update
catalogNumber| 	Accession No
typeStatus	| Classification Type Status
verbatimEventDate	| Field Coll Date
recordedBy| 	Field Collector name only
maximumDepthInMeters	| Field Coll Depth to
minimumDepthInMeters	| Field Coll Depth from
verbatimDepth	| Field Coll Altitude to
verbatimElevation| 	Field Coll Altitude from
verbatimLocality| 	Ecological District
decimalLatitude| 	Latitude export
decimalLongitude	| Longitude export
geodeticDatum	| Datum
scientificName	| Classification for GBIF
taxonRank	| Taxon Rank
order| 	Taxon - Order
family| 	Taxon - Family
genus	| Taxon - Genus
specificEpithet	| Taxon - Species
infraspecificEpithet	| Taxon - Subname
associatedMedia	| API image Link
fieldNumber	| Field Coll Ref
higherGeography	| Field Coll Place
eventDate	| Field Collection Earliest

##Mappings

1.	Add a Darwin core occurrence 
2.	Select source - should be the CSV exported from Vernon.
3.	The system should Auto fill 22 fields based on the field names.
4.	You need to add a few static fields
	5.	Basis of record = Preserved Specimen
	6.	type = PhysicalObject
	6.	Language = en
	7.	institutionCode = AK
	8.	collectionCode = AK
5.	Save
6.	Click resource title to return to main page
7.	Publish


##Todo

- [x]
- [ ]




