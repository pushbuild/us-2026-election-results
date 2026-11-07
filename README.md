# US 2026 general election results, by state and county

Unofficial results of the November 3, 2026 US general election as each state's election office published them, one CSV per
state in `data/`: every contest the state's results feed carries (U.S. Senate, U.S. House, governor and other statewide
offices, legislature, ballot measures and, where the feed has them, local contests), statewide and by county.

**Live API:** query these results (and every later update) by state, contest or county at
https://pushbuild.com/apis/election-night-results.html (free key, sign up at https://pushbuild.com/apis/app/).

**Results as of November 6, 2026, 11:32 PM ET.** Counting continues after election night and states certify weeks later; this repository will be
refreshed after certification. Until then these are unofficial and can change.

| column | meaning |
|---|---|
| state | two-letter state code |
| level | `state` (statewide total) or `county` |
| county | county name (parish in Louisiana) for county rows |
| contest | contest name as the state publishes it |
| candidate | candidate or ballot option |
| party | party as the state publishes it, when it does |
| votes | votes for this candidate in this unit |
| pct | share of the contest's votes in this unit, in percent |
| contestTotalVotes | all votes cast in the contest in this unit |
| precinctsReporting, precinctsTotal | precincts counted / expected, when the state reports them |
| source | the official results source |
| sourceUrl | where the figures were read |
| sourceUpdatedAt | the source's own timestamp for the count, when it gives one |
| fetchedAt | when Pushbuild read it (UTC) |

| state | file | statewide rows | county rows | official source |
|---|---|---|---|---|
| Alaska | [ak.csv](data/ak.csv) | 174 | 4,928 | Alaska Division of Elections |
| Alabama | [al.csv](data/al.csv) | 293 | 0 | Alabama Secretary of State |
| Arkansas | [ar.csv](data/ar.csv) | 2,377 | 4,602 | Arkansas Secretary of State (Tally ENR) |
| Arizona | [az.csv](data/az.csv) | 415 | 1,608 | Arizona Secretary of State |
| California | [ca.csv](data/ca.csv) | 352 | 0 | California Secretary of State |
| Colorado | [co.csv](data/co.csv) | 646 | 5,792 | Colorado election offices via Clarity ENR |
| Connecticut | [ct.csv](data/ct.csv) | 878 | 6,530 | Connecticut Secretary of the State |
| Delaware | [de.csv](data/de.csv) | 124 | 0 | Delaware Department of Elections |
| Florida | [fl.csv](data/fl.csv) | 406 | 3,063 | Florida Division of Elections |
| Georgia | [ga.csv](data/ga.csv) | 457 | 5,817 | Georgia Secretary of State |
| Iowa | [ia.csv](data/ia.csv) | 655 | 5,355 | Iowa election offices via Clarity ENR |
| Idaho | [id.csv](data/id.csv) | 292 | 2,289 | Idaho Secretary of State |
| Illinois | [il.csv](data/il.csv) | 4 | 0 | Candidate list (Wikipedia race summary); official results not posted yet |
| Indiana | [in.csv](data/in.csv) | 7,407 | 9,114 | Indiana Election Division |
| Kansas | [ks.csv](data/ks.csv) | 3 | 194 | Candidate list (Wikipedia race summary); official results not posted yet, Harvey County Clarity ENR, Miami County Clarity ENR |
| Louisiana | [la.csv](data/la.csv) | 2,498 | 3,162 | Louisiana Secretary of State |
| Massachusetts | [ma.csv](data/ma.csv) | 4 | 0 | Candidate list (Wikipedia race summary); official results not posted yet |
| Maryland | [md.csv](data/md.csv) | 354 | 1,329 | Maryland State Board of Elections |
| Michigan | [mi.csv](data/mi.csv) | 0 | 386 | Ottawa County Clarity ENR, Roscommon County Clarity ENR |
| Minnesota | [mn.csv](data/mn.csv) | 648 | 8,285 | Minnesota Secretary of State |
| Missouri | [mo.csv](data/mo.csv) | 35 | 2,064 | Missouri Secretary of State |
| North Carolina | [nc.csv](data/nc.csv) | 660 | 5,614 | NC State Board of Elections |
| Nebraska | [ne.csv](data/ne.csv) | 625 | 0 | Nebraska Secretary of State |
| New Jersey | [nj.csv](data/nj.csv) | 0 | 1,316 | Cumberland County Clarity ENR, Essex County Clarity ENR, Passaic County Clarity ENR, Somerset County Clarity ENR |
| New Mexico | [nm.csv](data/nm.csv) | 362 | 0 | New Mexico Secretary of State |
| Nevada | [nv.csv](data/nv.csv) | 4 | 0 | Candidate list (Wikipedia race summary); official results not posted yet |
| New York | [ny.csv](data/ny.csv) | 2 | 0 | Candidate list (Wikipedia race summary); official results not posted yet |
| Ohio | [oh.csv](data/oh.csv) | 340 | 3,360 | Ohio Secretary of State |
| Oklahoma | [ok.csv](data/ok.csv) | 229 | 0 | Candidate list (Wikipedia race summary); official results not posted yet, Oklahoma State Election Board |
| Pennsylvania | [pa.csv](data/pa.csv) | 37 | 369 | Pennsylvania Department of State |
| Rhode Island | [ri.csv](data/ri.csv) | 1,277 | 2,796 | Rhode Island Secretary of State |
| South Carolina | [sc.csv](data/sc.csv) | 531 | 2,659 | South Carolina election offices via Clarity ENR |
| South Dakota | [sd.csv](data/sd.csv) | 232 | 0 | South Dakota Secretary of State |
| Texas | [tx.csv](data/tx.csv) | 917 | 17,568 | Texas Secretary of State |
| Utah | [ut.csv](data/ut.csv) | 290 | 1,187 | Utah Secretary of State |
| Virginia | [va.csv](data/va.csv) | 114 | 1,877 | Virginia  Secretary of State |
| Vermont | [vt.csv](data/vt.csv) | 540 | 0 | Vermont Secretary of State |
| Washington | [wa.csv](data/wa.csv) | 468 | 1,810 | Washington Secretary of State |
| Wisconsin | [wi.csv](data/wi.csv) | 2 | 142 | Candidate list (Wikipedia race summary); official results not posted yet, Dane County Clerk (unofficial), Milwaukee County Election Commission (unofficial) |
| Wyoming | [wy.csv](data/wy.csv) | 2 | 0 | Candidate list (Wikipedia race summary); official results not posted yet |

States not listed did not publish a machine-readable results feed we could read. All figures come from the official state
sources named above; collection is automated, so check a figure against the state's own site before relying on it.
Pushbuild is not affiliated with any election office.

The same data, live and filterable, is available as an API: [Election Night Results API](https://pushbuild.com/apis/election-night-results.html) (endpoint `https://api.pushbuild.com/election-night-results/run`),
and as pages at [pushbuild.com/apis/elections](https://pushbuild.com/apis/elections/).

License: CC0 1.0.
