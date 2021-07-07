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
    <p>Block Level element Paragraph</p>
    <a href="#">In line element a</a>
  </body>
</html>
```
If one element has css property defined at attribute level than it will override external css property. Though rules are little complex and not part of these sessions.

```CSS
h1{
  color: orange;
  text-decoration: underline;
}

div{
  border-style: solid;
}

p{
  color: grey;
  font-size: 20px;
  border-style: solid;
 column-count: 3;
  letter-spacing: 2px;
}
body{
  text-align: center;
}
a{
  border-style: solid;
}
/* */
.about{
  color: red;
  background-color: pink;
}
 .error{
  color: red;
}
p.error{
  color: red;
}

#content{
  background-color: lightgray;
}


```

**Inline Elements**
1. They line up next to each other.
2. Don't take more room than there contents need.
3. ex `<img>`, `<span>`, `<a>` , `<strong>` etc

**Block level Elements**
1. They do not sit side by side.
2. They take width of the page regardless of the content.
3. ex `<p>`, `<div>`, `<h1>` etc



**Margin and Padding**

![Difference](https://i.stack.imgur.com/UHD7W.gif)

## HTML5 Semantic Tags
### Heading
|Tags                     | Usage                                               |
|:---                     |:---                                                 |
| `<main>`|For the main content of a webpage, unique to a page.|
| `<section>`| Defines a certain section of a web page|
| `<article>`|Defines a bit of content which makes up an article.|
| `<aside>`|Defines some content related to something else(similar blogs)|
| `<header>`|For the header of a website, contains the nav, title etc|
| `<footer>`|The footer of a website|

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Mario Club</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <header>
      <h1>Mario Club</h1>
    </header>
    <section class="banner">
      <img id="banner-id" src="img/banner.png" alt="Mario Club Weclome Banner">
      <div class="welcome">
        <h2>Welcome to <br><span>Mario Club</span></h2>
      </div>
    </section>
    <nav class="main-nav">
      <ul>
        <li><a href="#">Join the Club</a></li>
        <li><a href="#">Latest News</a></li>
        <li><a href="#">New Games</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
    <main>
      <article class="">
        <h2>It's me, Mario</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
      </article>
      <ul class="images">
        <li><img src="img/thumb-1.png" alt="Mario thumb 1"></li>
        <li><img src="img/thumb-2.png" alt="Mario thumb 2"></li>
      </ul>
    </main>
    <footer>
      <p class="copyright">Copyright 2021</p>
      <p>Made with ❤️ by Farzam Alam</p>    </footer>
  </body>
</html>

```
```CSS
header{
  position: fixed;
  background-color: #f63232;
  padding: 15px;
  text-align: center;
  width: 100%;
  z-index: 1;
  top: 0;
  left: 0;
}
header h1{
  color: white;
  border: 8px solid white;
  padding: 6px 12px;
  display: inline-block;
  border-radius: 10px;
}

.banner{
  position: relative;
}

#banner-id{
  max-width: 100%;
}

.welcome{
  position: absolute;
  left: 0;
  top: 30%;
  color: white;
  background-color: #Feb614;
  padding: 30px;
}
.banner h2{
  font-size: 74px;
}

```
