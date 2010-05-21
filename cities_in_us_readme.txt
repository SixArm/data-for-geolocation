The cities file is generated from the MaxMind GPL cities of the world database.
Thanks to MaxMind.com for providing the data!

For details see http://drupal.org/node/19983

==Fields
  - Country code: two letters, upper case
  - United States state abbreviation: two letters, upper case
  - Name in English, in mixed case and with accents
  - Name in English, standardized to all lowercase and without accents
  - Latitude, as a decimal(10,7)
  - Longitude, as a decimal(10,7)

==Sample SQL
  CREATE TABLE cities (
    country char(2) NOT NULL default '',
    us_state char(2) NOT NULL default '',
    name_en varchar(30) NOT NULL default '',
    name_en_searchable varchar(30) NOT NULL default '',
    latitude decimal(10,7) NOT NULL default '0.0000000',
    longitude decimal(10,7) NOT NULL default '0.0000000'
  ) TYPE=MyISAM;

