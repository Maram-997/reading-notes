# Read: 09 - Forms and Events
## FORMS
#### Form Controls:
There are several types of form controls that you can use to collect information from visitors to your site.
* **Adding Text**:(Text input(single-line),Password input,Test Area(multi-line)).
* **Making Choices**:(Radio Buttons,Check Box,Drop-Down Box).
* **Submitting Forms**:(Submit Buttons,Image Buttons).
* **Uploading Files**:(File upload(Allows users to upload files)).
#### How Forms Work:
1. A user fills in a form and then presses a button to submit the information to the server.
2. The name of each form control is sent to the server along with the value the user enters or selects.
3. The server processes the information using a programming language. It may also store the information in a database.
4. The server creates a new page to send back to the browser based on the information received.
#### Form Structure:
* `<form>` : Form controls live inside a `<form>` element. This element should always carry the action attribute and will usually have a method and id attribute too.
* action: Every `<form>` element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
* method:Forms can be sent using one of two methods: get or post.
* id:We look at the id attribute on page 183, but the value is used to identify the form distinctly from other elements on the page.
#### Text Input:
`<input>`:The `<input>` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.
* type="text":When the type attribute has a value of text, it creates a single-line text input.
* name: When users enter information into a form, the server needs to know which form control each piece of data was entered into.
* Maxlength:You can use the maxlength attribute to limit the number of characters a user may enter into the text field.
#### Password Input:
**`<input>`**
> * type ="password" :When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out.
* name: The name attribute indicates the name of the password input, which is sent to the server with the password the user enters.
* Size. Maxlength:It can also carry the size and maxlength attributes like the the single-line text input.
#### Text Area:
The `<textarea>` element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. Any text that appears between the opening `<textarea>` and closing `</textarea>` tags will appear in the text box when the page loads.
#### Radio Button:
**`<input>`**
> * type="radio":Radio buttons allow users to pick just one of a number of options.
* name:The name attribute is sent to the server with the value of the option the user selects.
* Value:The value attribute indicates the value that is sent to the server for the selected option. The value of each of the buttons in a group should be different.
* Checked: The checked attribute can be used to indicate which value (if any) should be selected when the page loads.
#### CheckBox:
> **`<input>`**
* type="checkbox":Checkboxes allow users to select (and unselect) one or more options in answer to a question.
* name:The name attribute is sent to the server with the value of the option(s) the user selects.
* value:The value attribute indicates the value sent to the server if this checkbox is checked.
* checked:The checked attribute indicates that this box should be checked when the page loads.
#### Drop-Down List Box:
* `<select>`:A drop down list box (also known as a select box) allows users to select one option from a drop down list.
* name:The name attribute indicates the name of the form control being sent to the server, along with the value the user selected. 
* `<option>`:The `<option>` element is used to specify the options that the user can select from. 
* value:The `<option>` element uses the value attribute to indicate the value that is sent to the server along with the name of the control if this option is selected.
* selected:The selected attribute can be used to indicate the option that should be selected when the page loads. The value of this attribute should be selected.
#### Multiple Select Box:
**`<select>`**
* size: You can turn a drop down select box into a box that shows more than one option by adding the size attribute.
* multiple: You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple.
#### File Input Box:
**`<input>`**
* type="file":This type of input creates a box that looks like a text input followed by a browse button. When the user clicks on the browse button, a window opens up that allows them to select a file from their computer to be uploaded to the website.
#### Submit Button:
**`<input>`**
* type="submit":The submit button is used to send a form to the server.
* name:It can use a name attribute but it does not need to have one.
* vaue:The value attribute is used to control the text that appears on a button. It is a good idea to specify the words you want to appear on a button because the default value of buttons on some browsers is ‘Submit query’ and this might not be appropriate for all kinds of form.
#### Image Button:
**`<input>`**
* type="image":If you want to use an image for the submit button, you can give the type attribute a value of image.
#### Button & hidden Controls:
**`<button>`**
The `<button>` element was introduced to allow users more control over how their buttons appear, and to allow other elements to appear inside the button.
**`<input>`**
* type="hidden":This example also shows a hidden form control. These form controls are not shown on the page (although you can see them if you use the View Source option in the browser).
#### Labelling Form Controls:
* `<label>`: When introducing form controls, the code was kept simple by indicating the purpose of each one in text next to it.
* for:The for attribute states which form control the label belongs to. Note how the radio buttons use the id attribute.
#### Grouping Form Elements:
* `<fieldset>`: You can group related form controls together inside the `<fieldset>` element. This is particularly helpful for longer forms.
* `<legend>`:The `<legend>` element can come directly after the opening `<fieldset>` tag and contains a caption which helps identify the purpose of that group of form controls.
* HTML5 introduces new form elements which make it easier for visitors to fill in forms.
## LISTS, TABLES AND FORMS
#### Bullet Point Styles:
###### list-style-type: 
The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).
> It can be used on rules that apply to the `<ol>`, `<ul>`, and `<li>` elements.
#### Images for Bullets:
###### list-style-image:
You can specify an image to act as a bullet point using the list-style-image property. The value starts with the letters url and is followed by a pair of parentheses. Inside the parentheses, the path to the image is given inside double quotes. This property can be used on rules that apply to the `<ul>` and `<li>` elements.
#### Positioning the Marker:
###### list-style-position:
Lists are indented ito the page by default and the list-style-position property indicates whether the marker should appear on the inside or the outside of the box containing the main points.
>This property can take one of two values:
>* outside:The marker sits to the left of the block of text.
>* inside:The marker sits inside the box of text (which is indented).
#### Table Properties:
You have already met several properties that are commonly used with tables. Here we will put them together in a single example using the following:(width,padding,text-transform,letter-spacing. font size,border-top. border-botton,text-align,background-color,:hover,give cells padding, distinguish heading, shade alternate rows,align numbers).
#### Border on Empty Cells:
###### empty-cells: 
If you have empty cells in you have empty cells in your table, then you can use the empty-cells property to specify whether or not their borders should be shown.
It can take one of three values:(show,hide,inherit).
#### Gaps Between Cells:
###### border-spacing, border-collapse:
The border-spacing property allows you to control the distance between adjacent cells.By default, browsers often leave small gap between each table cell, so if you want to increase or decrease this space then the border-spacing property allows you to control the gap. The value of this property is usually specified in pixels. You can specify two values if desired to specify separate numbers for horizontal and vertical spacing.
Possible values are:(collapse,seprate,).
#### Styling Forms:
It is most common to style:
* Text inputs and text areas
* Submit buttons
* Labels on forms, to get the form controls to align nicely
#### Cursor Styles(cursor):
The cursor property allows you to control the type of mouse cursor that should be displayed to users.
Here are the most commonly used values for this property:(auto
crosshair,default,pointer,move,text,wait,help,url("cursor.gif");)
#### Web Developer Toolbar:
1. ***Outlines:*** When you hover over an element, a red outline will be drawn around it, showing you how much space the element takes up.
2. ***StruCture:*** While you are hovering over
an element, the structure will be shown at the top of the window. Here you can see the `<li>` element has a class of completed, inside a `<ul>` with a class called to-do. The list is inside a `<div>` element with an id of page, and this sits inside the `<body>` and `<html>` elements.
3. ***CSS styles:*** When hovering over an element, click with your mouse to display the CSS. You will be shown the rules that apply to that element (and the l
ine they are on). 
## EVENTS
Here is a selection of the events that occur in the browser while you are browsing the web. Any of these events can be used to trigger a function in your JavaScript code.
|events  |  description  |
|--------|---------------|
|load|Web page has finished loading|
|unload|Web page is unloading (usually because a new page was requested)|
|error|Browser encounters a JavaScript error or an asset doesn't exist|
|resize|Browser window has been resized|
|scroll|User has scrolled up or down the page|
 KEYBOARD EVENTS: Occur when a user interacts with the keyboard (see also input event)
 |events | description |
 |-------|-------------|
 |keydown|User first presses a key (repeats while key is depressed)|
 |keyup|User releases a key|
 |keypress|Character is being inserted (repeats while key is depressed)|
 MOUSE EVENTS: Occur when a user interacts with a mouse. trackpad, or touchscreen
 |events|description|
 |------|-----------|
 |click|User presses and releases a button over the same element|
 |dblclick|User presses and releases a button twice over the same element|
 |mousedown|User presses and releases a button twice over the same element|
 |mouseup|User presses and releases a button twice over the same element|
 |mousemove|User moves the mouse (not on a touchscreen)|
 |mouseover|User moves the mouse over an element (not on a touchscreen)|
 |mouseout|User moves the mouse off an element (not on a touchscreen)|


 ***TERMINOLOGY***
