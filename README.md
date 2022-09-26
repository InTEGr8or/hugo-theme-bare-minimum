# Bare Minimum

I think a menu is required for a bare minimum, so I have included

``` html
<div class="sidebar">
    {{- partial "open-menu.html" . -}}
</div>
```
## Understanding Hugo Templates and Themes

I've been working with Hugo templates for a few years, but it has been sporadic. One of the selling-points of Hugo is that it's a low on-ramp to creating a full-functioning static website. It has a lot of nice features, like being able to construct a richly structured static site by simply using Markdown files structured inside folders. That allows a wide veriety of content types, like images, PDF, csv, Mermaid, etc, just by editing ASCII files and puting content in folders.

Some of the structure, however, depends on the theme you are using, and making ad-hoc changes to themes is not as simple and straight-forward as I would like it to be.

There is an overlap between `{{ partial "file.html" . }}` and `{{ block "model" . }}` that is not obvious or clear. Anyone working with templates should have a very clear understanding about how those imports differ and which is better in which cases.

The best way to discover that structural difference is to try a bunch of variations while building up from the bottom.

That's what this minimal theme is for.

The `main` branch should remain the most minimal usable branch.

I will then add features like SEO, fonts, and a veriety of RAD structural elements into the other branches.

My hope is that we will be able to _compose_ richer solutions by merging multiple branches into the `main` branch to create new, more extensive themes.