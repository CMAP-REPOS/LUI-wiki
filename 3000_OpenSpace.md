# Open Space (3000 series)

**NOTE 1:** A large water body is coded the same as part of the
surrounding open space unless it is a *huge* water body like Fox Lake
and is a separate parcel. **NOTE 2:** Most frequently **3100 Open Space
Recreation** will be owned by a municipality or a park district and
**3300 Open Space Conservation** will be owned by a forest preserve
district or the Illinois Department of Natural Resources (IDNR). One
notable exception to this in the City of Chicago are small parcels
mostly in residential neighborhoods which are owned by NeighborSpace".
This is a nonprofit organization whose mission is to acquire and
preserve the community-based management of small parks, gardens, natural
areas, river edges, and scenic landscapes in Chicago. These should be
coded **3100** with a private owner except for those that are very
obviously conservation-focused, such as along a waterway with no sign of
a recreation function that would be coded **3300** with private owner.

Open Space, Primarily Recreation (3100)
---------------------------------------

**Definition:** Recreational open space with greater than 50% combined
impervious surface and manicured turf. Botanical gardens such as Chicago
Botanic Gardens and conservatories such as Garfield Park Conservatory
and Lincoln Park Conservatory are included in this category. Beaches are
also included in this category. Includes code for management agency type
such as municipality, county, state, etc.

**Discussion:** Typically 3100 Open Space Recreation parcels will be
owned by a municipality or park district. However, many local
communities have very active conservation programs, and will have a
number of parcels that qualify instead as 3300 (OS Conservation). Things
to consider when determining whether a parcel owned by a local agency
qualifies as 3100, 3300 or something else:

-   Is the intended use of the site more "active" (picnic, ball field,
    open lawn, boating, fishing; all 3100-style activities) or "passive"
    (hiking, nature study)?
-   Check to see if the property includes a dedicated nature preserve
    (automatic 3300).
-   Some communities have a Park District (a separate taxing body, so
    they will be identified differently in the TAXNAME field than the
    city/village); other communities just have a "Parks and Recreation
    Department" that is a part of the village, so parks in those
    situations are village-owned and not park district-owned. For those
    towns that have park districts, it's much easier to identify
    "natural-state" properties and assign the 3300 OS Conservation code.
    In either case, look on the town website or park district website
    for information telling you this is a designated conservation area
    to code it as Open Space Conservation.
-   When there is no park district and you are looking at a
    natural-state parcel that is owned by the municipality, then it is
    possible that the land is just vacant or set aside for flood
    control. Check the village website for a "parks and recreation"
    department and see if they identify parks; if there is a listing of
    a park for that property, then you can code it open space.
    Otherwise, it could be coded:
    -   **1151 Residential Common**, if it appears to serve as
        stormwater management in a residential setting
    -   **1565 Stormwater Management**, if it appears to serve as
        stormwater management/flood control in a non-residential setting
    -   **4140 Vacant Other**, if there is no apparent function

**Examples:**

**Q&A:**

-   *Q: How do I code horse stables or what may be called an equestrian
    center owned by a forest preserve district or owned by a park
    district?*
    -   **A:** In such a case, we will maintain the original rule of the
        default code based on owner. So such a facility owned by a
        forest preserve district would have the **3300** code and if
        owned by a park district, the **3100** code.
-   *Q: How do I code a recreation building with tennis courts and/or
    outdoor pool that is in a separate parcel and owned by a homeowners
    association?*
    -   **A:** Since this is owned by an HOA, code it **1151 Common Open
        Space**.
-   *Q: How do I code a parcel owned by a park district that only has a
    building on it that is a fitness center along with parking. There is
    no grass, park, tennis courts, etc. on this parcel.*
    -   **A:** Since there is only a building for indoor fitness
        activities and parking in this parcel and no "open space", code
        it **1240 Cultural/Entertainment**.
