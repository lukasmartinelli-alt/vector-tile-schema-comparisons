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
8,16d7
<   [maki]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [ref]
18,21d8
< #barrier_line
<   [class]
< #building
<   [underground]
23,30d9
<   [code]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
32,33d10
< #housenum_label
<   [house_num]
36d12
<   [type]
39d14
<   [type]
42,60d16
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [placement]
< #mountain_peak_label
<   [elevation_ft]
<   [elevation_m]
<   [maki]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
62,72d17
<   [capital]
<   [ldir]
<   [localrank]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [scalerank]
75,84d19
<   [localrank]
<   [maki]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [ref]
86,96d20
<   [type]
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
99d22
<   [oneway]
101d23
<   [type]
104,113d25
<   [len]
<   [localrank]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [ref]
115,125d26
<   [shield]
< #state_label
<   [abbr]
<   [area]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
127,134d27
<   [area]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
137,147d29
<   [type]
< #waterway_label
<   [class]
<   [name]
<   [name_de]
<   [name_en]
<   [name_es]
<   [name_fr]
<   [name_ru]
<   [name_zh]
<   [type]
```
