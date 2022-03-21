Navigating with SPARQL
======================

> A list of SPARQL ready-to-be-pasted binding blocks to compute
  operations on (lat,lon) pairs

Abstract
--------

Let's assume you are on a boat and have to navigate only basic items
such as a map or a compass, and a . . . . . . SPARQL engine! How to
set a course? How to compute distances? Here, we provide a set of
SPARQL code-blocks to be used in such situation and more generally in
use-cases where practitioners need to compute mathematical calculus on
geo-data represented by (lat,lon) pairs.


How to use these resources?
---------------------------

The repository provides several ready-to-be-used bindings blocks of
SPARQL 1.1. Practically, the various funtions are split in several
files which are all self-contained. They are all adopting the same
structure.

Warning: If a specific requires to use several blocks within the same
final SPARQL query, the query designer will have to pay attention to
the multiple intermediate variables (e.g. ?sub1, ?sub2, ...) to be
sure that the same (sub-)variable will not be called by different
feature-blocks, otherwise renaming actions should be taken!


Repository files
----------------

This repository contains:

- `README.md` (this file): providing documentation;
- `distance_great_circle.txt`: taking two (lat,lon) points, returns their great-circle distance on Earth;
- `distance_equirectangular_approx.txt`: performs an equirectangular approximation to compute the distance between points;
- `distance_to_horizon.txt`: returns the distance to the horizon from a specific height;
- `initial_bearing_great_circle.txt`: gives the initial bearing for a great-circle course between two points;
- `mid_point_great_circle.txt`: computes the coordinates (lat,lon) in radians of the mid-point of a great-circle course between two points (considering their lat/lon coordinates in degrees);
- `LICENSE`.


Author
------

Damien Graux <https://dgraux.github.io/>  
Inria, France  
2022
