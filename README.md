Styled hint blocks in your docs
==============

This plugins requires gitbook `>=2.0.0`.

### Install

Add the below to your `book.json` file, then run `gitbook install` :

```json
{
    "plugins": [ "hints" ]
}
```

### Usage

You can now provide hints in various ways using the `hint` tag.

```markdown
{% hint style='info' %}
Important info: this note needs to be highlighted
{% endhint %}
```
The above example will produce a styled alert, with an icon:

``` html
<div class="alert alert-info hints-alert">
  <div class="hints-icon"><i class="icon-info"></i></div>
  <div class="hints-container">
    <p>Important info: this note needs to be highlighted</p>
  </div>
</div>
```

Available styles are:

- `danger`
- `info` (default)
- `success`
- `warning`
