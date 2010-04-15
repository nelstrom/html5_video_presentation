!SLIDE
#FLASH VIDEO

!SLIDE smaller
##EXAMPLE FROM YOUTUBE

    @@@html
    <object width="425" height="344">
      <param name="movie"
        value="http://www.youtube.com/v/9sEI1AUFJKw&hl=en_GB&fs=1&"></param>
      <param name="allowFullScreen"
        value="true"></param>
      <param name="allowscriptaccess"
        value="always"></param>
      <embed src="http://www.youtube.com/v/9sEI1AUFJKw&hl=en_GB&fs=1&"
        type="application/x-shockwave-flash" allowscriptaccess="always"
        allowfullscreen="true" width="425"
        height="344"></embed>
    </object>

!SLIDE
#HTML5 VIDEO

!SLIDE smaller

    @@@html
    <video src="movies/example.ogg"/>

!SLIDE
##IDEAL

!SLIDE
##REAL

!SLIDE smaller

    @@@html
    <video>
        <source src="/example.ogg" type="video/ogg"/>
        <source src="/example.mp4" type="video/mp4"/>
    </video>

!SLIDE
##OPTIONS

!SLIDE smaller
##FALLBACK CONTENT
    @@@html
    <video src="/movies/example.ogg">
        Download the <a href="/movies/example.ogg">video</a>.
    </video>

!SLIDE smaller
##DIMENSIONS
    @@@html
    <video src="/movies/example.ogg"
        width="480"
        height="360">
        Download the <a href="/movies/example.ogg">video</a>.
    </video>

!SLIDE smaller
##POSTER FRAME
    @@@html
    <video src="/movies/example.ogg"
        width="480"
        height="360"
        poster="/poster/example.jpg">
        Download the <a href="/movies/example.ogg">video</a>.
    </video>

!SLIDE smaller
##AUTOBUFFER
    @@@html
    <video src="/movies/example.ogg"
        width="480"
        height="360"
        poster="/poster/example.jpg"
        autobuffer>
        Download the <a href="/movies/example.ogg">video</a>.
    </video>
