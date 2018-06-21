



# A-Frame cheat sheet

## standard entity

This makes a 1 meter red cube ,
positioned 4 meters in front of the camera at head height,
rotated by 45 degrees

```html
<a-entity
   geometry="primitive:box; width:1.0, height:1.0, depth:1.0;"
   material="color:red;"
   position="0 1.5 -4"
   rotation="0 45 0"
>
</a-entity>
```


Always use `a-entity` except for `a-scene`, `a-camera`, `a-assets`, `a-asset-item`, `img`, `video`. 

## standard components:
```html
geometry="primitive:box; width:1.0; height:2.0; depth:3.0;"
geometry="primitive:sphere; radius:0.5;"
geometry="primitive:torus; radius:2; radiusTubular: 0.5;"
geometry="primitive:plane; height:10; width:10;" 
```

See more at [https://aframe.io/docs/0.8.0/components/geometry.html](https://aframe.io/docs/0.8.0/components/geometry.html)

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

Full AFrame Docs at [https://aframe.io/docs/0.8.0/introduction/](https://aframe.io/docs/0.8.0/introduction/)

Assets for this project at [https://vr.josh.earth/assets/](https://vr.josh.earth/assets/)

find GLTF files on the web at [https://vr.josh.earth/assets/](https://sketchfab.com/), search
for models that allow downloading. Also [https://vr.josh.earth/assets/](https://poly.google.com/)

Find 360 photos on the web by searching for '360 equirectangular creative commons'
[Search: equirectangular | Flickr](https://www.flickr.com/search/?text=equirectangular&license=2%2C3%2C4%2C5%2C6%2C9)

Find sounds on the web at [FreeSound.org](https://freesound.org/)









