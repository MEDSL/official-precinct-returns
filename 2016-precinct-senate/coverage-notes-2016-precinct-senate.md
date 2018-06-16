# Coverage in U.S. Senate Precinct-Level Returns 2016

URL: http://dx.doi.org/10.7910/DVN/NLTQAD

Version: 2018-06-16

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
| Indiana                 | 2018-06-05 |
| Iowa                    | 2018-04-23 |
| Kansas                  | 2018-04-23 |
| Kentucky                | 2018-04-23 |
| Louisiana               | 2018-03-11 |
| Maine                   | 2018-05-09 |
| Maryland                | 2018-06-04 |
| Massachusetts           | 2018-03-29 |
| Michigan                | 2018-04-09 |
| Minnesota               | 2018-03-29 |
| Mississippi             | 2018-05-09 |
| Missouri                | 2018-05-10 |
| Montana                 | 2018-05-10 |
| Nebraska                | 2018-04-23 |
| Nevada                  | 2018-04-23 |
| New Hampshire           | 2018-05-10 |
| New Jersey              | 2018-06-04 |
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

  - Idaho House and Senate returns were added 2018-06-12.


## Illinois

Added 2018-04-23.

  - Illinois jurisdictions are counties, with the exception of these six cities:
Aurora, Bloomington, Chicago, Danville, East St. Louis, Galesburg, and
Rockford. We joined their returns with `county_` identifiers by jurisdiction
and precinct, using the jurisdiction given by the `JurisContainerID` variable
in the source data.


## Indiana

Added 2018-06-05.

  - Candidate names for lower office are not always consistent across counties.
  - The data don't yet include write-in votes for president, with the exception of
returns from La Porte and Marshall.


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

Added 2018-06-04.


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

  - State legislative returns are post-recount, and added 2018-06-12.


## New Jersey

Added 2018-06-04.

  - Candidate names for lower office are not always consistent across counties.


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