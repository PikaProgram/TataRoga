# Per-property consensus

A facility has several independent aspects (a vending machine can be operational yet out of drinks; a bathroom can be open yet lack toilet paper), so one combined status cannot represent them.

We decided: each facility type declares a fixed set of **Properties**, each with allowed **Values** (single- or multi-select). A report covers whichever properties the observer noticed. The **Consensus** is computed *independently per property* as the weighted majority of reports mentioning that property in the last 7 days, weighted by reporter trust.
