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
file for each size. The files and the number of graphs in each file are listed
in the table below:

| Size | Filename | Number of graphs |
| ---: | -------- | ---------------: |
| 10 | `non-planar-c4c-10.txt.gz` | 2 |
| 12 | `non-planar-c4c-12.txt.gz` | 15 |
| 14 | `non-planar-c4c-14.txt.gz` | 79 |
| 16 | `non-planar-c4c-16.txt.gz` | 596 |
| 18 | `non-planar-c4c-18.txt.gz` | 6074 |
| 20 | `non-planar-c4c-20.txt.gz` | 78736 |

The directory `all-graphs` contains representations of both planar and
non-planar cyclically 4-connected cubic graphs, except for the Petersen graph
*P*<sub>10</sub>, the M&ouml;buis ladders *V*<sub>2*k*</sub> and the ladder
graphs *Q*<sub>2*k*</sub>. There is one file for each size. The files, along with the number of graphs in each file, and the number of graphs of the same size listed in [OEIS sequence 175847](https://oeis.org/A175847/b175847.txt) are all listed in the table below. 

| Size | Filename | Number of graphs | OEIS number | Note |
| ---: | -------- | ---------------: | ----------: | ---- |
| 10 | `c4c-10.txt.gz` | 2 | 5 | File does not include *V*<sub>10</sub>, *P*<sub>10</sub> or *Q*<sub>10</sub> |
| 12 | `c4c-12.txt.gz` | 16 | 18 | File does not include *V*<sub>12</sub> or *Q*<sub>12</sub> |
| 14 | `c4c-14.txt.gz` | 82 | 84 | File does not include *V*<sub>14</sub> or *Q*<sub>14</sub> |
| 16 | `c4c-16.txt.gz` | 605 | 607 | File does not include *V*<sub>16</sub> or *Q*<sub>16</sub> |
| 18 | `c4c-18.txt.gz` | 6098 | 6100 | File does not include *V*<sub>18</sub> or *Q*<sub>18</sub> |
| 20 | `c4c-20.txt.gz` | 78822 | 78824 | File does not include *V*<sub>20</sub> or *Q*<sub>20</sub> |

## File format

The graphs representations are stored in gzipped text files, with one graph per
line in [graph6 format](http://users.cecs.anu.edu.au/~bdm/data/formats.html).
These files can be read using utilities accompanying [Brendan McKay's nauty
system](https://pallini.di.uniroma1.it/), the [networkx library](https://networkx.org/documentation/stable/reference/readwrite/sparsegraph6.html) in Python, or others.
