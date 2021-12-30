# c4c - Data and Python scripts for generating cyclically 4-connected cubic graphs

## Background

This repository contains data files with representations of all cyclically
4-connected cubic graphs of size 2*k* for 4 &le; *k* &le; 10. This data was
generated using methods based on results in the paper "Generating cyclically
4-connected cubic graphs" by R. J. Kingan and S. R. Kingan. Python scripts for
generating the data will be added at a later date.

## Organization of the data

The directory `non-planar-graphs` contains representations of non-planar
cyclically 4-connected cubic graphs, except for the Petersen graph
*P*<sub>10</sub> and the M&ouml;bius ladders *V*<sub>2*k*</sub>. There is one
file for each size:

* `non-planar-c4c-10.txt.gz`
* `non-planar-c4c-12.txt.gz`
* `non-planar-c4c-14.txt.gz`
* `non-planar-c4c-16.txt.gz`
* `non-planar-c4c-18.txt.gz`
* `non-planar-c4c-20.txt.gz`

The directory `all-graphs` contains representations of both planar and
non-planar cyclically 4-connected cubic graphs, except for the Petersen graph
*P*<sub>10</sub>, the M&ouml;buis ladders *V*<sub>2*k*</sub> and the ladder
graphs *Q*<sub>2*k*</sub>. There is one file for each size:

* `c4c-10.txt.gz`
* `c4c-12.txt.gz`
* `c4c-14.txt.gz`
* `c4c-16.txt.gz`
* `c4c-18.txt.gz`
* `c4c-20.txt.gz`

## File format

The graphs representations are stored in gzipped text files, with one graph per
line in [graph6 format](http://users.cecs.anu.edu.au/~bdm/data/formats.html).
