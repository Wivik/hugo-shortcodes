# Mastodon Toot integration

## Usage

This shortcode will convert `{{<toot link="https://mastodon.instance/thetoot">}}` into this :

```html
<div style="text-align:center;">
<iframe src="{{ $link }}/embed" class="mastodon-embed" style="max-width: 100%; border: 0" width="400" allowfullscreen="allowfullscreen"></iframe><script src="https://mastodon.instance/embed.js" async="async"></script>
</div>
```

Example :

```golang
{{<toot link="https://fosstodon.org/@Wivik/107645377769254953">}}
```

Will render :

![toot](toot.png)

## Install

Copy the content of the `shortcodes/` folder into on of these folders (order by Hugo's precedence):

1. `/layouts/shortcodes/toot.html`
2. `/themes/YOURTHEME/layouts/shortcodes/toot.html`

