directory                   | format   | notes
--------------------------- | -------- | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
_other_example_files        | various  |
countries-and-currencies    | CSV      | A Foreign Key example linking two CSV files in the same data package
cpi                         | CSV      | A CSV of Consumer price index (2010 = 100) by The World Bank.
cpi-data-via-url            | CSV      | CSV data referenced via a URL
donation-codes              | CSV      | Foreign key relationship with donations data package
donation-codes-schema       | JSON     | table schema only
donation-codes-via-url      | JSON     | CSV data, table schema and dialect all references via URLs
donations                   | CSV      | Example of the [Foreign Keys to Data Packages pattern](http://frictionlessdata.io/specs/patterns/#table-schema:-foreign-keys-to-data-packages)
finance-vix                 | CSV      | Data Package providing Volatility Index (VIX) Historical Price Data by [Cboe](http://www.cboe.com/)
geo-countries               | GeoJSON  | Countries in GeoJSON format
geo-lat-lon-as-numbers      | CSV      | A single csv file with location defined by two fields of type `number`, Latitude and Longitude
geo-location-fk             | CSV      | A CSV file with location defined by a field of `"type": "string" with a Foreign key relationship to another CSV file in the same package that contains point locations
geo-location-uri            | CSV      | A single CSV file with location defined by a field of `"type": "string",` `"format": "uri"`
geopoint-array              | CSV      | A single CSV file with location defined by a field of `type: GeoJSON`, `format: array`
geopoint-default            | CSV      | A single CSV file with location defined by a field of `type: GeoJSON`, `format: default`
geopoint-object             | CSV      | A single CSV file with location defined by a field of `type: GeoJSON`, `format: object`
gross-domestic-product-2014 | CSV      | A data package providing Country, regional and world GDP in current US Dollars ($) for 2014
gross-domestic-product-all  | CSV      | A data package providing Country, regional and world GDP in current US Dollars ($)
inflation                   | CSV      | A data package providing Annual growth rate of the GDP implicit deflator and Inflation measured by the consumer price index
iso-639-1-language-codes    | CSV      | This data package implements the [Language support](https://frictionlessdata.io/specs/patterns/#language-support) pattern. Some properties in the [data package](datapackage.JSON) have been given both English and Spanish values.
open-data-day-tweets-2018   | CSV      | Scripts to create Open Data Day 2018 Tweets periodic-table                                                                                                                                                                          | CSV | simple-GeoJSON | GeoJSON | text-file | txt | world-continents-topoJSON | topoJSON |
periodic-table              | CSV      | The Periodic Table as a data package
simple-geoJSON              | GeoJSON  | Example GeoJSON Data Package
text-file                   | TXT      | An example of a txt file providing non-tabular data inside a data package.
world-continents-topoJSON   | TopoJSON | Example World Continents TopoJSON Data Package
