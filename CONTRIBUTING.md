# Intel® IoT Getting Started Docs Contribution Guide

We welcome pull requests and bug reports on these docs.

**For minor typos and edits:** Fork this repo, make your edits on your local computer or [directly on Github](https://help.github.com/articles/editing-files-in-your-repository/), then [submit a PR](https://help.github.com/articles/using-pull-requests/).

**For larger updates:** Start a ticket in the Github issue tracker to let us know what you are working on. This will allow others to provide feedback as well as coordinate contribution efforts.

## Markdown files

All content (with a few exceptions) are written in Markdown, mixed with some HTML. The flavour of Markdown used by the current Jekyll templating system is 'kramdown'.

### Templating

All content files (found in the 'docs' folder) must start with a snippet like this:

```
---
layout: default
title: Getting Started
---
```

### Headings

Headings get `id` attributes automatically generated for them. To create a table of contents, wrap it in a `div` with `id="toc" class="box" markdown="1"`. Setting `markdown="1"` means that you can write markdown within the html block. An example Table of Contents:

```
<div id="toc" class="box" markdown="1">
* [Install Intel® Edison standalone drivers »](#install-intel-edison-standalone-drivers)
* [Install FTDI serial drivers »](#install-ftdi-serial-drivers)
* [Restart your computer »](#restart-your-computer)
</div>
```

### Videos

Let's comment out videos for now but eventually they will look be embedded on the page with width="565" and height="367". For example:

```
<div id="related-videos" class="callout video">
  <object id="flashObj" width="565" height="367" ...
  <embed ... name="flashObj" width="565" height="367" ...></embed></object>
</div>
```

### TLDR summary

The html for summary boxes for each section (with the blue roadsign icon, which I call the "Too long, didn't read" box) look like this:

```
<div class="tldr" markdown="1">
Some 1-2 sentence blurb
</div>
```

### Callout boxes

The html for other callboxes boxes look like this:

```
<div class="callout info" markdown="1">
**Bolded Title (optional)**

Some stuff.
</div>
```

Or when there are multiple items, use a horizontal rule to divide them.

```
<div class="callout info" markdown="1">
**First Title**

First thing

---

**Second Title**

Second thing
</div>
```

Check the CSS file for final callout box options but so far they are:

* info
* goto
* troubleshooting
* done
* warning
* danger


### Next steps

The closing (blue) box at the bottom of the page has this markup:

```
<div id="next-steps" class="note" markdown="1">
Link with where to go next
</div>
```


## Style Guide

Many of these docs originated as a Google Doc and PDFs. Some of the points in the [original style guide](https://docs.google.com/document/d/1C-UeNNmMEX-wXcJLTrflbCm_L93bq3g0aa2CTHNf6Aw/preview) may not apply to these Markdown docs but still worth a read. 

### Language

* Explain what **and why** but keep it short and sweet.
* Keep "skimmability" in mind at all times. No one reads every word so make important ones **jump** out using bold or italics.
* Use numbered lists and bullet points. Avoid rambling in paragraphs.
* Make the content impersonal, gender neutral, and action-oriented -- this content is meant to be re-used across different mediums and platforms. Jokes do not translate well.

### Images

* **Show, don't tell**: Add screenshots and/or photos for clarity.
* However, having said that, even when using an image **do not leave out text-based instructions** for accessibility reasons.
* For ease of translation, do not put text overlays in images. Use numbered or lettered captions, if necessary.
* To show an action, put together a before & after montage or consider an [animated gif](https://github.com/vvo/gifify).
* Use #ff8c00 orange for callout arrows and circles. (Avoid #e21f20 red callouts unless it is actually an indication of an error or danger.)
* Crop images to bring extra attention to the important area and to save space — but make sure to keep context (ie. don't overcrop).
* Compress your images before adding to the repo. Try [TinyPNG](https://tinypng.com/) or similiar tools.

### Command line input

* Make commands that a reader needs to type jump out and easy to copy/paste by using a single backtick (\`) or [triple backticks](https://help.github.com/articles/github-flavored-markdown/#fenced-code-blocks) (```) for multiple lines.

### Code samples

* Make code easy to copy/paste -- use [triple backticks](https://help.github.com/articles/github-flavored-markdown/#fenced-code-blocks) (```) for code blocks.
* 2 spaces (not tabs)

## Possible additions

### Want to add a new breakout board?

1. Add it to the main [README.md](README.md)
2. Create a sub-folder in the [assembly folder](/assembly) for the new board
  * Create a doc for **assembly**
  * And another **connecting_cables** doc that is more like an appendix
3. Create an end-to-end guide in the [START_HERE folder](START_HERE/) for some basic Hello World app

### Want to add a new sensor kit?

1. Create a sub-folder in the [sensor examples folder](/sensor_examples) for the new kit
  * Create an **intro** doc
  * Put code samples into a language specific folder (since there will likely be different screenshots/gifs/videos for different languages)

---

## Questions or concerns?

Please file a ticket in the Github issue tracker. The Intel® IoT team want these to be the best docs out there so don't be shy. Please follow the [Contributor Code of Conduct](CODE_OF_CONDUCT.md)