-   *Q: I know that a forest preserve district owner typically means
    that a parcel will be coded 3300 Open Space Conservation, but what
    about a parcel with such an owner that ONLY has a baseball field on
    it?*
    -   **A:** You're right in that if you have an owner that is a
        forest preserve district you will almost always code the parcel
        as 3300 Open Space Conservation. You must build a strong case to
        code that parcel something other than this. In a case where the
        parcel ONLY has a definite recreational activity on it, you may
        code it 3100 Open Space Recreation. Be sure to also identify
        "county" in the OS\_MGMT field.
-   *Q: How do I code a parcel owned by a park district that has a
    building with park district offices and/or maintenance facilities?
    No recreation areas or facilities are in this parcel.*
    -   **A:** Since no recreation is happening on this parcel and the
        owner is a government entity, code it **1330 Government
        Administration and Services**.
-   *Q: How do I code a small parcel in a downtown area owned by a
    municipality that does not have turf, but instead has a fountain,
    sidewalks, benches, flowers/bushes and is intended for people to
    relax and enjoy that area?*
    -   **A:** Code this **3100 Open Space, Recreation**.
-   *Q: How do I code a community garden where people can rent a plot
    and have a garden for themselves?*
    -   **A:** Code this **3100 Open Space Recreation** and instead of
        Agriculture because people are doing this more as a "hobby" and
        not as their main livelihood as would more often be the case
        with the Agriculture code.
-   *Q: Where do we draw the line between Common Open Space in a
    Residential Development (1151) and Open Space, Primarily Recreation
    (3100)? Grande Park is a massive residential development surrounding
    a very large park and school in Plainfield. I’ve coded the school as
    K-12 Educational Facilities, but am wondering what to do about the
    park land. It’s all owned by the local park district; should the
    park be regular recreational open space, or should it be common open
    space since it’s technically within a residential development? What
    about the trail system (also in parcels owned by the park
    district)?*
    -   **A:** The rule of thumb is to follow the parcel owner. Even
        though land is by a housing development, if it’s owned by a park
        district and looks like it could be used for recreation as open
        space then code it **3100 Open Opace Recreation**. This applies
        to the trail system parcels owned by the park district as well.
-   *Q: How do I code parcels owned by Chicago Park District that are
    currently wooded? Information from the park district is that there
    is a park planned here but not yet built.*
    -   **A:** Since there is no park here yet, code this **4140 Vacant
        Other**.
-   *Q: The photo below is a small portion of two large mostly wooded
    areas on both sides of W Francis Rd that make up one parcel owned by
    the Joliet Park District. On the land to the south of the road are
    buildings for Trinity Services. Research shows that this
    organization provides services for people with disabilities, that
    the buildings include a school, and also include a long-term care
    facility. Census block data says the Total Population is 46; Pop\_GQ
    (Group Quarters population) is 46 and the I\_NURS (Nursing Home
    population) is 46. How do I code this since it is on park district
    owned land and there's a school and a long-term care facility?*
    -   **A:** We're going to use the concept of coding to the more
        active land use. Even though this parcel is owned by a park
        district, the more active land use in this case is that of
        Trinity Services which appears to be a school AND a long-term
        care facility. Because of this, let's use the code **1370 Other
        Institutional**.
        <img src="1370_3.PNG" title="fig:1370_3.PNG" width="400" alt="1370_3.PNG" />

Golf Course (3200)
------------------

**Definition:** Public golf courses, country clubs and driving ranges;
including associated buildings and parking. Includes code for management
agency type.

**Discussion:**

**Examples:**

**Q&A:**

-   *Q: How do I code a 9-hole putting green owned by a homeowners
    association and in a separate parcel?*
    -   **A:** Code this as **1151 Common Open Space**. This is because
        it is owned by an HOA. In order to better automate parcel-based
        landuse in the future, we are putting more emphasis than before
        on owner.

Open Space, Primarily Conservation (3300)
-----------------------------------------

**Definition:** Open space in a natural state (less than 50% combined
impervious surface/manicured turf); includes public land (federal and
state parks and conservation areas, county forest preserves, as well as
local parks that are primarily in a natural state), state-dedicated
nature preserves (regardless of ownership status), and privately-run
conservation facilities. Campgrounds within these facilities are
included as part of the preserve. Includes code for management agency
type.

