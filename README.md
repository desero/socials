# socials
Social icons

## Preview
Open **demo.html** to see a list of all the glyphs in your font along with their codes/ligatures.

## Usage
HTML
```html
<div class="social-container">
  <ul class="nav social-links-nav">
    <li><a href="#" target="_blank" title="Follow us on Facebook"><span class="icon icon-facebook"></span></a>
    </li>
    <li><a href="#" target="_blank" title="Follow us on Twitter"><span class="icon icon-twitter"></span></a>
    </li>
    <li><a href="#" target="_blank" title="Follow our RSS feed"><span class="icon icon-rss"></span></a>
    </li>
    <li><a href="#" target="_blank" title="Follow our Mail RSS feed"><span class="icon icon-mail"></span></a>
    </li>
    <li><a href="#" target="_blank" title="Follow us on YouTube"><span class="icon icon-youtube"></span></a>
    </li>
    <li><a href="#" target="_blank" title="Follow us on GooglePlus"><span class="icon icon-googleplus"></span></a>
    </li>
  </ul>
</div>
```

Sass
```sass
.social-links-nav {
  // include some clear fix helper here
  // @include cf;
  li {
    float: left;
  }
  a {
    display: block;
  }
  $icons-set: (
    'facebook',
    'twitter',
    'rss',
    'mail',
    'youtube',
    'googleplus'
  );
  @each $icon in $icons-set {
    .icon-#{$icon} { @include social-icon-before($icon); }
  }
}
```
