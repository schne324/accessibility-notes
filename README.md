Accessibility Notes
===================

## aria-describedby

- tooltips
- error messages

example:
```
<div id="tooltip">this is a tooltip</div>
<input type="text" id="tooltip-target" aria-describedby="tooltip" \>
```

## aria-labelledby
"aria-labelledby can be used in conjunction with the <label> element (using the for attribute) to improve compatibility with user agents that do not yet support ARIA." (mdn)

- this can often times replace the desired behavior of a fieldset/legend markup scheme
example:
```
<div id="radio_label">My radio label</div>
<ul role="radiogroup" aria-labelledby="radio_label">
    <li role="radio">Item #1</li>
    <li role="radio">Item #2</li>
    <li role="radio">Item #3</li>
</ul>
```
