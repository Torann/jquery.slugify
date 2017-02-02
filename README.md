# jQuery Slugify

Yet another url slug creation plugin for jQuery.

## Getting Started

You can install the plugin using Bower:

```bash
bower install jquery.slugify
```

The script will automatically create the slug from the inputted data from element (source) with the `data-slugify` attribute, and add it to the element (target) specified in the `data-slugify` attribute. You can also setup an URL preview by adding an element ID or classname in the `rel` tag on the target element.

```html
<script src="jquery.js"></script>
<script src="jquery.slugify.js"></script>

<div class="form-group">
    <label for="post-title">Title</label>
    <input id="post-title" type="text" value="" name="title" data-slugify="#post-slug">
</div>

<div class="form-group">
    <label for="post-slug">Slug</label>
    <input id="post-slug" type="text" value="" name="slug" rel="#post-slug-preview">

    <span class="help-block">
        /blog/<span id="post-slug-preview"></span>
    </span>
</div>
```