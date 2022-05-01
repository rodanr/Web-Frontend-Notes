# HTML Basics
1. Simplest html form
```html
<!DOCTYPE html>
<!--
    -text inside this bracket is comment which is ignored by the browser
    -comments can be use to make reminder or explain the code
-->
<!--html tag is container tag that contains other tag inside it-->
<html>
  <!--An indentation should be made while creating child tag inside the parent tag-->
  <head>
    <!--title tag is a content tag that stores content/text inside it-->
    <title>Simples html as much possible</title>
  </head>
  <body>
    Body of the html file
  </body>
</html>
```
2. Basic tags
```html
<!DOCTYPE html>
<html>
  <head>
    <!--
            Meta tags:
            -Used to provide metadata about the site
            -e.g. description, charset etc
            -Helps search engine to know what more about it is
            -name gives the type of attribute and content gives its value
        -->
    <meta charset="UTF-8" />
    <meta name="description" content="This is an amazing site" />
    <title>Basic tags</title>
  </head>
  <body>
    <!--
            Note:
            - Layout of tags depend upon the order you have defined them
                -e.g paragraph tag can be above heading tag if it is defined first
        -->
    <!--
            Heading tags:
            -adds font size and weights making as heading in newspaper which is big and bold
            -ranges from h1 being biggest to h2 being smallest
        -->
    <h1>This is Heading 1</h1>
    <h2>This is Heading 2</h2>
    <h6>This is Heading 6</h6>
    <!--
            Paragraph tags:
            -use to write simple text paragraphs
            -auto adds spaces between paragraph tags
        -->
    <p>This is a paragraph</p>
    <p>This is another paragraph</p>
    <!--
            Bold,italic, underline tags
        -->
    <p>This is <b>bold</b></p>
    <p>This is <i>italic</i></p>
    <p>This is <u>underlined</u></p>
    <p>
      This is
      <b
        ><i><u>boldItalicUnderlined</u></i></b
      >
    </p>
    <!--
            Break tags:
            - Used to give a line break where it exists
            - It is a single tag that means it doesn't require start & end tag like <p></p> but only <br/>
            -<br> only works but <br/> is technically correct better to use it
        -->
    <p>above break tag</p>
    <br />
    <p>below break tag</p>
    <!--
            horizontal rule tag:
            -Use to draw a horizontal line to separate the contents in the web page
        -->
    <h5>Text above horizontal line or horizontal rule tag</h5>
    <hr />
    <!--
            Big tag and small tag:
            Big tag: Used to make a content/text little bit bigger
            Small tag: Used to make a content/text little bit smaller
        -->
    <p>This is Big:<big>Big</big> and Small:<small>Small</small></p>
    <!--
            Subscript and superscript tag:
            Subscript: use to write 2 in H2O where 2 lies below right to H
            Superscript: use to write 2 in a square where 2 lies above right to a
        -->
    <p>Use of Subscript: H<sub>2</sub>O</p>
    <p>Use of Superscript: a<sup>2</sup></p>
  </body>
</html>
```
3. Style and colors
```html
<!--
            -Style and colors are mainly done using css
            -Here some basics styling and coloring inside html is explained
        -->
<!DOCTYPE html>
<html>
  <head>
    <title>Style and colors</title>
  </head>
  <!--Making body background light blue-->
  <body style="background-color: lightblue">
    <h2 style="color: green"><big>This</big> header is green</h2>
    <p style="color: blue">This paragraph is blue</p>
  </body>
</html>
```
4. Formatting page
```html
<!--
  -Formatting helps to make a good code writing practice also helps in SEO
-->
<!DOCTYPE html>
<html>
  <head>
    <title>Formatting page</title>
  </head>
  <body>
    <!--
      -For best practice we divide the body into 3 parts
        -Header
        -Main
        -Footer
    -->
    <header>
      <!--Inside header we keep the head section of website like nav bar-->
      <nav>
        <ul>
          <li><a href="#">My Nav Item</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <!--Main content of the website is kept here-->
      <article>
        <!--Assuming as a blog website we have a article having several sections-->
        <section>
          <h2>Section Heading h2</h2>
          <h3>Section Heading h3</h3>
        </section>
        <section>
          <!--aside tag include those contents that are not actual website content but are shown like ads-->
          <aside>This is a advertisement</aside>
        </section>
      </article>
    </main>
    <footer>
      <!--Foot section of the website includes things like company name, contact, address etc-->
    </footer>
  </body>
</html>
```
5. Links
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Links</title>
  </head>
  <body>
    <!--
          -Links are used to travel between the webpages
          -Links can also be used to access a different website, a file etc.
      -->
    <!--
          -Clicking on it opens google homepage
        -->
    <a href="https://www.google.com" target="_blank">
      <!--
          -We can put any html element like heading tag, image etc here on clicking which user is redirected to that link
          -target setting as '_blank' helps to make user stay on our website and open link in new tab
        -->
      <h1>Google's Homepage</h1>
    </a>
    <!--
        Linking local html file here
    -->
    <a href="./extras/test_link.html" target="_blank">
      <big>Goto</big> local test_link html
    </a>
    <!--
        Linking to a image of cat
    -->
    <a href="./extras/cat.jpg" target="_blank">
      <h3>Open cat Image</h3>
    </a>
  </body>
