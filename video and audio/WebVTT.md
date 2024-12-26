# WebVT file format (.vtt file extension)
WebVTT is a format for writing text files containing multiple strings of text along with metadata such as the time in the video at which each text string should be displayed, and even limited styling/positioning information. These text strings are called cues, and there are several kinds of cues which are used for different purposes. The most common cues are:

subtitles
Translations of foreign material, for people who don't understand the words spoken in the audio.

captions
Synchronized transcriptions of dialog or descriptions of significant sounds, to let people who can't hear the audio understand what is going on.

timed descriptions
Text which should be spoken by the media player in order to describe important visuals to blind or otherwise visually impaired users.

File example: 

WEBVTT

1
00:00:22.230 --> 00:00:24.606
This is the first subtitle.

2
00:00:30.739 --> 00:00:34.074
This is the second.

…

## Key Features:
- Header (WEBVTT): The file starts with the keyword WEBVTT.

- Timestamps: Timestamps specify when each caption should appear and disappear. The format is:
hours:minutes:seconds.milliseconds --> hours:minutes:seconds.milliseconds.

- Text: The text following a timestamp is displayed as a caption.

- Empty Line: Each block of captions is separated by an empty line.

## Optional Features

- Cue Identifiers:
Optional identifiers placed before the timestamps to name or number cues.
eg :
<pre>
1
00:00:01.000 --> 00:00:05.000
Welcome to our video.
</pre>
Here 1 is the cue identifier.

- Positioning and Styling:
Cue settings allow alignment, positioning, or styling.
eg:
<pre>
00:00:01.000 --> 00:00:05.000 position:10%,line:90% align:left
Welcome to our video.
</pre>

- Metadata Blocks:
Notes or comments begin with NOTE and are ignored by the player.
Example:
<pre>
NOTE This is a comment.
</pre>

## Intergration in HTML file (with `<video>` or `<audio>` files)
```
<video controls>
  <source src="video.mp4" type="video/mp4">
  <track src="subtitles.vtt" kind="subtitles" srclang="en" label="English">
</video>
```
