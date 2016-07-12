# schema-comparisons

Compare vector tile schemas of different style and TileJSON specs with OSM2VectorTiles

## Schemas

**TileJSON**

- osm2vectortiles-v2
- mapbox-streets-v7

**Styles**

- basic-v9
- dark-v9
- streets-v9
- bright-v9
- light-v9

## Comparisons

**mapbox-streets-v7 vs osm2vectortiles-v2**

```diff
4d3
<   [iso_3166_1]
32d30
<   [parent]
34d31
<   [type]
53,58d49
< #motorway_junction
<   [class]
<   [name]
<   [ref]
<   [reflen]
<   [type]
108d98
<   [layer]
114d103
<   [iso_3166_2]
```

**osm2vectortiles-v2 vs bright-v9**

```diff
*** osm2vectortiles-v2.schema	Tue Jul 12 14:42:45 2016
--- bright-v9.schema	Tue Jul 12 14:43:20 2016
***************
*** 5,147 ****
  #aeroway
    [type]
  #airport_label
-   [maki]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [ref]
    [scalerank]
- #barrier_line
-   [class]
- #building
-   [underground]
  #country_label
-   [code]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
    [scalerank]
- #housenum_label
-   [house_num]
  #landuse
    [class]
-   [type]
  #landuse_overlay
    [class]
-   [type]
  #marine_label
    [labelrank]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [placement]
- #mountain_peak_label
-   [elevation_ft]
-   [elevation_m]
-   [maki]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
  #place_label
-   [capital]
-   [ldir]
-   [localrank]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [scalerank]
    [type]
  #poi_label
-   [localrank]
-   [maki]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [ref]
    [scalerank]
-   [type]
- #rail_station_label
-   [maki]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [network]
  #road
    [class]
-   [oneway]
    [structure]
-   [type]
  #road_label
    [class]
-   [len]
-   [localrank]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [ref]
    [reflen]
-   [shield]
- #state_label
-   [abbr]
-   [area]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
  #water_label
-   [area]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
  #waterway
    [class]
-   [type]
- #waterway_label
-   [class]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [type]
--- 5,29 ----
```
