Accessibility Notes
===================

**Key:**
- VO: _Voice Over_ (paired with Safari)
- NVDA: _NonVisual Desktop Access_ (paired with FireFox or _FF_)
- JAWS: _Job Access With Speech_ (paired with Internet Explorer or _IE_)

## aria-describedby

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


##aria-label

- Supported by Jaws in most cases
- NOT supported by NVDA
