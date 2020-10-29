# Institutional Land Uses (1300 series)

**PLEASE NOTE:** The order presented below implies a sequence for
selection. For example, a hospital within a public university would be
coded \#1310 (Medical and Health Care Facilities). **Also note:** Code
any detention or retention basin areas near institutional buildings with
the same code as the nearby institutional building even if these parcels
are owned by a different organization, such as a government entity.
These institutional buildings could not have been built in that area if
land had not also been set aside for water detention or retention.

Medical Facilities (1310)
-------------------------

**Definition:** Includes hospitals as well as nursing homes and other
long-term care facilities.

**Primary Reference Layer:**

-   *HospitalsNursingHomes.lyr* in Reference folder, which contains:
    -   Long-term care facilities, provided by the IL Dept of Public
        Health;
    -   Hospitals (IDPH);
    -   Stand-alone same day surgical centers and
    -   Polygons from the 2005 Land Use Inventory coded as 1310 MEDICAL
-   *CENBLOCK\_(county)*, Census block feature class with household and
    group quarters data. The field **I\_NURS** lists the number of
    people in that block living in nursing homes (which are considered
    "Institutionalized Group Quarters").

**Discussion:** Since the reference layers for this use are fairly
definite/reliable, and the number of properties for most counties not
too overwhelming, this would be a good use to tackle at once, by going
down the list of long-term care facilities in the county, zooming to and
coding each one as you go. While hospitals are fairly obvious, other
properties that might or might not fall in to this category need a
little explanation.

-   Medical office centers: basically, office buildings which are
    primarily or completely taken up with physicians' offices, etc. If
    they are not directly associated with and adjacent to a hospital,
    these should be coded 1220: Office.
-   Same day surgical centers, also called ambulatory surgical centers,
    provide same-day surgical care, including diagnostic and preventive
    procedures. In some cases you will find them in a building that is
    not on a hospital campus. Also code these as institutional medical
    as you would a hospital.
-   Senior "spectrum" properties: places that offer a wide range of care
    within different portions of the property, with independent living
    (considered multi-family) as well as nursing/long-term care
    facilities. See Q&A below for how to handle these properties.
-   Independent living facilities should be coded 1131: Multi-Family (No
    Commercial Component)

As to the question of where to draw the distinction between nursing
homes and independent living (multi-family) structures (assuming it's
not a "spectrum" development), the reference layers should give a good
clue. If it appears in the Long Term Care reference layer, or if there
is a population listed in the I\_NURS field of the Census Block layer,
then it is most likely a nursing home. **Examples:** Sherman Hospital,
Elgin. ![](1310_1.PNG "fig:1310_1.PNG") Nursing home in Elgin.
Corroborated by the *Long Term Care* reference layer, and by the
presense of a population in the census block living in nursing homes
(I\_NURS &gt; 0). ![](1310_2.PNG "fig:1310_2.PNG") Holmstad Retirement
Community, Batavia. Parcels don't neatly match the building layouts, but
the development's website (found by Googling the name in the TAXNAME
field) provided a map which identified the separate units. 1310
properties include the main building, nursing home and assisted living
structures. ![](1310_3.PNG "fig:1310_3.PNG")

**Q&A:**

-   *Q: Large senior living communities often have several different
    types of housing as part of their community. How do I handle this?*
    -   **A:** If a nursing home component of housing is in such a
        parcel which also includes independent living houses,
        townhouses, and/or apartments, then code the entire parcel as
        medical. If there is a parcel in the senior community that is
        entirely independent living residences, then code that parcel as
        residential single-family detached, attached, or multifamily
        depending on the type of independent housing in that parcel. If
        the parcel is coded as single-family detached or attached, be
        sure to change the residential units number to show how many
        single-family units are in that one parcel.

<!-- -->

