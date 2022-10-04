## TOC
1. [TOC](#toc)
2. [What is SVG](#what-is-svg)
3. [Why use SVG](#why-use-svg)
  1. [When not to use SVG](#when-not-to-use-svg)
  2. [Devsign alternative](#devsign-alternative)
4. [Using SVG](#using-svg)
  1. [Inner workings](#inner-workings)
  2. Including SVG
  3. Manipulating SVG

## What is SVG 
## Why use SVG

### When not to use SVG
   [Shapes of css](https://css-tricks.com/the-shapes-of-css/)
### Devsign alternative

## Using SVG

### Inner workings

When looking at a SVG file in an editor/IDE, you'll find a familiar to HTML. This is because both are based on XML (Extensible Markup Language), SVG is, essentially, to graphics what HTML is to text.

They follow the same rules for structure, being comprised of elements that have attributes, including things like `id` and `class`. The main difference comes from the [elements](https://developer.mozilla.org/en-US/docs/Web/SVG/Element) available.
So instead of paragraphs and headers you will have things like circles and paths, for example:

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <path
    d="
      M 10,30
      A 20,20 0,0,1 50,30
      A 20,20 0,0,1 90,30
      Q 90,60 50,90
      Q 10,60 10,30 
      z
    "
  />
</svg>
```
The `d` attribute here takes a series of [Path Commands](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/d#path_commands), which results in the following shape:

### Including SVG

SVGs can be used in HTML/JSX in the same way as other types of images:

```html
<img src="/path/to/image.svg" alt="SVG as an image">
```

As well as in CSS (and its pre-processors) as a background image:

```css
figure {
  background-image: url["/path/to/image.svg"];
}
```

While it is simple to add a svg file this way, it does not allow you to customise the svg as it will just be loaded in as a static resource.



- [React](https://blog.logrocket.com/how-to-use-svgs-in-react/)
- [Angular](https://angular.io/guide/svg-in-templates)
- [Vuejs](https://dev.to/jacqueline/using-svgs-in-vuejs-made-simple-2e1a)