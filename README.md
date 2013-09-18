videojs-imageOverlay
====================

Adds a clickable image over the top of the player that is displayed during a specified start and stop time.


## USAGE:

```html
<video id="video" src="movie.mp4" controls></video>
<script src="video.js"></script>
<script src="videojs-imageOverlay.js"></script>
<link href="videojs-imageOverlay.css" rel="stylesheet">
<script>
  var player = videojs('video');
  player.imageOverlay({
    image_url: "http://assets0.ordienetworks.com/misc/JimCarreyEyebrow.jpg",
    click_url:"https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewAlbum?id=624854547",
    opacity: 0.5,
    start_time: 10,
    height: '20%'
  });

</script>
```

