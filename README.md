# Precinct-Level Election Returns

This is the MEDSL repository for precinct-level election returns. We periodically publish its contents to our [Dataverse](https://dataverse.harvard.edu/dataverse/medsl_election_returns) and [website](https://electionlab.mit.edu/data).

The `2016-precinct-*` directories contain data and documentation for Dataverse datasets. Returns by state are in the `source` directory.


# Coverage

| State                   | Added      |
| ----------------------- | ---------- |
| Alabama                 | 2018-03-29 |
| Alaska                  | 2018-03-11 |
| Arizona                 | 2018-05-09 |
| Arkansas                | 2018-05-04 |
| California              | 2018-04-09 |
| Colorado                | 2018-03-11 |
| Connecticut             | 2018-03-11 |
| Delaware                | 2018-05-09 |
| District of Columbia    | 2018-03-11 |
| Florida                 | 2018-05-09 |
| Georgia                 | 2018-04-23 |
| Hawaii                  | 2018-03-29 |
| Idaho                   | 2018-03-11 |
| Illinois                | 2018-04-23 |
| Indiana                 |            |
| Iowa                    | 2018-04-23 |
| Kansas                  | 2018-04-23 |
| Kentucky                | 2018-04-23 |
| Louisiana               | 2018-03-11 |
| Maine                   | 2018-05-09 |
| Maryland                |            |
| Massachusetts           | 2018-03-29 |
| Michigan                | 2018-04-09 |
| Minnesota               | 2018-03-29 |
| Mississippi             | 2018-05-09 |
| Missouri                | 2018-05-10 |
| Montana                 | 2018-05-10 |
| Nebraska                | 2018-04-23 |
| Nevada                  | 2018-04-23 |
| New Hampshire           | 2018-05-10 |
| New Jersey              |            |
| New Mexico              | 2018-03-11 |
| New York                | 2018-04-23 |
| North Carolina          | 2018-03-29 |
| North Dakota            | 2018-03-11 |
| Ohio                    | 2018-04-23 |
| Oklahoma                | 2018-03-29 |
| Oregon                  | 2018-04-09 |
| Pennsylvania            | 2018-04-23 |
| Rhode Island            | 2018-03-29 |
| South Carolina          | 2018-03-29 |
| South Dakota            | 2018-04-09 |
| Tennessee               | 2018-03-11 |
| Texas                   | 2018-04-09 |
| Utah                    | 2018-04-23 |
| Vermont                 | 2018-04-09 |
| Virginia                | 2018-03-29 |
| Washington              | 2018-04-09 |
| West Virginia           | 2018-05-10 |
| Wisconsin               | 2018-03-29 |
| Wyoming                 | 2018-03-11 |



## Alabama

Added 2018-03-29.

  - Party-line voting appears in the data as `office` values of `Straight Party`
and `candidate` values of, for example, `Alabama Republican Party`. To
calculate vote totals, sum the votes candidates' received on their own lines
and from party-line voting.
  - The data don't yet include write-in votes for president.
  - No elections to the Alabama House or Senate were held in 2016.


## Alaska

Added 2018-03-11.

  - Because EAVS data are unavailable for Alaska, the `county_` identifiers for
county-equivalents are missing.


## Arizona

Added 2018-05-09.

  - Reporting counties were inconsistent in the use of accented characters.
Candidate name spellings aren't entirely consistent.
  - Returns from some counties do not yet give `district` values when office is
`State House` or `State Senate`.


## Arkansas

Added 2018-05-04.

  - In the raw data, it seems that votes for unopposed candidates sometimes appear
twice: once under a candidate's name and again in totals for all unopposed
candidates. But these totals are slightly lower than the sum of votes for all
unopposed candidates. We've dropped them.


## California

Added 2018-04-09.

  - Write-in votes are not yet included in the data. They're available only by
county from the [Secretary of State](http://www.sos.ca.gov/elections/prior-
elections/statewide-election-results/general-election-
november-8-2016/statement-vote). (Our precinct-level returns are from the
[Statewide Database](http://statewidedatabase.org/d10/g16.html).)


## Colorado

Added 2018-03-11.


## Connecticut

Added 2018-03-11.


## Delaware

Added 2018-05-09.

  - The data don't yet include write-in votes.


## District of Columbia

Added 2018-03-11.

  - The data don't yet include write-in votes for president.
  - Returns for the Council and Advisory Referendum can be found in the `state`
dataverse. Advisory Neighborhood Commission returns are in the `local`
dataverse.


## Florida

Added 2018-05-09.


## Georgia

Added 2018-04-23.

  - The data don't yet include third-party or write-in votes for president.


## Hawaii

Added 2018-03-29.

  - Kalawao County is the only county in Hawaii that doesn't appear as a
`jurisdiction` or `county_name`; it doesn't administer elections.


## Idaho

Added 2018-03-11.

  - The data don't yet include elections to the Idaho House and Senate.


## Illinois

Added 2018-04-23.

  - Illinois jurisdictions are counties, with the exception of these six cities:
Aurora, Bloomington, Chicago, Danville, East St. Louis, Galesburg, and
Rockford. We joined their returns with `county_` identifiers by jurisdiction
and precinct, using the jurisdiction given by the `JurisContainerID` variable
in the source data.


## Indiana

Not yet included.

  - There are inconsistencies in `candidate` spellings following OCR. Values in the
`votes` column may also be affected.
  - Vote counts are too high, compared to county-level returns.


## Iowa

Added 2018-04-23.


## Kansas

Added 2018-04-23.


## Kentucky

Added 2018-04-23.


## Louisiana

Added 2018-03-11.

  - No elections to the Louisiana House or Senate were held in 2016.


## Maine

Added 2018-05-09.

  - County identifiers aren't yet available for all jurisdictions.


## Maryland

Not yet included.

  - In the current release, only election-day votes are included. Other vote modes
are reported at the county level, and we need to append them to the precinct-
level returns.


## Massachusetts

Added 2018-03-29.


## Michigan

Added 2018-04-09.

  - The data don't yet include write-in votes for president.
  - Note when aggregating over `precinct` the rows that represent "statistical
adjustments."


## Minnesota

Added 2018-03-29.

  - The data don't yet include write-in votes for president.
  - Democratic candidate `party` values are left as `Democratic-Farmer-Labor`.


## Mississippi

Added 2018-05-09.

  - In the current release, values of `district` are missing where `office` is
`State House`.


## Missouri

Added 2018-05-10.

  - County identifiers are unavailable for Kansas City returns, which are reported
by the municipality. (The associated Census Place FIPS is `2938000`.) In the
future we may include sub-county and place identifiers.


## Montana

Added 2018-05-10.

  - The data don't yet include write-in votes for president.


## Nebraska

Added 2018-04-23.

  - The data don't yet include write-in votes.
  - There are no returns for local races.
  - Nebraska Legislature returns appear with an `office` value of `State Senate`.


## Nevada

Added 2018-04-23.

  - Some jurisdictions suppressed returns from low-turnout precincts to preserve
ballot secrecy. Details forthcoming.


## New Hampshire

Added 2018-05-10.

  - The data don't yet include write-in votes for president.
  - The data don't yet include returns for state legislative or local races.


## New Jersey

Not yet included.

  - There's extensive double-counting of returns from inconsistency across
municipalities in use of total rows.


## New Mexico

Added 2018-03-11.


## New York

Added 2018-04-23.

  - Candidate names for lower office are not always consistent across counties.


## North Carolina

Added 2018-03-29.


## North Dakota

Added 2018-03-11.

  - The data don't yet include write-in votes for president.


## Ohio

Added 2018-04-23.

  - The data don't yet include write-in votes for president.


## Oklahoma

Added 2018-03-29.

  - No general election was held for the first U.S. House district after Jim
Bridenstine's opponent withdrew and left him unopposed.


## Oregon

Added 2018-04-09.


## Pennsylvania

Added 2018-04-23.


## Rhode Island

Added 2018-03-29.

  - The data don't yet include write-in votes for president.


## South Carolina

Added 2018-03-29.

  - Party-line voting appears in the data as `office` and `candidate` values of
`Straight ticket`. Compute candidates' vote totals as the sum of the votes they
received on their own lines and from party-line voting.


## South Dakota

Added 2018-04-09.


## Tennessee

Added 2018-03-11.

  - There are no returns for local races.


## Texas

Added 2018-04-09.

  - The data don't yet include write-in votes for president.
  - There are no returns for local races.


## Utah

Added 2018-04-23.


## Vermont

Added 2018-04-09.

  - The data don't yet include write-in votes for president, except for the ~18,000
cast for Bernie Sanders and reported at the precinct level.


## Virginia

Added 2018-03-29.

  - The data don't yet include write-in votes for president.


## Washington

Added 2018-04-09.

  - King County results appear for now as county aggregates.
  - The data don't yet include about 108,000 write-in votes for president, which
are available at the county level.


## West Virginia

Added 2018-05-10.

  - The data don't yet include write-in votes for president.


## Wisconsin

Added 2018-03-29.

  - Presidential returns are post-recount.
  - The data don't yet include write-in votes for president.


## Wyoming

Added 2018-03-11.

  - The data don't yet include write-in votes for president.


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
