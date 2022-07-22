---
title: "Render hooks"
date: 2022-07-20T08:25:17-08:00
draft: false
type: render-hooks
menu: main
---
Default render hook templates are places in `layouts/_default/_markup/render-[element].html`. Render hook templates examples for this page have been placed in `layout/render-hooks/render-[element].html` because `type: render-hooks` has been set in the front matter above. Hugo will then look in the `layouts/render-hooks` directory before `layouts/_default`.

### Heading 3 {.custom-class-1 .custom-class-2 #custom-id aria-title="3rd level heading"}

[Link Text](www.google.com/ "Link Title")

![Alt Text](/img/image1.jpg "Title Text")

Code block which inherits the default render hook template for code blocks:

```js
function test() {
  // comment
}
```

Html Code block with custom attributes and highlight settings:

```html {#custom-id .custom-class .class2 translate="no" style="colorful"}
<div>sample code block</div>
<em>with the colorful style and custom html id</em>
```

CSS code block with options set as inline attributes, and hard coded in the render hook template:

```css {style="colorful"}
.hidden-class {
  display: none;
}
```
