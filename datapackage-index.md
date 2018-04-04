directory                   | format   | notes
--------------------------- | -------- | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
_other_example_files        | various  |
countries-and-currencies    | CSV      | A Foreign Key example linking two CSV files in the same data package
cpi                         | CSV      | A CSV of Consumer price index (2010 = 100) by The World Bank.
cpi-data-via-url            | CSV      | CSV data referenced via a URL
donation-codes              | CSV      |
donation-codes-schema       | json     | table schema only
donation-codes-via-url      | json     | CSV data, table schema and dialect all references via URLs
donations                   | CSV      | foreign keys across data packages
finance-vix                 | CSV      |
geo-countries               | GeoJSON  |
geo-lat-lon-as-numbers      | CSV      |
geo-location-fk             | CSV      | foreign key relationship to link place name to lat lon point
geo-location-uri            | CSV      | A single CSV file with location defined by `"type": "string",` `"format": "uri"`
geopoint-array              | CSV      | A single CSV file with location defined by `type: GeoJSON`, `format: array`
geopoint-default            | CSV      | A single CSV file with location defined by `type: GeoJSON`, `format: default`
geopoint-object             | CSV      | A single CSV file with location defined by `type: GeoJSON`, `format: object`
gross-domestic-product-2014 | CSV      |
gross-domestic-product-all  | CSV      |
inflation                   | CSV      |
iso-639-1-language-codes    | CSV      | This data package implements the [Language support](https://frictionlessdata.io/specs/patterns/#language-support) pattern. Some properties in the [data package](datapackage.json) have been given both English and Spanish values.
open-data-day-tweets-2018   | CSV      | Scripts to create Open Data Day 2018 Tweets periodic-table                                                                                                                                                                          | CSV | simple-GeoJSON | GeoJSON | text-file | txt | world-continents-topojson | topojson |
periodic-table              | CSV      |
simple-geojson              | GeoJSON  | Example GeoJSON Data Package
text-file                   | TXT      | An example of a txt file providing non-tabular data inside a data package.
world-continents-topojson   | TopoJSON | Example World Continents TopoJSON Data Package
