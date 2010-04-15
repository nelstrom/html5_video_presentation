!SLIDE
# BENEFITS

!SLIDE
## PAGE ZOOM

!SLIDE full-page
![Video at normal size](video-size-normal.png)     

!SLIDE full-page
![Zoomed video](video-size-zoomed.png)     

!SLIDE
## STYLE WITH CSS
!SLIDE full-page
![Sublime video player](sublime-video.png)     

!SLIDE
## SCRIPT WITH JAVASCRIPT
!SLIDE full-page
![Video events api](video-events.png)     

!SLIDE bullets incremental
## CUSTOM CONTROLS

* \<html\> elements needn't overlap video frame
* brand your buttons (e.g. Fischer Price)
* \<ul\> of chapter markers

!SLIDE
## FUTURE PROOF

!SLIDE full-page
![Firefox full screen menu](firefox-fullscreen.png)

 !SLIDE full-page
![Ipad screenshot](ipad-screenshot.png)

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

!SLIDE full-page
![Tile video game](tile-game.png)

