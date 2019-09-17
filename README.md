# Dresden Maps
Contains a data file with locations from The Dresden Files. The data file is to be used for [my map tutorial in R](https://katiesaund.com/post/dresden_maps/). 


To access the data, download the file, then:
```
> install.packages("tidyverse")
> library(tidyverse)

> dresden_locations <- read_tsv("Dresden_Files_locations.tsv")

> head(dresden_locations)
# A tibble: 6 x 6
  Name                                     First_Appearance Character     Group   Lat  Long
  <chr>                                    <chr>            <chr>         <chr> <dbl> <dbl>
1 Burnham Harbor, Chicago                  Death Masks      Thomas Wraith NA     41.9 -87.6
2 Chicago Botanic Gardens                  Cold Days        Summer Lady   NA     42.1 -87.8
3 Cook County Hospital, Chicago            Fool Moon        NA            NA     41.9 -87.7
4 Field Museum of Natural History, Chicago Dead Beat        NA            NA     41.9 -87.6
5 Carbon & Carbide Building, Chicago       Skin Game        NA            NA     37.4 -94.8
6 Graceland Cemetery, Chicago              Grave Peril      NA            NA     42.0 -87.7
```

`Name` is the name of the location. 
`First_Appearance` is the book in which the location is initially described.
`Character` is the name of the person who is most strongly associated with the location.
`Group` is the society most associated with the location (e.g. White Council, Red Court, Paranet, etc...)
`Lat` is the location's latitude as determined by Google Maps. 
`Long` is the location's longitude as determined by Google Maps. 

