# Day 0

## HTML
> HTML stands for Hyper text markup language. It is an standard language to create webpages.
> It was invented by Tim Berners-Lee in 1991.

## Hello World!
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hello World Title</title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

This is a very simple webpage that only shows hello world on the browser.

#### Tags:
> These are some keywords which defines how web browser will display the content.

In simpler terms tags are words that are used to make website. **They are like bricks of webpage**.  

General format of tags are ``` <tagname> Some text </tagname>``` .Examples```<body></body>, <h1><h1> and <p></p> ``` etc.

> The format, spelling and case should be exact.


#### Lets Explore the tags:

1. ```<!DOCTYPE html>``` : This tells the browser that this document is of type html.
2. ```<html> </html>``` : All the code inside these tags are html code.
3. ```<head> </head>``` : Head defines the top portion of the browser, and most common tag there is ```<title>```
4. ```<body> <body>``` : Every thing that we see in the browser window lies inside body.
5. ```<title> </title>``` : Title is present in the head of browser, and used to give title to webpage. For ex: **facebook**
6. ```<h1> </h1>``` : Header 1 or h1 is used to give heading in browser.

#### Structure of a webpage:
                                <!DOCTYPE html>  

                                    <html>

                        ......           <head>
                        .    .             *
                        ......             *
                          ::             </head>
                    ---------------       <body>
                  / |             | \       *
                 /  |             |  \      *
                    |             |         *
                    |             |         *
                     --------------         *           
                        |     |             *  
                        |     |           </body>

                                     </html>
###### Exercise 01
1. Create a folder on your desktop called as *hello-world* and inside *hello-world* create a file called  *index.html* and open *index.html* in notepad ++
2. Write a html program (document) with title *your name* and print *Hello your name* in browser window as header.

###### [Solution 01](exercises/01/index.html)

## Simple Web profile

```html
<!DOCTYPE html>
<html >
  <head>
    <title>Farzam Alam</title>
  </head>
  <body>
    <h1>Profile Webpage</h1>
    <h2>About</h2>
    <p>My Name is Farzam Alam. I work as a software developer.</p>
    <h2>Photo</h2>
    <img src="img.jpg">
    <h2>Favourite Quotes</h2>
    <p> <i>"You must be the change you want to see in the world"</i> - <b>Mahatma Gandhi </b> <br>
        <i>"If you are going through hell, keep going"</i> - <b>Winston Churchill</b>
    </p>
    <h2>Contact</h2>
    <p> <b> Mobile Number</b>: 9876543210 <br>
        <b> Email</b>: farzamcse@gmail.com
    </p>
  </body>
</html>

```

#### Explore more tags:
1. ```<h2> </h2>``` : h2 is called as header 2, it is a heading tag which is smaller than h1 in size.
2. ```<p> </p>``` : Paragraph tag is used to write sentences or paragraphs.
3. ```<b> </b>``` : Bold tag is used to make text inside them as bold.
4. ```<i> </i>``` : Italic tag is used to make text inside them as Italic.
5. ```<br>``` : This tag does not have an ending tag. This is used to break line in paragraphs.
6. ```<img>``` : Image tag is used to show image on the browser. It takes one attribute **src** which is used to show the location of image to show. This tag also doesn't have any end tag.

###### Exercise 02
1. Create a folder on desktop called *github-username*.github.io , inside this create a new file called *index.html* and paste your photo inside this folder. Rename your photo to *img.jpg*. Then open index.html in notepad ++
2. Write a html program with following functions:
  * Title as your Name
  * "About Me" heading
  * Simple paragraph about you.
  * "Photo" heading.
  * Your photo inside the "Photo" heading.
  * "Favorite Quotes" heading
  * Any Five quotes with Italic quote and speaker's name in bold.
  * "Contact Me" heading
  * Mobile Number and Email

##### [Solution 02](exercises/02/index.html)

## Deploy to Github:
1. Create a New repository inside github with name *github-username*.github.io
3. Check Add a with README file, leave everything else.
4. After it is created. Click on Add file then upload files.
5. Upload both **index.html** and **img.jpg** from the folder which you created earlier on desktop called *github-username*.github.io
6. Wait for 5 minutes then go to https://*github-username*.github.io


#### Bonus tags
1. ```<a href = "https://instagram.com/">Instagram</a>``` : This is called as link tag. It is used to define links in our webpage.
2. ```<h1>This is heading 1</h1>``` : Largest heading
3. ```<h2>This is heading 2</h2>``` : Smaller than h1 and larger than h3.
4. ```<h3>This is heading 3</h3>``` : Smaller than h2 and larger than h4.
5. ```<h4>This is heading 4</h4>``` : Smaller than h3 and larger than h5.
6. ```<h5>This is heading 5</h5>``` : Smaller than h4 and larger than h6
7. ```<h6>This is heading 6</h6>``` : Smallest heading.
