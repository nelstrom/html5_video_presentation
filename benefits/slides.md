!SLIDE
# BENEFITS

!SLIDE bullets incremental small
## BENEFITS

* Native - works with page zoom
* Style with CSS
* Script with JavaScript
* Integration with \<canvas\>
* Low CPU usage
* Future proof

!SLIDE
## PAGE ZOOM
img: page with video

!SLIDE
## PAGE ZOOM
img: page with video zoomed

!SLIDE
## PAGE ZOOM
img: page with FLASH video zoomed

!SLIDE
## SCRIPT WITH JAVASCRIPT
img: the W3C video api

!SLIDE bullets
## CUSTOM CONTROLS

* \<html\> elements needn't overlap video frame
* brand your buttons (e.g. Fischer Price)
* \<ul\> of chapter markers

!SLIDE
## STYLE WITH CSS
img: the SUBLIME video player

!SLIDE
## INTEGRATION WITH \<CANVAS\>

!SLIDE smaller

## canvas.drawImage()

    @@@javascript
    var canvas = document.getElementById('canvas').getContext('2d');
    var video = document.getElementsByTagName('video')[0];
    video.onloadeddata = function(e) {
      canvas.drawImage(video, 0, 0);
    }

!SLIDE
img: the tile game using video

!SLIDE
img: the youtube video chooser

!SLIDE
## FUTURE PROOF
img: FireFox 3.6 full screen dialogue

 !SLIDE
## FUTURE PROOF
img: iPad screenshot

