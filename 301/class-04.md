# Read: Class 04 - React and Forms:
 ## Forms:
HTML form elements work a bit differently from other DOM elements in React.

>  In React, mutable state is typically kept in the state property of components, and only updated with setState().

### ***“controlled component”***
An input form element whose value is controlled by React.
The textarea Tag :

* In HTML, a `<textarea>` element defines its text by its children.
* In React, a `<textarea>` uses a value attribute instead. This way, a form using a `<textarea>` can be written very similarly to a form that uses a single-line input.
### ***the select tag :***

* In HTML, creates a drop-down list. For example, this HTML creates a drop-down list of flavors. Note that the Coconut option is initially selected, because of the selected attribute. 
* React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place.