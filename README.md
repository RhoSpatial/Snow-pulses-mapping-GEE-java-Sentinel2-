## Snow-pulses-mapping-GEE-java-Sentinel_2
### Vectorizing snow on individual snowy cloud free scene for clipping
```js
var S2snow_13jan21_MASK = ee.Image('COPERNICUS/S2_SR/20210113T120331_20210113T120325_T28RBS')
                                  .normalizedDifference(['B3','B11']).clip(box).gte(0.4) .selfMask();
var S2snow_17feb21_MASK = ee.Image('COPERNICUS/S2_SR/20210217T120319_20210217T120320_T28RBS')
                                  .normalizedDifference(['B3','B11']).clip(box).gte(0.4) .selfMask();

var jan_vectors = S2snow_13jan21_MASK.reduceToVectors({
  geometry: box,
  crs: S2snow_13jan21_MASK.projection(),
  scale: 10,
  geometryType: 'polygon',
  eightConnected: false,
  labelProperty: 'zone',                                });

///jep

```
the
## test
`the` best
 refer to the [name of link](https://eslint.org/docs/user-guide/configuring#specifying-processor "My link window")

```diff
- This is a red colored line
+ This is a green colored line
@@ This is a purple colored line @@
$$ the testing $$
tested
```