EVENTS FIRE OR ARE RAISED:
When an event has occurred, it is often described as having fired or been raised. In the diagram on the right, if the user is tapping on a link, a click event would fire in the browser.
EVENTS TRIGGER SCRIPTS:
Events are said to trigger a function or script. When the click event fires on the element in this diagram, it could trigger a script that enlarges the selected item.

FOCUS EVENTS:Occur when an element (e.g., a link or form field) gains or loses focus.
|event|description|
|-----|-----------|
|focus/focus in|Element gains focus|
|blur/focusout|Element loses focus|
Form EVENTS:Occur when a user interacts with a form element.
|events|description|
|------|-----------|
|input|Value in any `<input>` or `<textarea>` element has changed (IE9+) or any element with the contented i table attribute|
|change|Value in select box, checkbox, or radio button changes (IE9+)|
|submit|User submits a form (using a button or a key)|
|reset|User clicks on a form's res~t button (rarely used these days)|
|cut|User cuts content from a form field|
|copy|User copies content from a form field|
|paste|User pastes content into a form field|
|select|User selects some text in a form field|

MUTATION EVENTSL:Occur when the DOM structure has been changed by a script.
|events|description|
|------|-----------|
|DOMSubtreeModified|Change has been made to document|
|DOMNodelnserted|Node has been inserted as a direct child of another node|
|DOMNodeRemoved|Node has been removed from another node|
|OOMNodelnsertedlntoDocument|Node has been inserted as a descendant of another node|
|DOMNodeRemovedFromOocument|Node has been removed as a descendant of another node|

