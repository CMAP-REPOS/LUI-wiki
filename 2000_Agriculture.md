# Agricultural Land (2000 series)

Agricultural Land (2000)
------------------------

**Definition:** Land identified in county parcel data as agricultural,
where the parcel is dominated by: row crops, field crops & fallow field
farms & pasture, horse, dairy, livestock, and mixed, including dairy and
other livestock agricultural processing. Also includes land identified
in county parcel data as having a developed land use where, according to
corresponding aerial photography, the land is still in agricultural use;
in those instances, the land is coded as Agriculture, with the planned
land use (Residential, Commercial, Industrial, Other) identified in the
PLATTED modifier.

**Discussion:** While the previous inventories tried to split out the
"farmhouses" from the surrounding agricultural land, in this version
these properties are counted as Agricultural, but with (where
applicable) a RES\_UNIT count of "1" applied to each parcel where,
according to Assessor data, a house is present. In all counties except
Cook, this determination is made during the pre-production phase and is
based on the county classification code, some times used in conjunction
with property value data.

With the exception of Cook County, the initial coding of Agricultural
land is done through an automated procedure where all county-classified
Agricultural parcels are evaluated against the USDA's Cropland Data
Layer (CDL), which is a 30-meter raster-based landcover dataset which
emphasizes the classification of agricultural cover types. Through this
procedure, any Ag parcel that has at least 25% crop/meadow/orchard land
is automatically assigned the 2000 code. These parcels are then
re-checked to ensure that there aren't developed land uses (based on
high Assessor improvement values), utility rights-of-way (query
landowner for "Commonwealth Edison" or "Nicor"), and aren't involved in
mineral extraction activities (review 2005 extraction polygons). Cook
County parcels will be inspected/coded individually, since there are so
few.

Remaining parcels not caught during the automated procedure include:

-   County-classified AG parcels which are primarily woodlots or
    wetlands; these should receive a code of **4100
    (Vacant/Undeveloped)**.
-   Parcels recently subdivided for a developed land use, but
    construction activities haven't started yet and the actual property
    is still in agriculture (according to 2010 photography); these
    properties should recieve a code of **2000 (Agriculture)**, with the
    "Platted" field updated with the appropriate code.

Parcels on which there are **stables and pastures for horses** are often
classified as agriculture or farm by counties. This does not mean we
will necessarily code them as agriculture for land use. Below are the
three usual situations encountered and the Land Use codes that will be
used: 1. In rural residential areas, on land owned by the same homeowner
you may find horse stables and fenced areas or pastures for horses for
private use only. Code these with the appropriate the **Residential**
code for the type of housing and residential units depending on whether
the housing is on the same parcel or is on an adjoining parcel with the
same owner.

2\. If you encounter a parcel in which you find a riding center with
stables, riding rings, riding exhibitions, trails, etc. where people
ride horses as a private club or a public operation, code this
**1240(Cultural/Entertainment)**.

3\. If you determine that horse stables and/or pasture is a commercial
operation for raising, sale, boarding and/or breeding of horses, rather
than one of the two above cases, you may code this **2000 Agriculture**
and if applicable, put a one in the RES\_UNIT field.

**Nurseries and greenhouses** are coded based on the type of business
running the operation. See Examples 1 & 2 below.

**Examples:** **Example 1: Nursery coded as Urban Mix (not Ag)** In this
case, the nursery is a business called “Prestige Nursery Garden Center”,
which according to the D&B listing is a “Landscape Architectural
Service” (NAICS-6 code 541320) which is lumped into the NAICS-2 category
54: Professional, Scientific and Technical Services. This is the kind of
operation more consistent with an Urban Mix type of business. In this
instance, the AG parcel would get coded Urban Mix.
![](2000_1.PNG "fig:2000_1.PNG") **Example 2: Nursery coded as
Agriculture** On the other hand, large-scale nursery/greenhouse
operations would be coded Agriculture; for the most part these will have
NAICS-2 codes of “11” (Agriculture, Forestry, Fishing and Hunting).
Example \#2 below is a parcel with a NAICS-6 of 111421: Nursery and Tree
Production. ![](2000_2.PNG "fig:2000_2.PNG") **Example 3: Agriculture
with a Platted Modifier** In some cases, the 2010 aerial may show a
parcel as 25% or more still as crop/meadow/orchard even though the
parcel layer shows it as platted for a developed land use (Residential,
Commercial, Industrial, Other). Example \#3 below is an area where the
parcels that are 25% or more agriculture would get coded as 2000 and
those that are not would be coded vacant. The AG parcels would also need
a Platted Modifier which could be obtained easily if the county land use
has identified it as residential, commercial, etc. If the county codes
it as unknown, then use the NDD layer to see the intended future use for
an area that is currently agriculture or use the TaxName or other
information to be confident in the type of future development that it
will become. If you can find no information on intended use, then use
Other for the Platted Modifier.
<img src="2000_3.PNG" title="fig:2000_3.PNG" width="400" alt="2000_3.PNG" />
The following is a different situation in which a Platted Modifier is
appropriate to use. The parcel is owned by Elmhurst Cemetery Company and
is Exempt by the county. Only a tiny part of the northern most part of
the parcel clips the actual cemetery. The rest is mostly cultivated farm
field. Since the "active" land use by the cemetery is much too small,
this will be coded **2000 Agriculture**, but since it is classed as
Exempt by the county, we will add the Platted Modifier of "O" for Other.
<img src="2000_4.PNG" title="fig:2000_4.PNG" width="300" alt="2000_4.PNG" />
**Example 4: Rural Residential** Residential Land Use in a rural setting
may sometimes be classified as agriculture or farm by a county. *This
does not mean that we will code such parcels as agriculture.* For Land
Use coding, **2000 (Agriculture)** will be reserved for land with crops
or grazing of livestock as a commercial operation. This means someone's
large garden with no evidence this is a commercial business for them is
not coded agriculture even though the county may classify the land as
farm. Any parcel adjoining a house with the same owner must be evaluated
as to whether it meets the Agriculture Land Use criteria of land with
crops or grazing for livestock as a commercial business no matter what
classification the county assigns to it. Also, a house in a rural
setting on a large parcel with a private barn and horses would be coded
**Residential** unless there is evidence that it is a commercial
equestrian operation meaning they are commercially selling some
equestrian-related product or service. Below are two examples of **Rural
Residential** which would be coded **Residential** Land Use even though
the county may classify such land as agriculture or farm. In the first
photo, this Rural Residence is on 3 parcels. The small one on the far
right is the house. The other two are coded by the county as farm, but
there is no evidence of any commercial crop or grazing so this is coded
**1111 (Single-Family Detached)** with one residential unit in the
parcel containing the house and zero in the other two parcels, all of
which have the same owner.
<img src="1111_4.PNG" title="fig:1111_4.PNG" width="700" alt="1111_4.PNG" />
In the second photo, the house is in one parcel and the private horse
stables are in an adjoining parcel with the same owner. This also will
be coded as **Residential**.
<img src="1111_3.PNG" title="fig:1111_3.PNG" width="500" alt="1111_3.PNG" />

