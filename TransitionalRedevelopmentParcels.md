# Transitional/Redevelopment Parcels

One shortcoming that was pointed out during the 2013 Update was the
inability to flag a recently-vacated parcel which was going to be
redeveloped into a different use. Current coding rules say that, even if
a property is vacated, it should still be coded by the former use if
there’s been no modification to the property. A prime example of this is
the old Motorola campus outside in Harvard, which has sat vacant since
2003 but is still being coded as Industrial/Manufacturing. We take this
approach because it would be impossible to keep up with the
vacant/occupied status of so many properties. As long as the vacant
structure on the property is sound, then theoretically it can be
occupied by some future tenant for the same purpose. If we know that a
property is (a) vacant, and (b) going to be converted to another use,
then we need a way of flagging that property, not only to indicate that
the coded activity no longer applies, but also to let us know that there
are redevelopment plans afoot. This will help out the pre-processing for
the subsequent LU update since the Transition flag will alert us to a
new land use for that site. An example of how this would have been
applied in 2013: the old Children’s Memorial Hospital in Lincoln Park
closed in 2012 but the building was intact. Redevelopment plans
(residential + retail) were in the works but no actual demolition or
construction had taken place in 2013. Coding rules dictate that it
should still be coded Medical even though we knew the property was going
to be something else; and it wouldn’t be right coding it as Construction
if work had not actually started.

## How to flag a Transitional parcel
We will stick with the convention
of coding the parcel to the “old” use. With the parcel selected, select
the **COMMENT Update** tool (in the Non-Coding Tools toolbox). The tool
will have a window for you to type a statement which will go into the
COMMENT field for that parcel—write a simple description such as
“mixed-use, construction begins August 2017” as well as a check-box to
have the tool write a “T” in the MODIFIER field which will serve as the
Transitional indicator.

*Return to [A field guide to Land Use Inventory classifications](./README.md)*
