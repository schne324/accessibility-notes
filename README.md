Accessibility Notes
===================

**Key:**
- VO: _Voice Over_ (paired with Safari)
- NVDA: _NonVisual Desktop Access_ (paired with FireFox or _FF_)
- JAWS: _Job Access With Speec_ (paired with Internet Explorer or _IE_)

## aria-describedby

- tooltips
- error messages

__*AT Notes*__
- VO: if an element has multiple aria-describedby values only the first will be read out (ex: aria-describedby="id1 id2" only id1's content will be read out)



example:

```
<div id="tooltip">this is a tooltip</div>
<input type="text" id="tooltip-target" aria-describedby="tooltip" \>
```

## aria-labelledby
"aria-labelledby can be used in conjunction with the <label> element (using the for attribute) to improve compatibility with user agents that do not yet support ARIA." (mdn)

- lablledby can be used in conjunction with a label element
example:

```
<div id="radio_label">My radio label</div>
<ul role="radiogroup" aria-labelledby="radio_label">
    <li role="radio">Item #1</li>
    <li role="radio">Item #2</li>
    <li role="radio">Item #3</li>
</ul>
```
