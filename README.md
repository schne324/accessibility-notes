Accessibility Notes
===================

**Key:**
- VO: _Voice Over_ (paired with Safari)
- NVDA: _NonVisual Desktop Access_ (paired with FireFox or _FF_)
- JAWS: _Job Access With Speech_ (paired with Internet Explorer or _IE_)
- (mdn): Mozilla Developer Network (resource) - https://developer.mozilla.org/en-US/


## aria-describedby

"The aria-describedby attribute is used to indicate the IDs of the elements that describe the object. It is used establish a relationship between widgets or groups and text that described them" (mdn)

- tooltips
- error messages

__*AT Notes*__

example:

```
<div id="tooltip">this is a tooltip</div>
<input type="text" id="tooltip-target" aria-describedby="tooltip" \>
```

## aria-labelledby

"aria-labelledby can be used in conjunction with the <label> element (using the for attribute) to improve compatibility with user agents that do not yet support ARIA." (mdn)

- labelledby can be used in conjunction with a label element
example:

```
<div id="radio_label">My radio label</div>
<ul role="radiogroup" aria-labelledby="radio_label">
    <li role="radio">Item #1</li>
    <li role="radio">Item #2</li>
    <li role="radio">Item #3</li>
</ul>
```

##aria-label

- Supported by Jaws in most cases
- NOT supported by NVDA

## aria-hidden=true

- Can be used to hide visible content to screen readers
(http://www.456bereastreet.com/archive/201205/hiding_visible_content_from_screen_readers_with_aria-hidden/)

##aria-controls
- only supported by Jaws

## \<label "for"\> vs. \<input "title"\>

Chrome w/ChromeVox

- `for` only: only the label content is read.
- `for` & `title`: only the label contents are read.
- `title` only: only the "title" attribute is read.

Firefox w/NVDA & Internet Explorer w/JAWS

- `for` only: only the label content is read.
- `for` & `title`: first the label contents, then the "title" are read.
- `title` only: only the "title" attribute is read.

Safari w/Voiceover

- `for` only: only the label content is read.
- `for` & `title`: first title contents, then the label contents are read.
- `title` only: only the "title" attribute is read.

##Click events with JAWS and NVDA

JAWS

- The `Enter` key by itself will not trigger click events on focusable elements
- Instead, use `Shift + Enter`

NVDA

- The `Enter` key by itself will not trigger click events on focusable elements
- Instead, use `NVDA key` (often caps-lock) `+ Enter`

##Keyboard events with JAWS and NVDA

JAWS

- To access default arrow key behavior (i.e. within a datepicker), press *control + window + {arrow key}*

NVDA
- To access default arrow key behavoir (i.e. within a datepicker), press *control + shift + alt + {arrow key}*
