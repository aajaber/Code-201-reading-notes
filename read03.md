# Read: 03 - HTML Lists, CSS Boxes, JS Control Flow


** Lists in HTML:**
there are 3 types of **LISTS** in HTML 5:

- ***Ordered List:*** elements of this type will be ordered by numbers.

**Code Example :**

        <ol>
            <li>First Item.</li>
            <li>Second Item.</li>
            <li>Third Item.</li>
        </ol>

**Output:**

      1- First Item.
      2- Second Item.
      3- Third Item.



- ***Unordered List:*** elements of this type will be ordered by bullet point

**Code Example :**

        <ul>
            <li>First Item.</li>
            <li>Second Item.</li>
            <li>Third Item.</li>
        </ul>

**Output:**

-  First Item.
-  Second Item.
-  Third Item.





- ***Definition List:*** are made up of a set of terms along with the
definitions for each of those terms.

**Code Example :**

          <dl>
            <dt>Coffee</dt>
            <dd>Black hot drink</dd>
            <dt>Milk</dt>
            <dd>White cold drink</dd>
          </dl>

**Output:**

      Coffee
            Black hot drink
      Milk
         White cold drink



**Not Type**
- ***Nested Lists:*** inserting a list inside a main list.


**Code Example :**

        <ul>
            <li>ul First Item.</li>
            <li>
                <ol>
                    <li>OL First Item.</li>
                    <li>OL Second Item.</li>
                    <li>OL Third Item.</li>
                </ol>
            </li>
            <li>ul Second Item.</li>
            <li>ul Third Item.</li>
        </ul>

**Output:**

-  ul First Item

      1- OL First Item.

      2- OL Second Item.

      3- OL Third Item.
      
-  ul Second Item
-  ul this Item



## Boxes:
** Boxes in HTML:**
We can set several properties that affect the appearance of
these boxes. In this chapter you will see how to:

● Control the dimensions of your boxes

● Create borders around boxes

● Set margins and padding for boxes

● Show and hide boxes



**Box Dimensions:
width, height**

***Example:***

HTML
    <div>
        <p>
           <!--Add any Paragrapgh-->
        </p>
    </div>

CSS 

    div.box {
    height: 300px;
    width: 300px;
    background-color: #bbbbaa;}
    p {
    height: 75%;
    width: 75%;
    background-color: #0088dd;}



**Example of Boxes in HTML: **

      <!DOCTYPE html>
          <html>
               <head>
                <title>Boxes</title>
                 <style type="text/css">
           body {
           font-size: 80%;
           font-family: "Courier New", Courier,   monospace;
           letter-spacing: 0.15em;
            background-color: #efefef;}
            #page {
            max-width: 940px;
            min-width: 720px;
            margin: 10px auto 10px auto;
            padding: 20px;
            border: 4px double #000;
              background-color: #ffffff;}
              #logo {
              width: 150px;
              margin: 10px auto 25px auto;}
              ul {
              width: 570px;
              padding: 15px;
              margin: 0px auto 0px auto;
              border-top: 2px solid #000;
              border-bottom: 1px solid #000;
              text-align: center;}
              li {
              display: inline;
              margin: 0px 3px;}
              p {
              text-align: center;
              width: 600px;
              margin: 20px auto 20px auto;
              font-weight: normal;}
              BOXES 326
              Example
              BOXES
              a {
              color: #000000;
              text-transform: uppercase;
              text-decoration: none;
              padding: 6px 18px 5px 18px;}
              a:hover, a.on {
              color: #cc3333;
              background-color: #ffffff;}
              </style>
              </head>
              <body>
              <div id="page">
              <div id="logo">
              <img src="images/logo.gif" alt="The Analog Specialists" />
              </div>
              <ul id="navigation">
              <li><a href="#" class="on">Home</a></li>
              <li><a href="#">For Sale</a></li>
              <li><a href="#">Repairs</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Contact</a></li>
              </ul>
              <p>
              <img src="images/keys.jpg" alt="Fender Rhodes, Hohner Clavinet,
              and Wurlitzer EP200" />
              </p>
              <p>
              We specialise in the sales and repair of classic keyboards, in particular
              the Fender Rhodes, Wurlitzer EP200, and Hohner Clavinet.
              </p>
            </div>
          </body>
        </html>