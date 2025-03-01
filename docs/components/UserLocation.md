---
custom_edit_url: https://github.com/rnmapbox/maps/blob/main/src/components/UserLocation.tsx
---

  

```tsx
import { UserLocation } from '@rnmapbox/maps';

UserLocation

```


## props

  
### androidRenderMode

```tsx
'normal' | 'compass' | 'gps'
```
native/android only render mode

 - normal: just a circle
 - compass: triangle with heading
 - gps: large arrow

@platform android


  
### animated

```tsx
boolean
```
Whether location icon is animated between updates

  _defaults to:_ `true`

  
### children

```tsx
ReactElement | ReactElement[]
```
Custom location icon of type mapbox-gl-native components


  
### minDisplacement

```tsx
number
```
Minimum amount of movement before GPS location is updated in meters

  _defaults to:_ `0`
[Set Displacement](../examples/UserLocation/SetDisplacement)
  
### onPress

```tsx
func
```
Callback that is triggered on location icon press
*signature:*`() =&gt; void`

[Show Map](../examples/Map/ShowMap)
  
### onUpdate

```tsx
func
```
Callback that is triggered on location update
*signature:*`(location:Location) =&gt; void`

[User Location Updates](../examples/UserLocation/UserLocationUpdates)
  
### renderMode

```tsx
UserLocationRenderMode
```
@deprecated use LocationPuck component instead of UserLocationRenderMode.Native
Which render mode to use.

  _defaults to:_ `UserLocationRenderMode.Normal`
[User Location Render Mode](../examples/UserLocation/UserLocationRenderMode)
  
### requestsAlwaysUse

```tsx
boolean
```
Request the always location permission, and listen to the location even when the app is in background

@platform ios

  _defaults to:_ `false`

  
### showsUserHeadingIndicator

```tsx
boolean
```
Show or hide small arrow which indicates direction the device is pointing relative to north.

  _defaults to:_ `false`

  
### visible

```tsx
boolean
```
Whether location icon is visible

  _defaults to:_ `true`
[User Location Render Mode](../examples/UserLocation/UserLocationRenderMode)
  





## methods
### setLocationManager(&#123; running &#125;: &#123; running?: boolean &#125;)

Whether to start or stop listening to the locationManager<br/><br/>Notice, that listening will start automatically when<br/>either `onUpdate` or `visible` are set

#### arguments
| Name | Type | Required | Description  |
| ---- | :--: | :------: | :----------: |
| `{ running }: { running?: boolean }` | `{running?:boolean}` | `Yes` | undefined |


### needsLocationManagerRunning()

If locationManager should be running

#### arguments
| Name | Type | Required | Description  |
| ---- | :--: | :------: | :----------: |




