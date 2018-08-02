# Codebook for U.S. President Precinct-Level Returns 2016

URL: http://dx.doi.org/10.7910/DVN/LYWX3D

Version: 2018-08-02

This codebook describes a dataset on precinct-level returns for elections to
the U.S. presidency.

Each record in the dataset gives the number of votes reported from a precinct
for a candidate.


## Variables

The dataset contains the following variables:

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
