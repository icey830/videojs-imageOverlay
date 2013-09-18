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
  image_url (required): location of the image
  click_url: where the image links to
  opacity: css opacity of the image, default is 0.7
  start_time: time (in seconds) when the image displays skip if you want the image to be displayed at start of playback
  end_time: time (in seconds) when the image disappears
  height: css height of the image's container div, default is 15% of the video. Image takes up 100% of this element's height
  width: css width of the container div, default is 100%
