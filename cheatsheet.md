



# A-Frame cheat sheet
Always use `a-entity` except for `a-scene`, `a-camera`, `a-assets`, `a-asset-item`, `img`, `video`. 

## standard components:
```
geometry="primitive:box; width:1.0; height:2.0; depth:3.0;"
geometry="primitive:sphere; radius:0.5;"
geometry="primitive:torus; radius:2; radiusTubular: 0.5;"
geometry="primitive:plane; height:10; width:10;" 
```

See more at [https://aframe.io/docs/0.8.0/components/geometry.html](geometry)

## load images, videos, sounds, 3d models, etc. with assets
load resources in `a-assets` then reference with `#someIdName`. Use `a-asset-item` for models,
`img` for images, `audio` for sounds, `video` for video files.  YouTube does not allow A-Frame usage.

```html
<a-assets>
    <a-asset-item id="lake" src="https://server.com/model.gltf"></a-asset-item>
    <img id="river" src="assets/image.jpg">
    <video id="ocean" src="https://server.com/video.mp4"></video>
    <audio id="waves" src="https://server.com/song.mp3"></audio>
</a-assets>
```

## position and rotation

`position="x y z"` in meters

`rotation="x y z"` in degrees


## color material
change the color with `material`
use color names or RGB as hex

`material="color:red"`  
`material="color:#FF0000"` 

## load custom 3d objects
load objects from GLTF files in the a-assets section, then reference as
```
gltf-model="#lake"
```

## find more stuff
find GLTF files on the web at [Sketchfab](https://sketchfab.com/), search
for once that allow downloading. Also [Poly](https://poly.google.com/)

Find 360 photos on the web with '360 equirectangular creative commons'
[Search: equirectangular | Flickr](https://www.flickr.com/search/?text=equirectangular&license=2%2C3%2C4%2C5%2C6%2C9)

Find sounds on the web at [FreeSound.org](https://freesound.org/)