**Q&A:**

-   *Q: I'm looking at a parcel with LU pass 1 as AG. It's part of a
    nursery....There are many nursery trees and bushes on this parcel
    along with a few buildings and bins of rock material. Do I code this
    as Ag ..... or as Urban Mix as I did the other two parcels for this
    nursery which were LU pass 1 of COM?*
    -   **A:** These need to be handled on a case-by-case basis,
        depending on the type of operation. Refer to Examples 1 & 2
        above.
-   *Q: How do I code horse stables owned by a forest preserve district;
    as agricultural or as open space, conservation?*
    -   **A:** Code these as **3300 Open Space, Conservation**.
-   *Q: How do I code a parcel owned by a forest preserve district that
    appears to be a cultivated farm field?*
    -   **A:** Code this as **3300 Open Space, Conservation**.
-   *Q: How do I code a parcel identified as AG by the county that has a
    farm house on it?*
    -   **A:** If the parcel identified by the county as agriculture
        that has a house on it is 1 acre or less (43,560 sq ft) then
        code it **1111 Single-family detached**. If the parcel is larger
        than that and agriculture is the appropriate code, then code it
        **2000 Agriculture**. In both cases, make sure that there is a
        "1" in the residential units field.
-   *Q: How do I code a relatively small parcel identified by the county
    as AG which is next to a residential parcel with the same owner.
    There's a single family detached house on the residential parcel.
    The AG parcel has nothing on it that in any way would suggest
    agriculture; nothing that looks like it's used for horses or a large
    garden or anything else agricultural.*
    -   **A:** Code this as **1111 Single family detached** with "0" in
        the residential units field.
-   *Q: How do I code a community garden where people can rent a plot
    and have a garden for themselves?*
    -   **A:** Code this **3100 Open Space, Recreation** and instead of
        Agriculture because people are doing this more as a "hobby" and
        not as their main livelihood as would more often be the case
        with the Agriculture code.
-   *Q: Some of the parcels that were coded Ag through automation have a
    significant portion which is actually Mineral Extraction. Should
    they be left as Ag or changed?*
    -   **A:** The original automated procedures had a threshold of 25%,
        meaning 25% of the landcover pixels falling in the parcel had to
        have an agricultural classification. Since Mineral Extraction is
        considered a "developed" land use, it carries greater land use
        weight, and would trump the developed land use. For these mixed
        parcels, recode to Mineral Extraction if at least 25% of the
        parcel is covered by this activity (including pits, ponds and
        staging areas).
-   ''Q: How do I code an equestrian center that is mostly used for
    boarding horses, riding instruction, and competitions?
    -   **A:** Code this as **1240 Cultural Entertainment**.
-   ''Q: A parcel coded as AG by the county has a house on it and
    buildings and fencing determined by internet searches to be for dog
    breeding. There is no DnB point indicating a business and no
    evidence of a commercial sign on the property using
    GoogleStreetView. Do I code this as Agriculture with 1 for the
    residential units field?
    -   **A:** Even though the county classed this as Ag, dog breeding
        really does not fit our Agriculture definition. Since there is
        also no evidence of a commercial business, code this as *' 1111
        Single-Family Detached*' with 1 res unit.
-   *Q: How do I code a series of parcels owned by IDOT that appear to
    form what will be a future expressway? Some parcels appear to be
    vacant and others currently have crops on them.*
    -   **A:** Code the vacant parcels **4140 Other Vacant** and code
        the ones with at least 25% agricultural activity as **2000
        Agriculture** and put a **O** in the PLATTED Modifier field for
        the Ag ones.
-   *Q: Governors State University owns several parcels that are being
    farmed. They have no agriculture-related program. How should these
    be coded?*
    -   **A:** If a parcel is entirely being farmed, then code it **2000
        Agricultural**. If only a portion of the university-owned parcel
        is being farmed, then code it **1322 Post Secondary Educational
        Institution**.

*Return to [A field guide to Land Use Inventory classifications](./README.md)*
