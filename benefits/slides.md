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

!SLIDE
![Video at normal size](../images/video-size-normal.png "Title is optional")     

!SLIDE
![Zoomed video](../images/video-size-zoomed.png "Title is optional")     

!SLIDE
## STYLE WITH CSS
!SLIDE
![Sublime video player](../images/sublime-video.png "Title is optional")     

!SLIDE
## SCRIPT WITH JAVASCRIPT
!SLIDE
![Video events api](../images/video-events.png "Title is optional")     

!SLIDE bullets incremental
## CUSTOM CONTROLS

* \<html\> elements needn't overlap video frame
* brand your buttons (e.g. Fischer Price)
* \<ul\> of chapter markers

!SLIDE
## FUTURE PROOF

!SLIDE
![Firefox full screen menu](../images/firefox-fullscreen.png)

 !SLIDE
![Ipad screenshot](../images/ipad-screenshot.png)

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
![Tile video game](../images/tile-game.png)

!SLIDE
![youtube video chooser](../images/youtube-chooser.png)

