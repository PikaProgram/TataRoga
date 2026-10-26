# Tata Roga

Crowd-reported status of public facilities on the ITB Ganesha campus, usable offline on phones.

## Language

**Facility**:
A public amenity on the ITB Ganesha campus whose status is tracked. E.g. a vending machine, public bathroom, water dispenser, coworking space.
_Avoid_: pin, spot, item

**Property**:
An aspect of a facility that can be reported on, defined by its facility type (e.g. Status, Stock, Amenities). A property is single- or multi-select.
_Avoid_: tag, attribute, field

**Value**:
One of the allowed states of a property (e.g. "operational" for Status; "cold", "hot" for Water).
_Avoid_: tag, option, state
_Avoid_: category, kind

**Report**:
A single observation of one facility by one user, covering one or more of the facility's properties.
_Avoid_: feedback, ping, entry

**Consensus**:
The current state of a facility, derived per property by weighted majority over recent reports.
_Avoid_: status, verdict, majority vote

**Trust**:
A per-user score reflecting how often a user's reports are confirmed by independent observers; it weights the user's reports in the consensus. Anonymous reports carry a fixed minimum weight.
_Avoid_: reputation, karma, credit

**Verified user**:
A user whose registration proved they hold an itb.ac.id email address.
_Avoid_: member, registered user
