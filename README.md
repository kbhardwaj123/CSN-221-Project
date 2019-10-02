# Dual Data Cache

## Abstract
The Scalar Processors have a performance setback when it comes to Vector(Array) processing and other vector applications because of the Scalar processors limitation of processing single instruction at a time. The two most important reasons holding them back are: the use of same organization caching both spatial and temporal locality and the genrally implemented "eager" caching policy. This leads to the well known trade-off of designing caches with more number lines or implementing design which has large line size.

The remedy to such trade-off is a data cache organisation system called **Dual Data Cache**. Implementaion of such cache design leads to efficient exploitaion of both spatial and temporal localities in an efficient manner.
The Dual Data Caching technique implement lazy caching technique which is a caching strategy that loads data into the cache when it is mandatory and that is achieved by the use of *locality prediction table* which maintains a history of details regarding the most recently executed load/store instruction.  