</html>
```
6. Images
```html
<!--
    -Images are important part of html
    -Images are displayed using the image tag i.e img
    -The location is defined in img tag using src
    -Image location can be a image web address or directory location of hosted site
-->
<!DOCTYPE html>
<html>
  <head>
    <title>Images</title>
  </head>
  <body>
    <h2>Use of images tag</h2>
    <!--
        -alt text is displayed when images can't be loaded due to some reasons
        -Also, alt text help those people that are using text to speech feature to know what the image is
        Note: While sizing the img we have to maintain its aspect ration
        Giving only height or weight auto manages the undefined width or height
    -->
    <img src="./extras/cat.jpg" width="300" alt="A awesome cat image" />
    <!--Example of using image to open link-->
    <h3>Clicking on below cat image opens google homepage</h3>
    <a href="https://www.google.com" target="_blank">
      <img src="./extras/cat.jpg" height="100" alt="A awesome cat image" />
    </a>
  </body>
</html>
```
7. Videos and youtube iframes
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Videos and youtube iframes</title>
  </head>
  <body>
    <!--
        -controls property can be removed to disable user to play video
        -Thumbnail is added using the poster property
        -removing autoplay disables automatically playing while opening the site
        -loop helps to replay the video infinitely after the video finishes
    -->
    <video
      src="./extras/video.webm"
      poster="./extras/thumbnail.jpg"
      autoplay
      loop
      width="500"
      controls
    >
      This will be displayed if video can't be loaded somehow
    </video>
    <!--Embedding youtube video using iframe-->
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/EbCgL_gSXsw"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    >
      This will be displayed if iframe can't be loaded somehow</iframe
    >
  </body>
</html>
```
8. Lists
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Lists</title>
  </head>
  <body>
    <!--
          There are three types of list but first two types are most common
          1.Unordered list, put dot at beginning of the list 
          2.Ordered list, puts number, alphabet, roman number at the beginning of the list
          3.Description list, helps to add a list with description
      -->
    <!--Unordered list-->
    <h2>This is an Unordered list</h2>
    <ul>
      <li>item 1</li>
      <li>item 2</li>
      <ul>
        <li>sub item 1 of item 2</li>
        <li>sub item 2 of item 2</li>
      </ul>
      <li>item 3</li>
    </ul>
    <!--Ordered list-->
    <!--
        types of ordered list are
        type="a" numbering as a. b. c. ...
        type="A" numbering as A. B. C. ...
        type="I" numbering as I. II. ...
        type="i" numbering as i. ii. ...
        type="1" is default
    -->
    <h2>This is an ordered list</h2>
    <ol type="a">
      <li>item 1</li>
      <li>item 2</li>
      <ul>
        <li>sub item 1 of item 2</li>
        <li>sub item 2 of item 2</li>
      </ul>
      <li>item 3</li>
      <ol>
        <li>sub item 1 of item 2</li>
        <li>sub item 2 of item 2</li>
      </ol>
    </ol>
    <!--Description list-->
    <!--dt: description item-->
    <dl>
      <dt>Apples</dt>
      <dd>-They are Red</dd>
      <dt>Oranges</dt>
      <!--dd:describe description-->
      <dd>-They are orange</dd>
    </dl>
  </body>
