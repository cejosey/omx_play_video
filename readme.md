# omx_play_video

I made this little script to play web videos full screen using OMX player on the Raspberry Pi.

It uses youtube-dl to download the video into a buffer then to a fifo stream file
which OMX player then reads and plays.

Add the play_video.desktop file to your ~/.local/share/applications/ folder, then copy
play_video into /home/pi/bin/play_video and add a shortcut to the Pi
taskbar launcher.

To use it open the page with the video in your favorite brower.  Then copy the
URL to the clipboard and click the launcher.  It will open a terminal, start
the download, and play the video fullscreen in OMX player.  Be patient,
there is a 15 second delay to allow youtube-dl to start the download and to
buffer a bit.
