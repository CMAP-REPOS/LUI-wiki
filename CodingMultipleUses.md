---
title: Coding Multiple Uses
nav_order: 12
---

# Coding Multiple Uses
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

* TOC
{:toc}
---

The 2015 Inventory is our first attempt (since switching to a parcel
base) at assigning multiple uses to parcels. The last two inventories
had a MODIFIER flag that allowed for specific multiple-use combinations,
but was only put to use for combinations of church & school on the same
parcel. For 2015 we are adding a new field, LANDUSE2, to account for
multiple uses on parcels. Because some parcels have more than two
significant uses, this field is not limited to a single additional
use—it will allow for up to four additional uses, which will be written
into the field with just the four-digit land use codes with a semicolon
delimiter (the field is formatted Text with 20 characters assigned).
Because of this formatting the land use code domain (e.g. displaying
1111 as “Residential, Single-Family Detached”) can’t be applied to this
field…you’ll only see the code.


## When to code additional land uses

Allowing for additional land use codes does not mean every single
activity on a parcel needs to be reported; this is meant for
**significant** activity, either where there are two or more uses which
equally occupy the parcel (or the space within building on the parcel),
or where the smaller use (in terms of area) has an impact in the number
of jobs or households on the parcel. Below are some fairly
straightforward examples…this initial set of instructions doesn’t
anticipate every possible multiple-use instance. Instead, when
encountering a situation that you are not sure of, describe the
situation to [David](mailto:dcclark@cmap.illiinois.gov), who will mull
it over, recommend a course of action, and ask you to update the
**Questions & Recommendations** section below.

***Water Tower Place*** has at least three major uses:

-   Water Tower Place Mall (1211: Shopping Mall, 8 floors),
-   Ritz-Carlton Hotel (1250: Hotel/Motel, 15 floors), and
-   Residential condominiums (1130: Multi-Family Residential, 40 floors)

For 2010 and 2013 the property was assigned a single code for the mall,
on the premise that, while the mall occupies the fewest floors, it
generates the most activity of the three uses. For 2015, this parcel
would keep the 1211 code as the primary land use, but also get “1250”
and “1130” codes assigned to the LANDUSE2 field. Additionally, since one
of the uses is residential, an estimate of the number of residential
units needs to be entered using the RES UNITS Update tool.

***Jackson Park*** is a major Chicago park on the south side with two
parcels that have LANDUSE2 candidates:

-   The Museum of Science and Industry is on the north end of Jackson
    Park and has a significant enough presence to merit a LANDUSE2 of
    Cultural/Entertainment (1240) since it has hundreds of employees.
    For consistency with earlier inventories, the primary LU code should
    remain Recreational Open Space.
-   The next parcel to the south is the Jackson Park Golf Course, coded
    (naturally) 3200 Golf, but it includes La Rabida Children’s Hospital
    with a few hundred employees as well, so a LANDUSE2 of 1310 Medical
    Facilities is appropriate here.

***Nursing Home/Independent Living combinations*** Facilities for senior
citizens are expanding to offer more of a “continuum of care” that run
the gamut from independent-living townhomes to full-service nursing
facilities; in the Inventory the former are considered residential
(usually multi-family) while the latter are coded 1310 Medical. This
either/or designation is problematic: coding these as Residential
suggests there is limited employment activity, and doesn’t sync up with
the Census’ reporting of an Institutionalized Group Quarters population
in the area. Coding it as Medical suggests absence of a population that
is free to come and go, which affects travel model estimates. Facilities
which serve as both a nursing home as well as an independent living
community should be coded **1310 Medical** as their primary land use
code. After assigning this primary code, re-select the parcel(s) and run
the Flag Multiple Uses tool to assign **1130 (Multi-Family Res) and/or
1112 (Single-Family Attached, if there are townhomes on the property)**.
A Residential Unit Estimate should also be assigned to the property, for
the independent living units only. We try as much as possible to match
these residential unit estimates to the definitions used by the Census
Bureau, where population living in independent living units are treated
as “households,” while residents of the skilled nursing part of the
facility are counted as Group Quarters population. A residential unit
estimate can come from the 2010 Census Housing Units (HU\_TOT) count (if
it was there prior to 2010); sometimes the number of independent living
units is listed on the facility’s website.

***Hotel & Convention Center*** The Schaumburg Convention Center is an
example of two Commercial uses on the same parcel, since it has not only
the 150,000’ convention space but also 500 hotel rooms. In this instance
the hotel should get the primary code because it has 24/7 activity,
while the convention center is only in use when hosting a convention.


## Which is the Primary land use?

Some guidelines:

1. **What it was coded in the previous inventory:** For
consistency with earlier inventories, priority should be given to
whatever it was coded in 2010/2013 so any over-time analyses don’t flag
a land use change where one didn’t actually happen. Exception: if the
2010/3 code is wrong, it should be changed (which also involves
assigning an error point).

    -   *Note* -- for the church/school combos that were coded Educational with
        a “R” modifier, these can all be selected in a single query and have
        the 1350 (Religious Facilities) code pushed into the LANDUSE2 field.

2. **The more “active” use:** When \#1 (above) doesn’t apply, use the
same logic employed for previous inventories, assigning the more active
use as the primary code is recommended. “Active” in this context means:
how much activity (households, employment) is generated by each of the
uses? Some examples:

    -   Residential hi-rise with street level commercial: while the 1216
        “Urban Mix with Residential Component” covers buildings up to four
        stories high, taller buildings have in the past been coded
        multi-family. Under this new scheme, these buildings would still be
        coded multi-family (1130) but will also get a LANDUSE2 code of 1215
        (Urban Mix) to represent the retail/service component (which, being
        limited to the first floor, is a small fraction of overall
        activity).
    -   On the other hand, a high-rise office building with street-level
        retail does not need a 1215 LANDUSE2 designation, since most office
        buildings host some small amount of retail.


## Using the Flag Multiple Uses tool

Assigning additional uses requires activating the Flag Multiple Uses
tool. This is done after initial coding of the polygon (or assigning
added uses to something that was coded in an earlier inventory). Simply
select the polygon, open the tool, and select additional use (or uses... up
to four maximum), and run tool. In addition to populating the LANDUSE2
field, this tool will also set the value of MODIFIER to “M” (for
“multiple”). If the additional uses had a residential component, use the
RES UNITS Update tool (under Non-Coding Tools) to assign a residential
unit estimate. Note, some uses are not allowed to be secondary uses
since they don’t help characterize the activity of a parcel. These
include:

-   1565 - Stormwater Management
-   3500 - Trail or Greenway
-   4110 - Vacant Residential Land
-   4120 - Vacant Commercial Land
-   4130 - Vacant Industrial Land
-   4140 - Other Vacant
-   5000 - Water
-   9999 - Not Classifiable


## Questions & Recommendations

This section will get updated whenever a multi-use question is asked (&
answered)
