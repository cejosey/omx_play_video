# omx_play_video

I made this little script to play web videos full screen using OMX player on the Raspberry Pi.

It uses youtube-dl to get the video URL which OMX player then reads and plays.  As
long as the website is supported by youtube-dl this should work.

Add the play_video.desktop file to your ~/.local/share/applications/ folder, then
add a shortcut to the Pi taskbar launcher.

Copy play_video into /home/pi/bin/play_video.

To use it open the page with the video in your favorite brower.  Then copy the
URL to the clipboard and click the launcher.  It will open a terminal, get the URL
and play the video fullscreen in OMX player.