#### HOW EVENTS TRIGGER JAVASCRIPT CODE
When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
1. Select t he element node(s) you want the script to respond to.
2. Indicate which event on the selected node(s) will trigger the response.
Programmers call this binding an event to a DOM node.
3. State the code you want to run when the event occurs.
Here you can see how event handling can be used to provide feedback to users filling in a registration form. It will show an error message if their username is too short.
1. SELECT ELEMENT: The element that users are interacting with is the text input where they enter the username.
2. SPEC! FY EVENT: When users move out of the text input, it loses focus, and the blur event fires on this element.
3. CALL CODE: When the blur event fires on the username input, it will trigger a function called checkUsername ().This function checks if the username is less than 5 characters.
![img](/images/events1.png)

#### THREE WAYS TO BIND AN EVENT TO AN ELEMENT
Event handlers let you indicate which event you are waiting for on any particular element. There are three types of event handlers.
1. HTML EVENT HANDLERS:
Early versions of HTML included a set of attributes that could respond to events on the element they were added to.The attribute names matched the event names. Their values called the function that was to run when that event occurred.
2. TRADITIONAL DOM EVENT HANDLERS:
DOM event handlers were introduced in the original specification for the DOM.They are considered better than HTML event handlers because they let you separate the JavaScript from the HTML.
3. DOM LEVEL 2 EVENT LISTENERS:
Event listeners were introduced in an update to the DOM specification.They are now the favored way of handling events.

