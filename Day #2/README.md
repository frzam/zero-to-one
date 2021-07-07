# Day 2
## CSS (Style Sheets)
> A list of css rules or rule set

It has two components:
* **Selector:** The element/elements properties should be applied to.
* **Declaration:** Key value pair while defines the actual property and its value.

```CSS
div{
  color: red;
  margin: 20px;
}
h2{
  font-style: italic;
}
```

Here div and h2 are Selector and color and margin entries are the Declarations or property values.

There are three ways to apply css to any HTML document.
1. **Inline:** by using the style attribute inside HTML element.
2. **Internal:** by using the `<style>` element in the head section.
3. **External:** by using a link element to link to an external css file.

Generally external CSS is used and considered a best practice.

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Day #2</title>
    <!-- Internal CSS -->
    <style>
      h1{
        color: orange;
      }
      p{
        color: grey;
      }
      body{
        text-align: center;
        background-color: #bde38d
      }
    </style>
  </head>
  <body>
    <h1>CSS Tutorial</h1>
    <div class="about">
      <h2>About</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur ac semper orci. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Aenean mattis libero vitae eleifend efficitur. In at scelerisque metus, id viverra felis. Cras gravida dui sit amet urna lacinia, nec faucibus nibh venenatis. Suspendisse in ipsum ullamcorper ex auctor lobortis vitae non ex. Sed at justo eros. Maecenas quis neque purus.</p>
      <p>Aliquam erat volutpat. Sed venenatis orci venenatis metus dapibus feugiat. Vestibulum viverra semper urna nec tincidunt. Donec ultricies commodo justo, ac ornare ligula vulputate a. Proin luctus nulla id ultricies consequat. Aliquam erat volutpat. Proin eu mauris sit amet massa aliquet consequat ut a risus. Vestibulum ultrices dui at quam imperdiet, ac fringilla mauris elementum. Donec pellentesque pellentesque blandit.</p>
    </div>
    <div class="thanks">
      <h2>Thanks</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas quis risus in massa sagittis tincidunt. Aliquam enim magna, varius sit amet ante ut, rutrum vulputate orci. Integer in pellentesque nisl, et scelerisque arcu. Donec sem magna, blandit in auctor facilisis, aliquam nec erat. Vivamus vel libero rhoncus, sodales turpis in, bibendum libero. Nullam pulvinar lorem vel ante feugiat, auctor interdum justo rhoncus. Nulla congue quis est quis ullamcorper.</p>
    </div>
  </body>
</html>
```
If one element has css property defined at attribute level than it will override external css property. Though rules are little complex and not part of these sessions.
