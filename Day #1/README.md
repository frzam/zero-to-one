# Day 1

## Headings and Tags
```html
<!DOCTYPE html>
<html >
  <head>
    <meta charset="utf-8">
    <title>Headings and List</title>
  </head>
  <body>
    <!--There are six level of headings-->
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>

    <!--Link -->
    <a href="https://www.instagram.com" target="_blank">Instagram</a>

    <!-- Ordered List -->
    <h2>Ordered List</h2>
    <ol>
      <li>Harry Potter</li>
      <li>Song of Ice and Fire</li>
      <li>The Hobbit</li>
    </ol>

    <!--Unordered List-->
    <h2>Unordered List</h2>
    <ul>
      <li>Pulp Fiction</li>
      <li>Forrest Gump</li>
      <li>3 Idiots</li>
    </ul>

    <!--Discription List-->
    <h2>Description List</h2>
    <dl>Books and Review</dl>
      <dt>The War of Art:</dt>
      <dd>This is book about how to be more productive and beat resistence.</dd>
      <dt>Rich Dad and Poor Dad:</dt>
      <dd>This is a book to understand basics finance and why investment is important.</dd>
  </body>
</html>
```
## Tags
### Heading
|Tags                     | Usage                                               |
|:---                     |:---                                                 |
| `<h1>This is heading 1</h1>`|Largest heading|
| `<h2>This is heading 2</h2>`|Smaller than h1 and larger than h3.|
| `<h3>This is heading 3</h3>`|Smaller than h2 and larger than h4.|
| `<h4>This is heading 4</h4>`|Smaller than h3 and larger than h5.|
| `<h5>This is heading 5</h5>`|Smaller than h4 and larger than h6|
| `<h6>This is heading 6</h6>`|Smallest heading.|

### List
|Tags                     | Usage                                               |
|:---                     |:---                                                 |
|`<ul>` | An unordered list. The list item will be marked as bullets(small black circle) |
|`<ol>` | An ordered list. The list items will be marked as numbers by default.|
|`<li>` | li is used do denote each list item present in ordered or unordered list. |
|`<dl>` | It defines the description list. |
|`<dt>` | It defines the term in a description list  |
|`<dd>` | It describes the term in description list |

### Formatting
|Tags                     | Usage                                               |
|:---                     |:---                                                 |
|`<b>` |Bold text|
|    `<strong>`|Important text |
|    `<i>`|Italic text|
|    `<em>`|Emphasized text|
|    `<mark>`|Marked text|
|    `<small>`|Smaller text|
|    `<del>`|Deleted text|
|    `<ins>`|Inserted text|
|    `<sub>`|Subscript text|
|    `<sup>`|Superscript text|

###### Exercise 01
1. Create a webpage with below mentioned format. Attach link on amazon to each description term so that when we click on it,
it will redirect to amazon page.

<p style= "align:center">
  <img src="https://github.com/farzamalam/zero-to-one/blob/1de38d8dc0582b74e2853825b83648021dd2238a/Day%20%231/exercises/01/01.PNG" />
</P>

##### [Solution 01](exercises/01/index.html)

## Structure and CSS
**Style** attribute is used to add styles to an element, such as color, font, size and more.

```html
<!DOCTYPE html>
<html >
  <head>
    <meta charset="utf-8">
    <title>Basics of CSS</title>
  </head>
  <body>
    <p>I am normal</p>
    <p style="color:blue;">I am blue</p>
    <p style="color:red;">I am red</p>
    <p style="font-size:20px">I am big</p>
    <div style="background-color:yellow" >
      <p>My name is farzam alam, I grew up in Raebareli, UP.</p>
      <p>I went to New Vision School</p>
    </div>
    <div style="font-family:verdana;color: #f1948a ;">
      <p>I didn't like to attend classes</p>
      <p>I went to New Vision School</p>
    </div>
  </body>
</html>
```
### Structure
|Tags                     | Usage                                               |
|:---                     |:---                                                 |
|`<div>`| Defines a section in a document (block-level) It is used to divide big webpage into multiple smaller component.|
|`<span>`|Defines a section in a document (inline)|

1. Use the **style** attribute for styling HTML elements
2. Use **background-color** for background color
3. Use **color** for text colors
4. Use **font-family** for text fonts
5. Use **font-size** for text sizes
6. Use **text-align** for text alignment

## Tribute Page:
```html
<!DOCTYPE html>
<html >
  <head>
    <meta charset="utf-8">
    <title>Gandhi ji Tribute page!</title>
  </head>
  <body style="text-align:center; background-color: #bde38d;">
    <!--Intro -->
    <div class="intro">
      <h1>Mahatma Gandhi</h1>
      <p><i>"Be the change you want to see in this world"</i></p>
    </div>
    <!--Profile Photo-->
    <div class="profile-phot">
      <img src="gandhiji.jpg"  height="400px" width="500px">
    </div>

    <!--About-->
    <div class="about">
      <h1>About</h1>
      <p>
        <b>Born:</b> October 2, 1869 <br>
        <b>Died:</b> January 30, 1948 <br>
        <b>Spouse:</b> Kasturba Gandhi <br>
        <b>Education:</b> UCL Facility of Law
      </p>
    </div>
    <!--Timeline-->
    <div class="timeline">
      <h1>Timeline</h1>
      <ul style="list-style-type: none;">
        <li><b>Oct 02, 1869:</b> Birth Of Mahatma Gandhi</li>
        <li><b>Sep 04, 1888:</b> Gandhi leaves to England to study law</li>
        <li><b>Oct, 1899:</b>Outbreak of Boer War(1899-1901)in South Africa. Gandhi organizes an ambulance corps for the British.</li>
      </ul>
    </div>
    <!--Quotes-->
    <div class="quotes">
      <h1>Quotes</h1>
      <ul style="font-style:italic; list-style-type: none;">
        <li> A man is but a product of his thoughts. He thinks he become.</li>
        <li>I will not let anyone walk through my mind with their dirty feet.</li>
        <li>Nobody can hurt me without my permission.</li>
        <li>An ounce of practice is worth a thousand words.</li>
      </ul>
    </div>
    <!--Reference-->
    <div class="reference">
      <h1>Reference</h1>
      <a href="https://en.wikipedia.org/wiki/Mahatma_Gandhi">Wikipedia</a>
    </div>
    <!--About me-->
    <div class="about-me">
      <p>Made with ❤️ by Farzam Alam</p>
    </div>
  </body>
</html>


```