**Discussion:** See the Discussion section under **3100 Open Space,
Recreation** regarding "natural-state" properties owned by
municipalities and local park districts

Sometimes parts of a forest preserve will have parking lots, picnic
areas, trails for hiking, biking and/or cross country skiing, and even a
small marina if it is on a large lake or river. Even though these could
be considered recreational activities, continue to code these parcels as
**3300** because they are owned by a forest preserve district. A parcel
owned by the forest preserve district with ONLY a ball field on it, for
example, could be coded as **3100**. **Examples:** **Forest Preserve may
have trails on them** Below is Hadley Valley Preserve in Will County.
Even though this forest preserve does have a trail circling it, code it
**3300** because it is owned by a forest preserve district and is a
large natural area that may include forest, wetlands, and/or prairie.
Save the Trail code for true linear parcels that contain a trail.
<img src="3300_2.PNG" title="fig:3300_2.PNG" width="400" alt="3300_2.PNG" />
**Q&A:**

-   *Q: How do I code horse stables or what may be called an equestrian
    center owned by a forest preserve district or owned by a park
    district?*
    -   **A:** In such a case, we will maintain the original rule of the
        default code based on owner. So such a facility owned by a
        forest preserve district would have the **3300** code and if
        owned by a park district, the **3100** code.
-   *Q: How do I code a parcel owned by a forest preserve district or
    the IDNR that appears to be a cultivated farm field?*
    -   **A:** Code this as **3300 Open space, conservation**.
-   *Q: I have found a few parcels that are owned by a park district or
    municipality and from all that I've been able to see on the aerial
    and learn about this area from the Internet, it is solely
    conservation open space with no recreation areas in the parcel. May
    I code it as 3300 Open Space Conservation even though usually such
    an owner would mean that it would be coded 3100 Open Space
    Recreation?*
    -   **A:** You are right to assume the code 3100 Open Space
        Recreation if open space land is owned by a park district or
        municipality. However, some municipalities and park districts do
        own limited areas of conservation open space. If you have found
        strong evidence that this is the case, then you may code the
        parcel as 3300 Open Space Conservation. Be sure to fill in the
        OS\_MGMT field.
-   *Q: I have found several parcels owned by a municipality that appear
    to be wetlands and a stream corridor near and between housing
    developments. How do I code these parcels?*
    -   **A:** This does sound like a conservation use of the land. In
        this case it is important to determine if the municipality that
        owns the parcels also has a park district. If the county says
        that the park district of the municipality is the owner, then
        see what it says on their web site and most likely this will be
        coded 3300. If the municipality has a park district but there is
        NO mention of this area on their website, then code the parcels
        residential common because that wetlands and stream corridor is
        there essentially as part of that housing development. If the
        municipality does NOT have a park district and that function of
        open space recreation and/or conservation is solely a department
        within the municipality rather than a separate park district,
        then you could build a case for coding it 3300.
-   *Q: I have found a parcel in DuPage with a house on it and a person
    as owner. The county use code is open space. There are adjoining
    parcels with the same owner and zero land use value and no
    structures on them that are also coded by the county as land use
    open space. How do I code these parcels?*
    -   **A:** Most likely this individual has negotiated a conservation
        easement with the county or made arrangements to deed the
        property to the county after their death to be used for
        conservation purposes. Code the parcel with the house on it as
        Residential, Single Family with one detached house on it. Code
        the other parcels as 3300 Conservation Open Space with a private
        owner.
-   *Q: The photo below is of Events at Independence Grove, owned by
    Lake County Forest Preserve District. The parcels include venues
    which can be rented for special events and weddings, a cafe, beach,
    native garden, trails, etc. How should this be coded?*
    -   **A:** If the "event" spaces were in their own isolated parcel,
        then Cultural/Entertainment might be an appropriate alternative
        code, but besides the event venues, the same parcel also
        contains water, woods, and trails which are more associated with
        the conservation function of a forest preserve. We want to keep
        forest preserve district owned land intact under **3300** unless
        there is a compelling reason to assign a different code. In this
        case, there is not so code it **3300**.
        <img src="3300_1.PNG" title="fig:3300_1.PNG" width="350" alt="3300_1.PNG" />

