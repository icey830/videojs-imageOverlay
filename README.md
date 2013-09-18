videojs-imageOverlay
====================

Adds a clickable image over the top of the player that is displayed during a specified start and stop time.

![videojs-imageOverlay](http://assets0.ordienetworks.com/misc/videojs/imageOverlay.jpg)

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

## OPTIONS:
  * __image_url__ (required): location of the image
  * __click_url__: where the image links to
  * __opacity__: css opacity of the image, default is 0.7
  * __start_time__: time (in seconds) when the image displays skip if you want the image to be displayed at start of * playback
  * __end_time__: time (in seconds) when the image disappears
  * __height__: css height of the image's container div, default is 15% of the video. Image takes up 100% of this element's height
  * __width__: css width of the container div, default is 100%