-   *Q: How do I code the parcel shown in the photo below. It is a
    senior living community with a majority of townhouses. Dun &
    Bradstreet points show some residences have small home-based
    businesses. There is also a multi-story building which has
    independent-living and assisted-living apartments for seniors in
    which residents contract for needed services to assist them with
    daily life. The census data reference layer shows nothing in the
    I\_NURS field so there is no nursing home in this census block.*
    -   **A:** Since there is nothing in the I\_NURS census data field
        and your research shows there is not a nursing home, then this
        would NOT be coded 1310. While there is a majority of
        townhouses, the additional presence of the apartment building
        would mean **1131 Multi-Family Residential** would be the most
        appropriate code.
        <img src="1131_6.PNG" title="fig:1131_6.PNG" width="400" alt="1131_6.PNG" />

K-12 Educational Facilities (1321)
----------------------------------

**Definition:** Public and non-public schools as identified by the
Illinois State Board of Education. Church/school combinations that share
a common parcel are coded as schools.

**Discussion:** If a school district headquarters is on the same
property as the school, code the entire property as 1321 (K-12 EDU)
unless the HQ is clearly distinguishable on its own parcel (in which
case code that parcel 1330 GOVT). Don’t use the modifier field for this
particular combo.

**Examples:**

**Q&A:**

-   *Q: How do I code a parcel owned by a school district that I
    discover only has school administration offices?*
    -   **A:** This is coded as government, not educational.
-   *Q: A parochial school and the associated church are in the same
    parcel. How do I code this?*
    -   **A:** Following the note at the top of this 1300 Institutional
        section that the order of the 1300 codes implies a sequence for
        selection, you would code this parcel for the school. Also, put
        an "R" in the MODIFIER field to denote that this parcel also has
        a religion land use because the church is on the same parcel as
        the school. HOWEVER, first check the enrollment for the school
        (there is an enrollment field in the K-12 Schools reference
        layer); if a school on church property reports zero enrollment,
        then code the property as 1350 (Religious). Also, please know
        that in some cases the school located on the same parcel as a
        church is not necessarily a parochial school, meaning it is run
        by the church. In Chicago, there are charter schools, a part of
        Chicago International Charter Schools organization, which are
        publicly funded that are operating in buildings that formerly
        were parochial schools and located in the same parcel as the
        church which owns the parcel. With these situations, also code
        for the school and put an "R" in the MODIFIER field to show
        there is also a house of worship on this parcel.
-   *Q: How do I code the parcel in the photo below that is owned by the
    Catholic Bishop of Chicago? This one parcel contains a church, a
    parochial school and also a 4-story commercial building containing a
    commercial theater.*
    -   **A:** Because the owner of this one parcel is the Catholic
        Bishop of Chicago and the parcel does contain a church and
        parochial school we will have to ignore the theater in this case
        and code it **1321 K-12 Educational Facilities** with a modifier
        of 'R'.

<figure>
<img src="1321_1.PNG" title="1321_1.PNG" width="300" alt="1321_1.PNG" /><figcaption aria-hidden="true">1321_1.PNG</figcaption>
</figure>

-   *Q: How do I code a preschool or day care center?*
    -   **A:** If it is owned by a school district or some other
        government entity or nonprofit AND the county use code is
        Exempt, then code it **1321 K-12 Educational Facilities**. If it
        is owned privately, is for-profit, and the county use code is
        Commercial, then code it **1215 Urban Mix**. One caveat to this
        is if the County codes a parcel as Commercial even though it is
        owned by a church, for example, and has a day care center on it,
        put more weight on the County Code of Commercial and code it
        1215 urban mix. Since the county did not code the parcel Exempt
        even though it is owned by a church, likely the church is
        renting out the building or has this as a for-profit arm of the
        church so urban mix will be more the appropriate code.
-   *Q: Below is a photo of a school bus garage and parking on a parcel
    that is owned by a school district. It is not adjacent to any
    school, but rather in an industrial area. How should I code this? Do
    I use an Education code because the parcel is owned by a school
    district or do I use a Transporation code?*
    -   **A:** Even though the parcel is owned by a school district, the
        busses are used to transport students to and from schools and
        not to formally teach them anything in the transport process.
        Because of this, code it **1520 Other Linear Transportation**
        instead of an Education code.

