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
