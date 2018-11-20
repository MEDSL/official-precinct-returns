# Precinct-Level Election Returns

This is the MEDSL repository for precinct-level election returns. We periodically publish its contents to our [Dataverse](https://dataverse.harvard.edu/dataverse/medsl_election_returns) and [website](https://electionlab.mit.edu/data).

The `2016-precinct-*` directories contain returns organized by office (as on Dataverse):

* [U.S. President](https://github.com/MEDSL/precinct-returns/tree/master/2016-precinct-president)
* [U.S. Senate](https://github.com/MEDSL/precinct-returns/tree/master/2016-precinct-senate)
* [U.S. House](https://github.com/MEDSL/precinct-returns/tree/master/2016-precinct-house)
* [State offices](https://github.com/MEDSL/precinct-returns/tree/master/2016-precinct-state)
* [Local offices](https://github.com/MEDSL/precinct-returns/tree/master/2016-precinct-local)

Returns by state are in the `source` directory. These are alternative partitions of the same data.


# Coverage


## Alabama: 2016

Added 2018-03-29.

  - Party-line voting appears in the data as `office` values of `Straight Party`
and `candidate` values of, for example, `Alabama Republican Party`. To
calculate vote totals, sum the votes candidates' received on their own lines
and from party-line voting.


## Alaska: 2016

Added 2018-03-11.

  - Because EAVS data are unavailable for Alaska, the `county_` identifiers for
county-equivalents are missing.


## Arizona: 2016

Added 2018-05-09.

  - Reporting counties were inconsistent in the use of accented characters.
Candidate name spellings aren't entirely consistent.
  - Returns from some counties do not yet give `district` values when office is
`State House` or `State Senate`.


## Arkansas: 2016

Added 2018-05-04.

  - In the raw data, it seems that votes for unopposed candidates sometimes appear
twice: once under a candidate's name and again in totals for all unopposed
candidates. But these totals are slightly lower than the sum of votes for all
unopposed candidates. We've dropped them.


## California: 2016

Added 2018-04-09.


## Colorado: 2016

Added 2018-03-11.


## Connecticut: 2016

Added 2018-03-11.


## Delaware: 2016

Added 2018-05-09.


## District of Columbia: 2016

Added 2018-03-11.

  - Returns for the Council and Advisory Referendum can be found in the `state`
dataverse. Advisory Neighborhood Commission returns are in the `local`
dataverse.


## Florida: 2016

Added 2018-05-09.


## Georgia: 2016

Added 2018-04-23.


## Hawaii: 2016

Added 2018-03-29.

  - Kalawao County is the only county in Hawaii that doesn't appear as a
`jurisdiction` or `county_name`; it doesn't administer elections.


## Idaho: 2016

Added 2018-03-11.

  - Idaho House and Senate returns were added 2018-06-12.


## Illinois: 2016

Added 2018-04-23.

  - Illinois jurisdictions are counties, with the exception of these six cities:
Aurora, Bloomington, Chicago, Danville, East St. Louis, Galesburg, and
Rockford. We joined their returns with `county_` identifiers by jurisdiction
and precinct, using the jurisdiction given by the `JurisContainerID` variable
in the source data.


## Indiana: 2016

Added 2018-06-05.

  - Candidate names for lower office are not always consistent across counties.


## Iowa: 2016

Added 2018-04-23.


## Kansas: 2016

Added 2018-04-23.


## Kentucky: 2016

Added 2018-04-23.


## Louisiana: 2016

Added 2018-03-11.

  - No elections to the Louisiana House or Senate were held in 2016.


## Maine: 2016

Added 2018-05-09.

  - County identifiers aren't yet available for all jurisdictions.


## Maryland: 2016

Added 2018-06-04.


## Massachusetts: 2016

Added 2018-03-29.


## Michigan: 2016

Added 2018-04-09.

  - Note when aggregating over `precinct` the rows that represent "statistical
adjustments."


## Minnesota: 2016

Added 2018-03-29.

  - Democratic candidate `party` values are left as `Democratic-Farmer-Labor`.


## Mississippi: 2016

Added 2018-05-09.

  - In the current release, values of `district` are missing where `office` is
`State House`.


## Missouri: 2016

Added 2018-05-10.

  - County identifiers are unavailable for Kansas City returns, which are reported
by the municipality. (The associated Census Place FIPS is `2938000`.) In the
future we may include sub-county and place identifiers.


## Montana: 2016

Added 2018-05-10.


## Nebraska: 2016

Added 2018-04-23.

  - There are no returns for local races.
  - Nebraska Legislature returns appear with an `office` value of `State Senate`.


## Nevada: 2016

Added 2018-04-23.

  - Some jurisdictions suppressed returns from low-turnout precincts to preserve
ballot secrecy. Details forthcoming.


## New Hampshire: 2016

Added 2018-05-10.

  - State legislative returns are post-recount, and added 2018-06-12.


## New Jersey: 2016

Added 2018-06-04.

  - Candidate names for lower office are not always consistent across counties.


## New Mexico: 2016

Added 2018-03-11.


## New York: 2016

Added 2018-04-23.

  - Candidate names for lower office are not always consistent across counties.


## North Carolina: 2016

Added 2018-03-29.


## North Dakota: 2016

Added 2018-03-11.


## Ohio: 2016

Added 2018-04-23.


## Oklahoma: 2016

Added 2018-03-29.

  - No general election was held for the first U.S. House district after Jim
Bridenstine's opponent withdrew and left him unopposed.


## Oregon: 2016

Added 2018-04-09.


## Pennsylvania: 2016

Added 2018-04-23.


## Rhode Island: 2016

Added 2018-03-29.


## South Carolina: 2016

Added 2018-03-29.

  - Party-line voting appears in the data as `office` and `candidate` values of
`Straight ticket`. Compute candidates' vote totals as the sum of the votes they
received on their own lines and from party-line voting.


## South Dakota: 2016

Added 2018-04-09.


## Tennessee: 2016

Added 2018-03-11.

  - There are no returns for local races.


## Texas: 2016

Added 2018-04-09.

  - There are no returns for local races.
  - Returns for uncontested races to the Texas House of Representatives do not
appear in the data.


## Utah: 2016

Added 2018-04-23.


## Vermont: 2016

Added 2018-04-09.


## Virginia: 2016

Added 2018-03-29.


## Washington: 2016

Added 2018-04-09.

  - King County results appear for now as county aggregates.


## West Virginia: 2016

Added 2018-05-10.

  - The data don't yet include write-in votes for president.


## Wisconsin: 2016

Added 2018-03-29.

  - Presidential returns are post-recount.


## Wyoming: 2016

Added 2018-03-11.


# Codebook

Datasets contain the following variables:

- `year`
- `state`
- `state_postal`
- `state_fips`
- `state_icpsr`
- `county_name`
- `county_ansi`
- `county_fips`
- `county_lat`
- `county_long`
- `jurisdiction`
- `precinct`
- `office`
- `district`
- `stage`
- `special`
- `candidate`
- `candidate_last`
- `candidate_first`
- `candidate_middle`
- `candidate_normalized`
- `candidate_full`
- `candidate_suffix`
- `candidate_nickname`
- `candidate_fec`
- `candidate_fec_name`
- `candidate_google`
- `candidate_govtrack`
- `candidate_icpsr`
- `candidate_maplight`
- `candidate_opensecrets`
- `candidate_wikidata`
- `candidate_party`
- `writein`
- `party`
- `mode`
- `votes`


### year

Year of election.


### state

State name.


### state_postal

State U.S. Postal Service abbreviation (two-letter ISO 1366 code).


### state_fips

Numeric state FIPS 5-2 code.


### state_icpsr

Numeric ICPSR state code.


### county_name

County name.

Source: Census Bureau [National Counties Gazetteer
File](https://www.census.gov/geo/maps-data/data/gazetteer2017.html).


### county_ansi

County ANSI code.

Source: Census Bureau [National Counties Gazetteer
File](https://www.census.gov/geo/maps-data/data/gazetteer2017.html).


### county_fips

Numeric FIPS 6-4 code, the concatenation of two-digit `state_fips` and three-
digit county FIPS codes.

Source: Census Bureau [National Counties Gazetteer
File](https://www.census.gov/geo/maps-data/data/gazetteer2017.html).


### county_lat

County latitude (decimal degrees).

Source: Census Bureau [National Counties Gazetteer
File](https://www.census.gov/geo/maps-data/data/gazetteer2017.html).


### county_long

County longitude (decimal degrees).

Source: Census Bureau [National Counties Gazetteer
File](https://www.census.gov/geo/maps-data/data/gazetteer2017.html).


### jurisdiction

The name of the administrative jurisdiction, typically a county, as it appeared
in source data.

Source: Precinct returns for `jurisdiction`.


### precinct

The name of the precinct, as it appeared in source data.

Source: Precinct returns for `jurisdiction`.


### office

The office for which the `candidate` ran.

Source: Precinct returns for `jurisdiction`.


### district

District associated with the `office`, where applicable.

Source: Precinct returns for `jurisdiction`.


### stage

The electoral stage, either `gen` for general elections or `pri` for primary
elections.


### special

Whether the election was a special election, either `TRUE` for special
elections or `FALSE` otherwise.

Source: Precinct returns for `jurisdiction`.


### candidate

The name of the candidate.

Candidate names are standardized across jurisdictions.

Source: Precinct returns for `jurisdiction`.


### candidate_last

Candidate's last name.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_first

Candidate's first name.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_middle

Candidate's middle name.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_normalized

A normalizing transformation of the candidate's name for joins by name. This is
a single word from `candidate`, usually the last name, in lowercase. In the
case of hyphenated names, only the final name is included.

Source: MEDSL.


### candidate_full

Candidate's official full name.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_suffix

Candidate name suffix.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_nickname

Candidate's nickname.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_fec

Candidate's [FEC
identifier](https://www.fec.gov/data/advanced/?tab=candidates). Multiple FEC
IDs appear concatenated, separated by a semicolon and space (`; `).

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project and [FEC](https://www.fec.gov/data/advanced/?tab=candidates).


### candidate_fec_name

Candidate's name as it appears in FEC data.

Source: [FEC](https://www.fec.gov/data).


### candidate_google

Candidate's [Google Knowledge Graph](https://developers.google.com/knowledge-
graph) entity identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_govtrack

Candidate's [GovTrack.us](https://www.govtrack.us) identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_icpsr

Candidate's [ICPSR](https://www.icpsr.umich.edu) identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_maplight

Candidate's [MapLight](https://maplight.org) identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_opensecrets

Candidate's [OpenSecrets.org](https://www.opensecrets.org) identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_wikidata

Candidate's [WikiData](https://www.wikidata.org) identifier.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### candidate_party

Candidate's party affiliation. Values may differ from `party`, which gives the
candidate's party on the ballot.

Source: The [@unitedstates](https://github.com/unitedstates/congress-legislators)
project.


### writein

Whether the record describes a write-in candidate, either `TRUE` or `FALSE`.

Source: Precinct returns for `jurisdiction`.


### party

Party of the `candidate`, where applicable. Candidates may run on multiple
party lines, so to compute two-party vote shares or candidate vote totals,
aggregate over `party`.

Party names are standardized across jurisdictions.

Source: Precinct returns for `jurisdiction`.


### mode

Vote mode, e.g., `mail` or `Election Day`.

Source: Precinct returns for `jurisdiction`.


### votes

Number of votes received.

Source: Precinct returns for `jurisdiction`.
