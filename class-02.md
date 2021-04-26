# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions

 ## HTML Book :
### Text:
* Browsers display the contents of headings at different sizes. The contents of an `<h1>` element is the largest, and the contents of an h6 element is the smallest. The exact size at which each browser shows the headings can vary slightly.
* p tag : To create a paragraph, surround the words that make up the paragraph with an opening  tag and closing tag.
> By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.
* b tag : By enclosing words in the tags and  we can make characters appear bold.
* i tag : By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic 
* sup tag : The `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts.
sub tag : The `<sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas.
* br tag : As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag `<br />`.
* hr tag : To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the `<hr />` tag.
* strong tag : The use of the `<strong>` element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.
* em tag : The `<em>` element indicates emphasis that subtly changes the meaning of a sentence.
* blockqoute tag : The `<blockquote>` element is used for longer quotes that take up an entire paragraph. Note how the `<p>` element is still used inside the `<blockquote>` element.
* q tag : The `<q>` element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the `<q>` element.
* abbr tag : If you use an abbreviation or an acronym, then the `<abbr>` element can be used. A title attribute on the opening tag is used to specify the full term.
* cite tag : When you are referencing a piece of work such as a book, film or research paper, the `<cite>` element can be used to indicate where the citation is from.

### Introducing CSS :
* CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
* CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.
* link tags : The `<link>` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does
not need a closing tag), and it lives inside the `<head>` element. 
> **It should use three attributes** :
href:This specifies the path to the CSS file.
type:This attribute specifies the type of document being linked to.
rel: This specifies the relationship between the HTML page and the file it is linked to.

* CSS Selectors : 

| Selector | Meaning |
|----------|---------|
|Universal Selector | Applies to all elements in the document |
|Class Selector | Matches element names |
|ID Selector | Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol |
|Child Selector | Matches an element that is a direct child of another |
|Descendant Selector | Matches an element that is a descendent of another specified element (not just a direct child of that element) |

* CSS rules usually appear in a separate document, although they may appear within an HTML page. 


## JavaScript Book : 
### Basic JavaScript Instructions :
* Statements : A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.
* Comments : You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.
* Variables : A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.
 > How to declare a variable and assign value for them: 
 We need to announce that we want to use it. This means creating the variable and giving it a name. This called *Declarining a Variable* . After that we can tell it information we would like to store in it. This Called * Assigning a Value to a Variable* .
* DataTypes : JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.

### Decisions and Loops : 
#### Switch Statement :
Stats with a variable callrd the switch value. each case indicates a possible value for this variable and the code that should run if the variable matches that value.
>  The difference between If-else and Switch :
  **If - else:**
  *1.* There is no need to provide an option.
  *2.* With a Series of if statement, they are all check even if a match has been found.
**Switch:** 
*1.* you have a default option that is run if none of the cases matches.
*2.* if a match is found, that code is run; then the break statement stops the rest.


