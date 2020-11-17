# DOGAMI Shoreline Profile Data


## Projection information

## Transect data files
### File naming convention
`[littoralcell]_[transect]_transect_data_prj_epsg[epsg code].csv`

| Term | Definition |
-------|-------------
| `[littoralcell]` | |
| `[transect]` | |

Example file name: **Bayocean_Bay1_transect_data_prj_epsg32126.csv**

### Example file contents
```csv
survey_number,survey_date,point_number,easting,northing,distance,elevation,source
1,1997-10-18,1,2229807.882,209765.088,0.000,4.082,LIDAR
1,1997-10-18,2,2229807.000,209765.312,0.910,4.410,LIDAR
```
### Field descriptions
| Field | Description |
-------|-------------
| survey_number | incremental survey from the start, 1 - X 
| survey_date | |
| point_number | |
| easting_meters | |
| northing_meters | |
| distance_meters | |
| elevation_meters | |
| measurement_approach | LIDAR vs GPS |

## Littoral cell inventory files

### File naming convention
`[littoralcell]_littoralcell_inventory.csv`
| Term | Definition |
-------|-------------
| `[littoralcell]` | |

Example file name: **Bayocean_littoralcell_inventory.csv**

Change DOGAMI / NANOOS to DOGAMI-NANOOS

### Example file contents
```csv
transect,littoralcell,littoralcell_fullname,state,provider,projection,survey_count,date_first,date_last,lon,lat,start_lon,start_lat,end_lon,end_lat
Bay1,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.9601,45.5025,-123.9585,45.5023,-123.9629,45.5027
Bay2,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.956,45.5154,-123.9543,45.5153,-123.9591,45.5157
Bay3,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.9542,45.5241,-123.9523,45.524,-123.9579,45.5242
Bay4,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.9532,45.5332,-123.9514,45.5331,-123.9565,45.5334
Bay5,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.9519,45.5414,-123.9498,45.5415,-123.9554,45.5412
Bay6,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,53,1997-10-18,2018-12-10,-123.9506,45.5504,-123.9477,45.5507,-123.955,45.5501
Bay7,Bayocean,Bayocean Spit,Oregon,DOGAMI / NANOOS,epsg:32126,51,1997-10-18,2018-12-10,-123.9513,45.5595,-123.9489,45.5597,-123.9555,45.5588
```
### Field descriptions
| Field | Description |
-------|-------------
transect | |
littoralcell | |
littoralcell_fullname | |
state | |
provider | |
projection | |
survey_count | |
date_first | |
date_last | |
longitude | |
latitude | |
start_lon | |
start_lat | |
end_lon | |
end_lat | |

## Littoral cell inventory geojson files
### File naming convention
`[littoralcell]_littoralcell_inventory.geojson`

| Term | Definition |
-------|-------------
| `[littoralcell]` | |

Example file name: **Bayocean_littoralcell_inventory.geojson**

### File description
The GeoJSON files will be formatted according to the [GeoJSON specification](https://geojson.org/). The information presented in the GeoJSON file will be the same information presented in the [Littoral cell inventory files](#littoral-cell-inventory-files).