</html>
```
9. Tables
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Tables</title>
  </head>
  <body>
    <!--
          -Table helps to align data in rows and columns
          -thead is used to hold the heads of table like caption and column names
          -tbody is used to hold the actual data of tables
          -Caption is the title above table
          -tr: table row
          -th: table head
          -td: table data
      -->
    <table>
      <thead>
        <caption>
          <h2>List of Employees</h2>
        </caption>
        <tr>
          <th colspan="3">Name</th>
          <th>Roll</th>
          <th>Number</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td colspan="3">Ram Yadav</td>
          <td>12</td>
          <td>1234567890</td>
        </tr>
        <tr>
          <td colspan="3">Shyam Jyadav</td>
          <td>21</td>
          <td>1234557890</td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```
10. Divs and spans
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Divs and spans</title>
  </head>
  <body>
    <!--
          At first we need to understand block elements and inline elements
          -block elements are those elements that capture a whole width even if the content doesn't require it
          -inline elements are those elements that only captures width that it needs to display itself fully
          -example of block elements is paragraph tag and example of inline element is anchor tag
          We also need to understand container tag
            -container tags are those tags that holds html elements/ tags inside it
            - Divs and spans are container tags that is used to specify container for collection of elements so that a property common to the whole collection can be applied by applying to that container as result all elements takes that effect
      -->
    <span>span1</span>
    <span>span2</span>
    <hr />
    <div>div1</div>
    <div>div2</div>
  </body>
</html>
```
11. Input and forms
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Input and forms</title>
  </head>
  <body>
    <!--
          -input tags helps to get input from user which is then grabbed by javascript code
          -type can be defined for the input type like password that gives some feature as for password the text is hidden
      -->
    <input type="text" value="username" />
    <input type="password" />
    <input type="date" />
    <input type="email" />
    <input type="range" />
    <input type="file" />
    <input type="checkbox" />
    <!--Only can click one radio button if has same attribute like name where checkboxes can have multiple select-->
    <input name="btn" type="radio" />
    <input name="btn" type="radio" />
    <input name="btn" type="submit" value="Submit plz" />
    <form action="">
      <!--Form is a wrapper for bunch of input elements-->
      <input type="text" name="username" />
      <input type="password" name="password" />
      <input name="btn" type="submit" value="Submit form" />
    </form>
    <!--Text area gives multiple block of lines for input like for paragraph entry-->
    <textarea rows="10" cols="30">
        Enter a paragraph
    </textarea>
    <!--Visit w3schools for more input elements-->
  </body>
</html>
```
12. iframes
```html
<!DOCTYPE html>
<html>
  <head>
    <title>iframes</title>
  </head>
  <body>
    <!--
          iframe allows to embed others website into our website
          Some website prevent themselves to be used as iframe like amazon as to avoid data theft
          removing frameborder gives more native feel
      -->
    <iframe
      src="https://www.mikedane.com/"
      width="1000"
      height="1000"
      frameborder="0"
      >This will be displayed if can't load iframe somehow</iframe
    >
  </body>
</html>
```
13. Metatags
```html
<!DOCTYPE html>
<html>
  <head>
    <!--
          -Metatags live in the head of html
          -Use to define the metadata about the particular webpage
          -help search engines to figure out about a particular page for SEO
      -->
    <meta name="description" content="Your description" />
    <meta name="author" content="Rodan" />
    <meta name="keywords" content="HTML, Tutorial, beginner" />
    <!--viewport Controls how your website is displayed is different devices-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Metatags</title>
  </head>
  <body></body>
</html>
```
