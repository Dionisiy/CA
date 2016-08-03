# Using HTML5 audio and video

HTML5 introduces built-in media support via the `<audio>` and `<video>` elements, offering the ability to easily embed media into HTML documents.

# **Embedding media**

Embedding media in your HTML document is trivial:

```
<video src="url" controls>
  Your browser does not support the <code>video</code> element.
</video>
```

This example plays a sample video, with playback controls.

Here is an example for embedding _audio_ into your HTML document

```
<audio src="/test/audio.ogg">
<p>Your browser does not support the <code>audio</code> element.</p>
</audio>
```

The `src` attribute can be a URL of the audio file or the path to the file on the local system.

This code example uses attributes of the `<audio>` element:

* `controls` : Displays the standard HTML5 controls for the audio on the web page.
* `autoplay` : Makes the audio play automatically.
* `loop` : Make the audio repeat \(loop\) automatically.

Multiple source files can be specified using the `<source>` element in order to provide video or audio encoded in different formats for different browsers. For instance:

```
<video controls>
  <source src="SampleVideo.ogv" type="video/ogv">
  <source src="SampleVideo.mp4" type="video/mp4">
  Your browser does not support the <code>video</code> element.
</video>
```

Controlling an HTML5 audio player to play, pause, increase and decrease volume using some Javascript is straightforward.



[See the code](https://denishromenko.gitbooks.io/codeacademy_doc/content/html_structure_using_lists/external-ex.html)

