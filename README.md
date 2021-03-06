sh
==

Random shell scripts.

### change-audio

I have two sets of available speakers -- a desktop set, and the speakers on my TV (via HDMI). Switching locations means going into KDE's audio settings and clicking some things. I wanted a convenient way to switch which speakers were active. So 'change-audio TV' moves everything to the TV, and 'change-audio desktop' moves everything to the desktop.

### change-desktop

This is what I use to overcome the fact that KDE has no reliably useful way to change your desktop background from the command line for 2 monitors.

Basically, I set the desktop background for each monitor to a slideshow for a set directory (/wallpapers/slide/L/ and /wallpapers/slide/R/). Then I run this script to copy from my main wallpaper directory into each of those directories, constantly overwriting a single file (L.jpg and R.jpg). I mostly just run `change-desktop rand` which will choose one at random, but it is also set up to specify the wallpaper slug, e.g. `change-desktop adventure-time` which will copy adventure-time-L.jpg and adventure-time-R.jpg into the appropriate spots.

### clementine-controller

Example script to show how to add a randomly chosen playlist to the current queue of Clementine (music player) and start it. 

### episode-namer

Parses a directory containing episodes of some season of some show, scrapes IMDB to grab the episode titles, and renames all the files in order to the format SXXEYY - Episode Title.

### listsinks / movesinks

Borrowed from here: http://askubuntu.com/questions/71863/how-to-change-pulseaudio-sink-with-pacmd-set-default-sink-during-playback

### mp4ify

Convert any random video format to mp4 using avconv.

### random-episode

This is my tool to deal with the fact that I don't have a paid cable subscription and miss the ease of plopping down in front of the TV and having something random play on its own. It basically just chooses a random episode from my TV directory, although you can also specify a show (`random-episode futurama`) or a type of show (`random-episode cartoons`), and opens it with VLC.

### timelapse

Use in a directory of sequential images to generate a timelapse movie. For example, `timelapse -o output.mp4 -f 36` for a 36 fps movie. Requires zeropad.

### video-highlights

I made this to create highlight videos of NFL and NBA games. Input a video file, specify an output file, start time offset, duration and period of the highlights, and a highlight video will be produced. Works only for MP4 at the moment.

### video-summary

Creates an image that includes metadata about a video and tiled screengrabs at regularly spaced intervals.

### video-thumb

Creates a thumbnail of a video by grabbing a frame about halfway through.

### zeropad

Used for renaming files. Borrowed from here: http://stackoverflow.com/questions/5417979/batch-rename-sequential-files-by-padding-with-zeroes
