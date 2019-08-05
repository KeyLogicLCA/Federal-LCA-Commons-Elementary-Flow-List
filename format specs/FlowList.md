## Flow List format

A Flow List is in the form of a pandas data frame with the following fields.

 Field | Type | Required |  Note |
----------- |  ---- | ---------| -----  |
 Flowable | string | Y | The flow name |
 CAS No | string | N | CAS number |
 Formula | string | N | Chemical formula|
 Synonyms | string | N | Flow synonyms
 Unit | string | Y  | The reference unit. uses [olca-ipc.py](https://github.com/GreenDelta/olca-ipc.py) units |
 Class | string | Y | The flow class, e.g. `Energy` or `Chemical` |
 External Reference | string | N | E.g. a web link |
 Preferred | int |  N |   `1` for preferred, `0` for non-preferred
 Context | string | Y | A path-like set of context compartments in the form of directionality/environmental media/environmental compartment... e.g. `emission/air/tropophere`|  
 Flow UUID | string | Y | Unique hexadecimal ID for the flow |
 AltUnit | string | N | Alternate unit for the flow |
 AltUnitConversionFactor | float | N | Conversion factor in the form of alternate units/reference unit | 