<!-- -->

-   *Q: The Calumet Memorial Park District in Calumet City and the Cook
    County Forest Preserve District own an intermingled set of parcels
    north east of Sand Ridge Nature Preserve and just north of Thornton
    Fractional North High School. There are no recreational facilities
    on this land; it is a mixture of trees and prairie. The photo below
    shows the Forest Preserve parcels in purple and the Park District
    parcels in yellow. There is no mention of this land on the park
    district website, nor can I find anything on the forest preserve
    district site. How should these be coded?*
    -   **A:** Since this appears to be conservation land, code all
        parcels **3300**. Despite these parcels being intermingled,
        stick with the owner type to dictate the OS OWNER field so those
        owned by the FPD would get a CNTY owner type and those owned by
        the park district would get a MUNI owner type. Any other
        parcels, not owned by either, could be coded vacant.
        <img src="3300_3.PNG" title="fig:3300_3.PNG" width="300" alt="3300_3.PNG" />
        <img src="3300_4.PNG" title="fig:3300_4.PNG" width="275" alt="3300_4.PNG" />

Non-Public Open Space (3400)
----------------------------

**Definition:** Generally, this category is reserved for those
activities which are considered “low-impact” outdoor recreation
occurring on land that is mostly in a natural state, but is not
protected through public ownership nor dedication as a Nature Preserve.
Including but not limited to hunting clubs, scout camps, and private
campgrounds.

**Discussion:**

**Examples:** Aside from the short list in the definition, other types
of places that can fall in this category include:

-   A "not-for-profit organization which provides therapeutic horseback
    riding to children and adults with disabilities," where the land is
    virtually all open space. A little over half is forested, while the
    other half is more manicured for equestrian activities.
-   A paintball facility whose setting is mostly natural.

**Q&A:**

-   *Q: In Northbrook on the Allstate Corporate Campus are a couple of
    parcels that contain 2 baseball fields, a network of walking paths
    and a pond. Would this be considered Non-Public Open Space?*
    -   **A:** No, since this is part of the Allstate Corporate Campus,
        code it **1220 Office** as you do the rest of that corporate
        campus. This does meet the definition for **3400**.

Trail or Greenway (3500)
------------------------

**Definition:** Right-of-way maintained for the purposes of recreational
activities. Do not include code for management agency type.

**Discussion:** Because of the way the coding models are set up, a
management agency code will get written into the parcel. Don't worry
about this, as they'll get erased during post-processing. Typically
these will be linear parcels that contain a trail. A large park or
forest preserve parcel that happens to also contain a trail should be
coded for the park or preserve, not for the trail. See Example with
photo above under **3300**.

**Examples:**

**Q&A:**

-   *Q: How about a situation in which a utility ROW also has a bicycle
    path on it? Which do I code, for the utility ROW or for the bike
    path?*
    -   **A:** The parcel owner sways how the parcel will be coded. In
        this situation, code **1561 Utility Right-of-Way** even though
        there is also a bike path on the parcel.
-   *Q: Below is a photo of parking owned by City of Joliet. The only
    other city-owned parcels nearby are for Old Plank Road Trail. It
    appears this is parking for those you want to use the trail. May I
    also code it 3500 even though it is not a linear parcel?*
    -   **A:** Yes, definitely. Although the parcel is not linear, the
        sole function is to provide parking for people who want to make
        use of the trail and need to drive to access it. Also code it
        **3500 Trail or
        Greenway**.<img src="3500_1.PNG" title="fig:3500_1.PNG" width="150" alt="3500_1.PNG" />

---

*Return to [A field guide to Land Use Inventory classifications](./README.md)*
