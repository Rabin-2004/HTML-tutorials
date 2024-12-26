
## Using Multiple Source Formats
Different browsers support different video formats. To improve compatibility, use multiple source formats:
```html
<video controls>
    <source src="rabbit320.mp4" type="video/mp4" />
    <source src="rabbit320.webm" type="video/webm" />
    <p>Your browser doesn't support this video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
In the above code snippet the type attribute defines the type and format of the video which specifies which media format the media is in

### Key Points
- **Container Formats**: Define the structure of media files (e.g., MP3, MP4, WebM).
- **Codecs**: Compress audio and video into manageable files.
- **Browser Support**: Different browsers support different codecs and container formats.

## Media File Support in Browsers
Popular formats like MP3 and MP4/H.264 are encumbered by patents, requiring browsers to pay license fees. To ensure compatibility, provide media files in multiple formats.

### Choosing the Right Format
- Consider the target audience and platforms.
- Use multiple formats to maximize compatibility.

### Example
```html
<video controls>
    <source src="rabbit320.mp4" type="video/mp4" />
    <source src="rabbit320.webm" type="video/webm" />
    <p>Your browser doesn't support this video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
