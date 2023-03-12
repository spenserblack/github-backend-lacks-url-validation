# GitHub's Backend lacks website URL validation

The input field for the repository's website URL is
```html
<input type="url">
```
which tells the browser to enforce a valid URL in the input.
But a quick usage of inspect element allows you to input a
much wider range of values.

There are *some* limitations. When attempting to put the
Jack O' Lantern emoji (🎃), I discovered that characters
with codes greater than `0xFFFF` aren't allowed.
