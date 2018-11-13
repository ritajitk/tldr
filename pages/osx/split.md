# split

> Split a file into pieces.

- Split a file, each split having 10 lines (except the last split):

`split -l {{10}} {{filename}}`

- Split a file into 5 files. File is split such that each split has same size (except the last split):

`split -n {{5}} {{filename}}`

- Split a file with 512 bytes in each split (except the last split; use 512k for kilobytes and 512m for megabytes):

`split -b {{512}} {{filename}}`

- Split a file into 10 files with 100 Kbytes, where each file is named with numeric suffixes (easier to merge later):

`split -d -b {{100k}} {{filename}} {{output}}`
