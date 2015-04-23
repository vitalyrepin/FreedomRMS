How to work with subtitles:

- Install subtitle editor gna: http://home.gna.org/subtitleeditor/
- Install wget utility: https://www.gnu.org/software/wget/
- Check that theora videos are supported by your gstreamer (e.g., you should have gst-plugins-theora ebuild installed if you are Gentoo user)

Files of every week are located in the corresponding directory:

- Intro: Introduction video
- W1: Week 1
- W2: Week 2
- W3: Week 3
- W4: Week 4
- W5: Week 5

In order to begin to work on subtitles you need to download videos first. Go to the directory which corresponds to the proper week and issue command "make".
It will download all the videos to your local file system.

Every directory has the following files:

- Video files (*.ogv)
- Waveform files (*.wf) and keyframe files (*.kf): needed by gna.
- gna project file (one file for each video file, file extension is "xml")
- Subtitle files (*.srt) SubRip format. One subtitle file for each video file. Suffixes are language codes. E.g., "IntroRMS-en.srt" - English subtitles for the IntroRMS.ogv video file. Make sure to keep this convention when you are adding new subtitle file!

How to start creating subtitles with gna: http://home.gna.org/subtitleeditor/docs/how-to-editing-subtitles-with-waveform.html