<figure>
<img src="1520_2.PNG" title="1520_2.PNG" width="450" alt="1520_2.PNG" /><figcaption aria-hidden="true">1520_2.PNG</figcaption>
</figure>

Post-Secondary Educational Facilities (1322)
--------------------------------------------

**Definition:** Universities, colleges, community colleges; public, as
well as for-profit and not-for-profit private schools. As identified by
the Illinois Board of Higher Education. Includes satellite campuses,
where applicable.

**Discussion:** The Illinois Board of Higher Education reference layer
will be an important layer to use to identify these educational
facilities. Some private colleges may be quite small. The enrollment
number in that IBHE reference layer will be helpful to check. You can
also look up the school on the [IBHE
website](http://ibheprofiles.ibhe.org/). **Examples:**

**Q&A:**

-   *Q: How do I code a separate parcel that's owned by a college, but
    is clearly apartments for students? Is it multi-family residential
    or is it higher education institutional?*
    -   **A:** In determining the more appropriate land use code, a
        building owned by the college is one criteria. However, it also
        needs to be considered an ON-campus dorm. Count a dorm that is
        OFF-campus as multi-family housing. You can often find a college
        campus map on the school's web site to help you. Also, use the
        census block reference layer to guide you. A census count in the
        NI\_COLL field would indicate a non-institutionalized college
        (college dorm) resident population, which would lend support to
        a code of **1322** for a dorm rather than **1131 Multi-family
        residential.**
-   *Q: How do I code the parcel pictured below? It is owned by
    University of Chicago and the county classifies it as Exempt. 2005
    Land Use coded it as Industrial General. It is located much farther
    south than the main U of C campus and research shows it to be
    University of Chicago Press.*
    -   **A:** This would be coded **1420 Industrial General** once
        again in 2010. Even though it is Exempt by the county and is
        owned by University of Chicago, it is not a property where
        students and professors converge. They print books here.
        <img src="1420_1.PNG" title="fig:1420_1.PNG" width="200" alt="1420_1.PNG" />
        <img src="1420_2.PNG" title="fig:1420_2.PNG" width="200" alt="1420_2.PNG" />

Government Administration and Services (1330)
---------------------------------------------

**Definition:** Includes executive, legislative, and judicial functions;
protective functions (police, fire, civil defense); postal services and
public libraries; public works facilities that are not included in the
1500 (Transportation, Communication, Utilities & Waste) series. Also,
military facilities (including military group housing quarters, military
residences, training bases, arsenals, armories) such as the Great Lakes
Naval Center and Illinois National Guard Centers.

**Discussion:**

**Examples:**

**Q&A:**

-   *Q: How do I code a parcel owned by a school district that I
    discover only has school administration offices?*
    -   **A:** This is coded as **1330 government**, not educational.
-   *Q: How do I code a parcel owned by a park district that has a
    building with park district offices and/or maintenance facilities?
    No recreation areas or facilities are in this parcel.*
    -   **A:** Since no recreation is happening on this parcel and the
        owner is a government entity, code it **1330 Government
        Administration and Services**.
-   *Q: How do I code a small parcel owned by a municipality that
    contains a civil defense siren mounted on a very tall pole?*
    -   **A:** Since this is owned by a municipality and not a
        communications company, code it **1330 Government Administraton
        and Services**.
-   *Q: How do I code a parcel taken up by highway maintenance
    buildings, DOT trucks, and/or salt storage?*
    -   **A:** Code it coded **1520 (Other Linear Trans)**, regardless
        if it's owned by IDOT, a county highway department, or a
        municipality. On the other hand, if this type of facility shares
        a parcel with other municipal functions (i.e. fire station),
        then code it 1330 Govt.
-   ''Q: How do I code a parcel containing a building in which the US
    Post Office is located when the parcel is coded as commercial by the
    county and is owned privately, not by the US Government?
    -   **A:** If the building appears to ONLY contain the US Post
        Office and is not also being used by other tenants, then code it
        **1330 Government**. Sometimes we have found smaller post
        offices in buildings owned privately. However, if the building
        also contains other offices or tenants, then code it **1215
        Urban Mix**.
-   *Q: How do I code a parcel that is owned by the State of Illinois
    that has 2 houses on it that appear to be occupied and used as
    homes, not offices for state employees. The county use code is
    Exempt. Zero in the Residential Units field.*
    -   **A:** The count in the Residential Units field is a guess based
        on other information found in the parcel data during
        pre-processing. In this case, the reason for the zero is because
        of the Exempt status by the county. The State of Illinois owns
        some parcels that continue to have active residences because
        they have bought that land in anticipation of a future
        development project such as an expressway, a bypass, a new
        airport, etc. If you see evidence that the parcel is being used
        as residence, then even though it is owned by State of Illinois,
        code it with the appropriate Residential code and change the
        Residential Units to the correct number.

Prison and Correctional Facilities (1340)
-----------------------------------------

**Definition:** Government establishments primarily engaged in managing
and operating correctional institutions. The facility is generally
designed for the confinement, correction, and rehabilitation of adult
and/or juvenile offenders sentenced by a court.

**Discussion:**

**Examples:**

**Q&A:**

-   *Q: In the photo below are 2 parcels coded as residential by the
    county. This is Fox Valley Adult Transition Center which is a
    facility in which women are transitioned from prison life to regular
    life. the parcel owner is Old Second National Bank of Aurorar,
    Trustee. How should this be coded?*
    -   **A:** Based on the description of Fox Valley Adult Transition
        Center, the choice would be between 1340 Correctional Facility
        and 1370 Other Institutional. In this case, let the Census block
        reference data be your guide. If that census block has a
        significant incarcerated population (the I\_CORR field, meaning
        Institutionalized Group Quarters, Correctional), then go with
        **1340 Prison/Correctional**. If the census shows that
        population in some other group quarters situation, either
        Institutionalized/Other (I\_OTH) or Non-Institutionalized/Other
        (NI\_OTH), then code it **1370 Other Institutional**. In this
        particular case, there is a large number in the I\_CORR field
        for the Census block reference data so it would be coded
        **1340**.

<figure>
<img src="1340_1.PNG" title="1340_1.PNG" width="300" alt="1340_1.PNG" /><figcaption aria-hidden="true"><code>1340_1.PNG</code></figcaption>
</figure>

Religious Facilities (1350)
---------------------------

**Definition:** Houses of worship, along with associated structures and
property.

**Discussion:** It is important to remember that the key concept here is
that the parcel contains a house of worship for that particular religion
for it to be coded 1350. In some cases, the house of worship building
and associated parking will take up more than one parcel. It is ok to
code all of them 1350. Often you will also find parcels owned by a
religious organization, but the activity at that location is not
primarily worship. It may be a house owned by the organization for its
staff or it may be a social service organization run by that religious
organization. In these cases, do NOT code the parcel 1350. Instead,
identify the way the land is being used, and code it accordingly.
Usually this means a residential code (1111, 1112, or 1130), a code for
institutional other (1370), or a school code depending on the grade
level of education provided. Remember that religious organizations often
own houses in residential neighborhoods, not just next to their house of
worship. So if a house in a residential neighborhood is owned by a
religious organization, code it as a house!

Also, be sure to pay attention to the directions in the Q & A below for
when a house of worship and a parochial school share the same parcel or
are on adjacent parcels.

**Be Aware: Not all church buildings are currently houses of worship**
The photo below shows a church building. However, there are several
pieces of information indicating this building is not currently used for
worship. Look at the name of the owner of the parcel. How does the
county code it? Is there a Dunn & Bradstreet point associated with this
parcel? For this photo, the owner is Masonic Building Corp. County codes
it Commercial and a D&B point says it is a Masonic Lodge. With this
information, the appropriate land use code would be **1215 Urban Mix**.
<img src="1215_2.PNG" title="fig:1215_2.PNG" width="100" alt="1215_2.PNG" />

**Be Aware: Not all current houses of worship have county tax exempt
status** While most all active religious houses of worship will have
county tax exempt status, there are parcels containing currently active
houses or worship which do not happen to have this county tax exempt
status. If you have definitive evidence that a parcel or group of
parcels is owned by a religious organization and contains a house of
worship and associated parking, it is appropriate to code this **1350**
even though the county code is not Exempt. **Examples:**

**Q&A:**

-   *Q: How do I code a separate parcel owned by a religous organization
    that primarily has a house on it while the actual religous
    organization building for assembly is on a different parcel?*
    -   **A:** Code this as residential if only the house is on the
        parcel, not the building in which the congregation meets.
        Remember to code the residential units as "1".
-   *Q: A parochial school and the associated church are in the same
    parcel. How do I code this?*
    -   **A:** Following the note at this top of this 1300 Institutional
        section that the order of the 1300 codes implies a sequence for
        selection, you would code this parcel for the school. Also, put
        an "R" in the MODIFIER field to denote that this parcel also has
        a religion land use. HOWEVER, first check the enrollment for the
        school (there is an enrollment field in the K-12 Schools
        reference layer); if a school on church propoerty reports zero
        enrollment, then code the property as **1350 (Religious)**.
-   *Q: What do I do with a separate parcel that is a parking lot for a
    church or for a church and associated parochial school?*
    -   **A:** If there is only a church, then also code the parking lot
        parcel as **1350 Religious Facilities**. If there is a church
        and associated school, then you would have coded those parcels
        as **1321 K-12 Educational Facilities** with an "R" in the
        Modifier field. Do the same for the parcel that is a parking lot
        for the church and/or school, making sure to put an "R" in the
        Modifier field for this parcel too.
-   *Q: How do I code a parcel containing a social service organization
    that is a ministry of a religious organization?*
    -   **A:** Since there is no house of worship on this parcel, this
        will **NOT** be coded **1350**. IF the county says it is tax
        exempt, most likely it will qualify to be coded as **i1370
        Institutional Other** for the specialized professional services
        provided. IF the county codes it as Commercial, then code it
        **1215 Urban Mix**.
-   *Q: How do I code a parcel that is identified as residential by the
    county and with 1 residential unit on it, but the aerial photo shows
    that the parcel has a small church and parking lot on it and also a
    house on it?*
    -   **A:** Code this **1350 Religious Facilities** for the church
        and also make sure the residential units field has 0 residential
        unit in it. Even though there is a house on this parcel, ONLY
        parcels coded as residential will contain a residential unit
        number in the final processing.

Cemeteries (1360)
-----------------

**Definition:** Includes associated chapels and mausoleums.

**Discussion:**

**Examples:**

**Q&A:**

-   *Q: I found a pet cemetery complete with tombstones and a building
    similar to a funeral parlor. How do I code this?*
    -   **A:** Code this also as cemetery. The land use and other
        factors are similar to cemeteries for people.

Other Institutional (1370)
--------------------------

**Definition:** Includes: YMCA, Moose, Elks, VFW, and similar service
organizations. It also includes the YMCA, YWCA, Salvation Army service
centers, and other tax-exempt social service organizations that provide
specific social services for people. It also includes free-standing
buildings used for workforce development purposes that are not in an
office space setting. However, organizations that provide services for
animals such as animal shelters or dog training clubs will be considered
1215 Urban Mix. **Criteria for classifying as 1370 includes:**

-   Property is classed as "Exempt" by the county
-   The use does not fall into any of the other Institutional categories
-   Owner is a "service" (Elks, VFW, etc.) or a social service (YMCA,
    Salvation Army, etc.)
-   Excluded would be office buildings owned by such an organization in
    which the primary function is administrative, rather than service to
    people. These would be coded 1220 Office.
-   Also, see Discussion below about residences owned by non-profit
    social service organizations.

**Discussion:** **Residence owned by non-profit social service
organization** With some tax-exempt, non-profit social service
organizations which own residences, distinctions must be made. For
example, a service center for Salvation Army would be coded as
institutional other (1370), but a residence owned by Salvation Army for
its employees or to house clients would be coded using the appropriate
residence code depending on whether it is a house, a duplex or
townhouse, or an apartment building. This would be true for other
tax-exempt, non-profit social service organizations that own houses that
are used as group living facilities for the mentally or physically
disabled, or residences for extended rehabilitation treatment. If it
looks like a house with no easy indication of separate apartments, then
code it as single-family detached or attached residential (1111 or
1112). You can also use the Census Data reference layer to help you
decide the code.

With Moose, Elk, VFW, Masonic Lodges, similar service
lodges/organizations and also other social service organizations, an
important criteria for coding a non-residential building **1370 Other
Institutional** is whether the county has given it tax-exempt status. If
this is the case, then this code is appropriate unless, of course, it is
a residence owned by such an organization as is mentioned above. If the
property is coded Commercial by the county, then **1215 Urban Mix** will
be the likely land use code, unless you happen to have strong evidence
which would support a different code.

**Examples:** **Unclear if parcel is residence owned by tax exempt
organization** The photos below show a parcel that contains what could
be a large, tax-exempt apartment building owned by Uhlich Children's
Advantage Network, a non-profit social service agency with many programs
and services. While the census count of 81 households for this census
block and the street view of the building could be a case for coding it
as an apartment building, much more investigation would need to be done
to code it that with certainty. Because of we are not certain it is not
used as offices or some other use by that non-profit organization, we
will code it **1370 Institutional Other**. It is typically easier to
code houses owned by tax exempt organizations as residential.
<img src="1370_1.PNG" title="fig:1370_1.PNG" width="400" alt="1370_1.PNG" />
<img src="1370_2.PNG" title="fig:1370_2.PNG" width="300" alt="1370_2.PNG" />

**Q&A:**

-   *Q: How do I code the large building and parking lot for Institute
    in Basic Life Principles in Oak Brook? It is a Christian
    organization that provides conferences, seminars, teaching
    materials, and individual mentoring, but there are no religious
    worship services provided. Likewise, how do I code the Robert Crown
    Center for Health Education? This organization provides health
    education to children and parents.*
    -   *' A:*' Since these two organization are both non-profit and
        provide such specific services, it is probably best to code each
        as **1370 Other Institutional** This will be true for other
        similar organizations especially if the county also codes the
        parcel as tax exempt.
-   *Q: How do I code a parcel containing a social service organization
    that is a ministry of a religious organization?*
    -   **A:** Since there is no house of worship on this parcel, this
        will **NOT** be coded **1350**. IF the county says it is tax
        exempt, most likely it will qualify to be coded as
        **institutional other 1370** for the specialized professional
        services provided. IF the county codes it as Commercial, then
        code it **1215 Urban Mix**.
-   *Q: In the photo below are 2 parcels coded as residential by the
    county. This is Fox Valley Adult Transition Center which is a
    facility in which women are transitioned from prison life to regular
    life. the parcel owner is Old Second National Bank of Aurorar,
    Trustee. How should this be coded?*
    -   **A:** Based on the description of Fox Valley Adult Transition
        Center, the choice would be between 1340 Correctional Facility
        and 1370 Other Institutional. In this case, let the Census block
        reference data be your guide. If that census block has a
        significant incarcerated population (the I\_CORR field, meaning
        Institutionalized Group Quarters, Correctional), then go with
        **1340 Prison/Correctional**. If the census shows that
        population in some other group quarters situation, either
        Institutionalized/Other (I\_OTH) or Non-Institutionalized/Other
        (NI\_OTH), then code it **1370 Other Institutional** In this
        particular case, there is a large number in the I\_CORR field
        for the Census block reference data so it would be coded
        **1340**.
        <img src="1340_1.PNG" title="fig:1340_1.PNG" width="300" alt="1340_1.PNG" />

<!-- -->

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

National Laboratory (1380)
--------------------------

**Definition:** Special category for Argonne National Laboratory and
Fermilab.

**Discussion:** Argonne is entirely in DuPage County; Fermilab is in
DuPage and Kane Counties.

**Examples:**

**Q&A:**

---

*Return to [A field guide to Land Use Inventory classifications](./README.md)*
