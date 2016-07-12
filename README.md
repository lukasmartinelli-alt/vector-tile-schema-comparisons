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

**mapbox-streets-v7 vs osm2vectortiles-v3**

```diff
4d3
<   [iso_3166_1]
8,18d6
< #airport_label
<   [maki]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [ref]
<   [scalerank]
22d9
<   [underground]
32d18
<   [parent]
34d19
<   [type]
36c21
<   [house_num]
---
>   [addr]
44,62c29
<   [labelrank]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [placement]
< #motorway_junction
<   [class]
<   [name]
<   [ref]
<   [reflen]
<   [type]
< #mountain_peak_label
<   [elevation_ft]
<   [elevation_m]
<   [maki]
---
>   [scalerank]
72d38
<   [ldir]
96,105d61
< #rail_station_label
<   [maki]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [network]
108d63
<   [layer]
114,115d68
<   [iso_3166_2]
<   [len]
126d78
<   [shield]
129c81
<   [area]
---
>   [scalerank]
138c90
<   [area]
---
>   [scalerank]

```

**mapbox-streets-v7 vs osm2vectortiles-v2**

```diff
***************
*** 1,7 ****
  #admin
    [admin_level]
    [disputed]
-   [iso_3166_1]
    [maritime]
  #aeroway
    [type]
--- 1,6 ----
***************
*** 29,37 ****
    [name_fr]
    [name_ru]
    [name_zh]
-   [parent]
    [scalerank]
-   [type]
  #housenum_label
    [house_num]
  #landuse
--- 28,34 ----
***************
*** 50,61 ****
    [name_ru]
    [name_zh]
    [placement]
- #motorway_junction
-   [class]
-   [name]
-   [ref]
-   [reflen]
-   [type]
  #mountain_peak_label
    [elevation_ft]
    [elevation_m]
--- 47,52 ----
***************
*** 105,117 ****
    [network]
  #road
    [class]
-   [layer]
    [oneway]
    [structure]
    [type]
  #road_label
    [class]
-   [iso_3166_2]
    [len]
    [localrank]
    [name]
--- 96,106 ----
```

**osm2vectortiles-v2 vs bright-v9**

```diff
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

**osm2vectortiles-v2 vs dark-v9**

```diff
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
  #barrier_line
    [class]
  #building
    [underground]
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
    [scalerank]
    [type]
  #poi_label
-   [localrank]
    [maki]
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
!   [oneway]
    [structure]
    [type]
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
-   [reflen]
-   [shield]
  #state_label
-   [abbr]
    [area]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
  #water_label
    [area]
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
  #waterway_label
    [class]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [type]
--- 5,41 ----
  #aeroway
    [type]
  #airport_label
    [scalerank]
  #barrier_line
    [class]
  #building
    [underground]
  #country_label
    [scalerank]
  #landuse
    [class]
  #landuse_overlay
    [class]
  #marine_label
    [labelrank]
  #place_label
    [scalerank]
    [type]
  #poi_label
    [maki]
    [scalerank]
  #road
    [class]
!   [layer]
    [structure]
    [type]
  #road_label
    [class]
  #state_label
    [area]
  #water_label
    [area]
  #waterway
    [class]
  #waterway_label
    [class]

```


**osm2vectortiles-v2 vs streets-v9**

```diff
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
  #barrier_line
    [class]
  #building
    [underground]
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
    [localrank]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
    [scalerank]
    [type]
  #poi_label
    [localrank]
    [maki]
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
  #rail_station_label
    [maki]
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
    [oneway]
    [structure]
    [type]
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
    [shield]
  #state_label
-   [abbr]
    [area]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
  #water_label
    [area]
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
  #waterway_label
    [class]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [type]
--- 5,48 ----
  #aeroway
    [type]
  #airport_label
    [scalerank]
  #barrier_line
    [class]
  #building
    [underground]
  #country_label
    [scalerank]
  #landuse
    [class]
  #landuse_overlay
    [class]
  #marine_label
    [labelrank]
  #place_label
    [localrank]
    [scalerank]
    [type]
  #poi_label
    [localrank]
    [maki]
    [scalerank]
  #rail_station_label
    [maki]
  #road
    [class]
+   [layer]
    [oneway]
    [structure]
    [type]
  #road_label
    [class]
    [reflen]
    [shield]
  #state_label
    [area]
  #water_label
    [area]
  #waterway
    [class]
  #waterway_label
    [class]

```

**osm2vectortiles-v2 vs basic-v9**
```diff
***************
*** 1,147 ****
  #admin
-   [admin_level]
-   [disputed]
-   [maritime]
- #aeroway
-   [type]
- #airport_label
-   [maki]
-   [name]
-   [name_de]
-   [name_en]
-   [name_es]
-   [name_fr]
-   [name_ru]
-   [name_zh]
-   [ref]
-   [scalerank]
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
-   [scalerank]
- #housenum_label
-   [house_num]
  #landuse
    [class]
-   [type]
  #landuse_overlay
    [class]
-   [type]
- #marine_label
-   [labelrank]
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
-   [scalerank]
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
-   [class]
-   [oneway]
-   [structure]
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
-   [reflen]
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
- #water_label
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
--- 1,14 ----
```