#### TRADITIONAL DOM EVENT HANDLERS
All modern browsers understand this way of creating an event handler,but you can only attach one function to each event handler.
Here is the syntax to bind an event to an element using an event handler,and to indicate which function should execute when that event fires:
![img](/images/event2.png)
#### USING DOM EVENT HANDLERS
Before the DOM event handler, two things are put in place:
1. If you use a named function when the event fires on your chosen DOM node, write that function first. (You could also use an anonymous function.)
2. The DOM element node is stored in a variable.
#### EVENT LISTENERS
Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.
Here is the syntax to bind an event to an element using an event listener,and to indicate which function should execute when that event fires:
![img](/images/event3.png)
#### USING EVENT LISTENERS
the event listener appears on the last line of the JavaScript. Before you write an event listener, two things are put in place:
1. If you use a named function when the event fires on your chosen DOM node, write that function first.
2. The DOM element node(s) is stored in a variable.
**BROWSER SUPPORT**
Internet Explorer 8 and earfier versions of IE do not support the addEventlistener() method,but they do support a method called attachEvent().
**EVENT NAMES**
When you specify the name of the event that you want to react to, the event name is not preceded by the word "on".
#### USING PARAMETERS WITH EVENT HANDLERS & LISTENERS
Because you cannot have parentheses after the function names in event handlers or listeners, passing arguments requires a workaround.
Usually, when a function needs some information to do its job, you pass arguments within the parentheses that follow the function name.
When the interpreter sees the parentheses after a function call, it runs the code straight away. In an event handler, you want it to wait until the event triggers it.
Therefore, if you need to pass arguments to a function that is called by an event handler or listener, you wrap the function call in an anonymous function.
#### USING PARAMETERS WITH EVENT LISTENERS
The first line of this example shows the updated checkUsername() function. The mi nlength parameter specifies the minimum number of characters that the username should be.
The value that is passed into the checkUsername() function is used in the conditional statement to check if the name is long enough, and provide feedback if the username name is too short.
#### WHY FLOW MATTERS
THe flow of events only really matters when your code has event handlers on an element and one of its ancestor or desendent elements. 
The examples below has event listeners that respond to the click event on each of the following elements:(`<ul>`,`<li>`,`<a>`).
#### THE EVENT OBJECT:
When an event occurs, the event object tells you information about the event, and the element it happened upon.
Every time an event fires, the 
event object contains helpful 
data about the event, such as: 
* Which element the event happened on 
* Which key was pressed for a keypress event object 
* What part of the viewport the user clicked for a click event
>The event object is passed to any function that is the event handler or listener.
![img](/images/event4.png)
#### EVENT LISTENER WITH PARAMETERS
1. The reference to the event object is automatically passed to the anonymous function, but it must be named in the parentheses.
2. The reference to the event object can then be passed onto the named function. It is given as the first parameter of the named function.
3. The named function receives the reference to the event object as the first parameter of the method.
4. It can now be used by this name in the named function.
#### EVENT DELEGATION
Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.
>If users can interact with a lot of elements on the page, such as:
>* a lot of buttons in the UI
>* a long list
>* every cell of a table adding event listeners to each element can use a lot of memory and slow down performance.
#### ADDITIONAL BENEFITS OF EVENT DELEGATION
###### WORKS WITH NEW ELEMENTS
If you add new elements to the DOM tree, you do not have to add event handlers to the new elements because the job has been delegated to an ancestor.
###### SOLVES LIM ITATIONS WITH this KEYWORD
Earlier in the chapter, the this keyword was used to identify an event's target, but that technique did not work in IE8, or when a function needed parameters.
###### SIMPLIFIES YOUR CODE
It requires fewer functions to be written, and there are fewer ties between the DOM and your code, which helps maintainability.
#### CHANGING DEFAULT BEHAVIOR
The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event.
* preventDefault() : Some events, such as clicking on links and submitting forms, take the user to another page.
* stopPropagation() : Once you have handled an event using one element, you may want to stop that event from bubbling up to its ancestor elements (especially if there are separate event handlers responding to the same events on the containing elements).
> ***USING BOTH METHODS***
You will sometimes see the following used in similar situations that are in a function: return false; It prevents the default behavior of the element, and prevents the event from bubbling up or capturing further. It also works in all browsers, so it is popular.
#### WHICH ELEMENT DID AN EVENT OCCUR ON?
When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see the approach below used; it relies on the this keyword.
#### USER INTERFACE EVENTS
User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it.
The event handler I listener for UI events should be attached to the browser window.
![img](/images/event5.png)
