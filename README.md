Styled hint blocks in your docs
==============

This plugins requires gitbook `>=2.0.0`.

### Install

Add the below to your `book.json` file, then run `gitbook install` :

```json
{
    "plugins": ["hints"]
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
  <div class="hints-icon"><i class="fa fa-info"></i></div>
  <div class="hints-container">
    <p>Important info: this note needs to be highlighted</p>
  </div>
</div>
```

Available styles are:

- `info` (default)
- `tip`
- `danger`
- `working`

### Configuration

You can specify custom classes for the icons (or none) in your `book.json`:

```json
{
    "plugins": ["hints"],
    "pluginsConfig": {
        "hints": {
            "info": "fa fa-info-circle",
            "tip": "fa fa-mortar-board",
            "danger": "fa fa-exclamation-cicle",
            "working": "fa fa-wrench"
        }
    }
}
```
