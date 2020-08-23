# Marcokai - a listed.to blog theme

Marcokai is a combination of _Marco's_ dark blog theme and modified monokai code highlighting.
The theme can be used as is or modify elements to make the site your own!
See the install and customize sections for how to use and remix, check out contributing section to provide changes.

# Install

This theme can be installed one of two ways.
The recommended way is to import this stylesheet into your blog.
By importing the theme it means you'll get the latest bug fixes and tweaks and will be supported by the latest listed.to markup.
It will also provide you with an easy way to remix the theme by allowing you to modify elements with your own flair!
Make sure you've already create a listed.to account and linked it to your Standard Notes account.

## CSS Import

If you haven't already, create a new note titled `theme.css` and set the editor to `Plain Editor`.

Copy and paste the following code snippet:

```
---
metatype: css
---

@import url(https://marcoceppi.github.io/listed-marcokai/dist/marcokai.min.css);
```

Now publish the post as a Private Post and refresh your listed.to author page!

## Copy / Pasta

If you don't want automatic updates, and wish to instead use this as a base just copy and paste everything in [`marcokai.css`](/src/marcokai.css) while following [these instructions](https://docs.standardnotes.org/listed/styles#to-stylize-your-blog-with-custom-css)

# Remixing

Marcokai is meant to be a base theme.
What's great about listed's site format is you can override any of the CSS by adding blocks of CSS code after the `@import` line.
For example, make all the links pink:

```css
---
metatype: css
---

@import url(https://marcoceppi.github.io/listed-marcokai/dist/marcokai.min.css);

:root {
  --link-color: #f92672;
}
```

Or, perform some more nuianced changes, like instead of the typical `⋮` between Listed and your blog name (or the `>` that Marcokai inserts) you can make it whatever you'd like:

```css
---
metatype: css
---

@import url(https://marcoceppi.github.io/listed-marcokai/dist/marcokai.min.css);

#page-header .left .path-item:before {
  content: "≡";
}
```

# Contributing

If you've made it this far you might be interested in helping maintain this little listed theme!
There are several ways to help out the project:

* [Open a Github Issue with a bug, feature, or question](https://github.com/marcoceppi/listed-marcokai/issues)!
  Often times just informing of bugs, or asking to support newer extensions, or even asking for help can make all the difference.
  If you're asking, or seeing an issue, there's a good chance someone else is - being the first to ask will save many in the future.
* [Opening a pull request](https://github.com/marcoceppi/listed-marcokai/network/members)!
  Contributing back code to keep this project alive is much appreciated.
  Personally, this is my listed theme so helping keep it working is :100:, but it will also help out all those who are using it as a base.
  While not required, it's preferable to have pull requests organized to a single commit and linked to an existing issue.
  However, we won't turn away contributions for bureaucracy!
* Star & Watch!
  It may not seem like much, but watching the repo & answering issues or just giving a star go a long way for small open source projects like these.
