# Using HTML5 audio and video

HTML5 introduces built-in media support via the `<audio>` and `<video>` elements, offering the ability to easily embed media into HTML documents.

## **Embedding media**

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



This code example uses attributes of the [`<audio>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio "The HTML <audio> element is used to embed sound content in documents. It may contain one or more audio sources, represented using the src attribute or the <source> element; the browser will choose the most suitable one.") element:

* `controls` : Displays the standard HTML5 controls for the audio on the web page.
* `autoplay` : Makes the audio play automatically.
* `loop` : Make the audio repeat \(loop\) automatically.

