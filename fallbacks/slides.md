!SLIDE
# FALLBACKS

!SLIDE
## FLASH CAN PLAY H.264

!SLIDE smaller

    @@@html
    <video>
        <source src="/example.ogg" type="video/ogg"/>
        <source src="/example.mp4" type="video/mp4"/>

        <object width="425" height="344">
          <param name="movie"
            value="/example.mp4"></param>

            ...[ghastly markup elided]...

        </object>

    </video>

!SLIDE bullets small incremental
##VIDEO FOR EVERYBODY

* use \<video\> where supported
* fallback to flash
* do not require javascript
* [http://camendesign.com/code/video_for_everybody](http://camendesign.com/code/video_for_everybody)

!SLIDE smaller

    @@@html
    <!-- "Video For Everybody" v0.3.3
         =================================================================================================================== -->
    <!-- first try HTML5 playback. if serving as XML, expand `controls` to `controls="controls"` and autoplay likewise -->
        <video width="640" height="360" poster="__POSTER__.JPG" controls>
            <!-- MP4 must be first for iPad! you must use `</source>` to avoid a closure bug in Firefox 3.0 / Camino 2.0! -->
            <source src="__VIDEO__.MP4" type="video/mp4"><!-- Safari / iPhone video    --></source>
            <source src="__VIDEO__.OGV" type="video/ogg"><!-- Firefox native OGG video --></source>
            <!-- IE only QuickTime embed: IE6 is ignored as it does not support `<object>` in `<object>` so we skip QuickTime
                 and go straight to Flash further down. the line break after the `classid` is required due to a bug in IE -->
            <!--[if gt IE 6]>
            <object width="640" height="375" classid="clsid:02BF25D5-8C17-4B23-BC80-D3488ABDDC6B"><!
            [endif]-->
            <!-- non-IE QuickTime embed (hidden from IE): the self-closing comment tag allows non-IE browsers to
                 see the HTML whilst being compatible with serving as XML -->
            <!--[if !IE]><!-->
            <object width="640" height="375" type="video/quicktime" data="__VIDEO__.MP4">
            <!--<![endif]-->
            <param name="src" value="__VIDEO__.MP4" />
            <param name="showlogo" value="false" />
            <param name="autoplay" value="false" />
            <!-- fallback to Flash -->
            <object width="640" height="384" type="application/x-shockwave-flash"
                data="__FLASH__.SWF?image=__POSTER__.JPG&amp;file=__VIDEO__.MP4">
                <!-- Firefox uses the `data` attribute above, IE/Safari uses the param below -->
                <param name="movie" value="__FLASH__.SWF?image=__POSTER__.JPG&amp;file=__VIDEO__.MP4" />
                <!-- fallback image. download links are below the video. warning: putting anything more than
                     the fallback image in the fallback may trigger an iPhone OS3+ bug where the video will not play -->
                <img src="__POSTER__.JPG" width="640" height="360" alt="__Title of video__"
                     title="No video playback capabilities, please download the video below"
                />
            </object><!--[if gt IE 6]><!-->
            </object><!--<![endif]-->
        </video>

