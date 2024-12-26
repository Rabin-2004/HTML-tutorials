# HTML Forms
An HTML form is used to collect user input. The user input is most often sent to a server for processing.

## The `<form>` element 
The HTML `<form>` element is used to create an HTML form for user input:
```
<form>
form elements
</form>
```
The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

## The `<input>` Element
One of the most used form elements is the `<input>` element.The `<input>` element can be displayed in several ways, depending on the type attribute.
Example
```
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname"> 
```
## The `<label>` element
- The `<label>` Element

- The `<label>` element defines a label for several form elements.

- The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

- The `<label>` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the `<label>` element, it toggles the radio button/checkbox.

- The for attribute of the `<label>` tag should be equal to the id attribute of the `<input>` element to bind them together. 

### The `<select>` Element
The `<select>` element defines a drop-down list:
Example
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

The `<option>` element defines an option that can be selected.

By default, the first item in the drop-down list is selected.

To define a pre-selected option, add the selected attribute to the option: 
` <option value="fiat" selected>Fiat</option> `

Use the size attribute to specify the number of visible values:
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select> 
```
Use the multiple attribute to allow the user to select more than one value:
Example
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select> 
```

### The `<textarea>` element
- The `<textarea>` element specifies a long text-area commonly used for remarks and taking user feedbacks.
- the rows attribute is used to define the number of visible lines in a text-area.
- The column attribute is used to define the width of text area.
- You can also use CSS to define the height and width of the text-area.
<form>
<textarea name="message" rows="10" cols="30">
Hello World!
</textarea> 
</form>

### The `<button>` element
- The `<button>` element specifies a clickable button.
<button type="button" onClick="alert('Hello World')">Click Me</button>
- When button type is submit and reset it specifies a submit button and a reset button respectively provided the button is inside a form element.
<form>
<label for='name'> Name: </label>
<input type='text' name='name' id='name'>
<button type="submit">Click Me</button>
</form>

### The `<fieldset>` and `<legend>` attribute
- The `<fieldset>` element is used to group related data in a form.

- The `<legend> `element defines a caption for the `<fieldset>` element.

 <form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="Rabin"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Poudyal"><br><br>
    <button type="submit"> Submit </button>
  </fieldset>
</form> 

### The `<datalist>` element
- The <datalist> element specifies a list of pre-defined options for an <input> element.

- Users will see a drop-down list of the pre-defined options as they input data.

- The list attribute of the `<input>` element, must refer to the id attribute of the `<datalist>` element.

 <form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form> 

### The `<output>` element
- The `<output>` element represents the result of a calculation (like one performed by a script.

eg:
 <form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form> 