# Release Notes for U.S. President Precinct-Level Returns 2016

URL: http://dx.doi.org/10.7910/DVN/LYWX3D


## 2018-08-02

Adds write-in votes requested from jurisdictions.


## 2018-07-16

This release adds write-in votes in California, DC, Delaware, Georgia, Indiana,
Michigan, Minnesota, Montana, Nebraska, North Dakota, Ohio, Rhode Island,
Texas, Vermont, Virginia, Washington, Wisconsin, and Wyoming. It also
incorporates ongoing work on data quality across the states.


## 2018-06-16

In this release, we add returns for local races in New Hampshire, and improve
the data for Kentucky and New York by removing duplicative rows that inflated
vote counts.


## 2018-06-15

This bugfix release assigns Arizona returns to the correct archives/dataverses,
and adds excluded returns from Tillamook County, Oregon.


## 2018-06-12

The data now include state legislative returns from New Hampshire and Idaho,
and presidential write-in votes from new Hampshire.


## 2018-06-05

This release brings coverage to all 50 states and DC, by adding precinct-level
returns from Indiana, Maine, Maryland, Mississippi, Missouri, Montana, New
Hampshire, New Jersey, and West Virginia.

The remaining gaps in coverage are
(1) returns for state legislative elections in Idaho and New Hampshire; (2)
local-election returns from 4 states; and (3) write-in votes in 21 states. For
details, see the coverage notes.


## 2018-04-23

This release adds precinct-level returns from Georgia, Illinois, Iowa, Kansas,
Kentucky, Nebraska, Nevada, New York, Ohio, Pennsylvania, and Utah.


## 2018-04-09

We've added identifiers for candidates in U.S. House and Senate races. [FEC
IDs](https://www.fec.gov/data) are present for nearly all candidates. A
comprehensive set of identifiers from the [@unitedstates
project](https://github.com/unitedstates/congress-legislators) is available for
incumbents and winners (GovTrack, ICPSR, MapLight, Open Secrets, WikiData, and
Google Knowledge Graph entity IDs). Further details are in the codebook, which
now gives the source of variables. Our approach was to join the datasets on
`office`, `state`, `district`, and a normalizing transformation of `candidate`,
which remains in the data as `candidate_normalized`. (This is a single word
from `candidate`, usually the last name, in lowercase.)

There are two new
files in the release. We're providing the returns in [Feather
format](https://github.com/wesm/feather) as well as CSV, and including a
supplementary table of variable-value frequencies.


## 2018-03-29

This release adds returns from ten new states; geographic identifiers; and
improvements from ongoing work on data quality. The new returns are from
Alabama, Hawaii, Massachusetts, Minnesota, North Carolina, Oklahoma, Rhode
Island, South Carolina, Virginia, and Wisconsin. This brings coverage to 19
states and the District of Columbia.

County-level geographic variables are now
available as `county_name`, `county_fips`, `county_ansi`, `county_lat`, and
`county_long`. We added these variables by merging in `jurisdiction` FIPS codes
from the [2016 Election Administration and Voting
Survey](https://www.eac.gov/research-and-data/datasets-codebooks-and-surveys)
(EAVS) by `jurisdiction` name, and then joining the returns by FIPS code with
the Census Bureau's [2017 gazetteer files](https://www.census.gov/geo/maps-
data/data/gazetteer2017.html). In states where the administrative jurisdiction
is the county (or equivalent), `jurisdiction` and `county_name` are roughly the
same but differ in source: `jurisdiction` is from the returns as released by
the county, and `county_name` is from the gazetteer. Where local governments
administer elections, the new geographic variables describe the county that
contains the `jurisdiction`. They are not yet available for Alaska.

We
continue to normalize the data across states and jurisdictions. Expect changes
throughout the data, but particularly for down-ballot races, in `candidate`,
`office`, `district`, `mode`, `writein`, and `party`.


## 2018-03-11

This initial release covers ten jurisdictions: Alaska, Colorado, Connecticut,
the District of Columbia, Idaho, Louisiana, New Mexico, North Dakota,
Tennessee, and Wyoming. Returns for the remaining states are forthcoming.

