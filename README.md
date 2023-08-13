# Dovrefjell 3D

A 3d representation of hiking routes in Dovrefjell, Norway.

Adapted from https://github.com/bertt/corsica_gr20.

## Overpass QL query for Huts
This query was run in https://overpass-turbo.eu/ and exported to GeoJSON.
```
node
  [tourism=wilderness_hut]
  ({{bbox}});
node
  [tourism=alpine_hut]
  ({{bbox}});
node
  [amenity=shelter]
  ({{bbox}});
out;
```