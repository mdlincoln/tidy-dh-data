## Description

Artwork data from a variety of institutions.

## Format

### artists.csv

1. `name` Artist name (primary key) (joining column with `creations.csv - name`)
2. `birth_year` Integer. Year of birth

### artworks.csv

1. `acq_no` Museum acquisition number (primary key) (joining column with `creations.csv - acq_no`)
2. `museum` Museum name (joining key to `museum.csv - museum`)
3. `tags` Semicolon-delimited column with tags describing artwork content
4. `year_early` Integer. Earliest possible year of creation
5. `year_late` Integer. Latest possible year of creation

### creations.csv

1. `acq_no` Museum acquisition number (joining column with `artworks.csv - acq_no`)
2. `name` Artist name (joining column with `artists.csv - name`)
3. `qualification` Qualifier for this attribution

### museums.csv

1. `museum` Museum name (primary key) (joining column with `artworks.csv - museum`)
2. `city` City in which this museum is located

## Source

XXX

## Citation

XXX
