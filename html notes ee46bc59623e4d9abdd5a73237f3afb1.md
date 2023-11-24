# html notes

**The <form> Element**

The HTML `<form>` element is used to create an HTML form for user input:

<form>

.

*form elements*

.

</form>

The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

All the different form elements are covered in this chapter: [HTML Form Elements](https://www.w3schools.com/html/html_form_elements.asp).

---

# The <input> Element

The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the `type` attribute.

Here are some examples:

| Type | Description |
| --- | --- |
| <input type="text"> | Displays a single-line text input field |
| <input type="radio"> | Displays a radio button (for selecting one of many choices) |
| <input type="checkbox"> | Displays a checkbox (for selecting zero or more of many choices) |
| <input type="submit"> | Displays a submit button (for submitting the form) |
| <input type="button"> | Displays a clickable button |

# Text Fields

The `<input type="text">` defines a single-line input field for text input.

# Example

A form with input fields for text:

```jsx
<form>  <label for="fname">First name:</label><br>  <input type="text" id="fname" name="fname"><br>  <label for="lname">Last name:</label><br>  <input type="text" id="lname" name="lname"></form>
```

This is how the HTML code above will be displayed in a browser:

First name:Last name:

**Note:** The form itself is not visible. Also note that the default width of an input field is 20 characters.

---

# The <label> Element

Notice the use of the `<label>` element in the example above.

The `<label>` tag defines a label for many form elements.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focuses on the input element.

The `<label>` element also helps users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the `<label>` element, it toggles the radio button/checkbox.

The `for` attribute of the `<label>` tag should be equal to the `id` attribute of the `<input>` element to bind them together.

---

# Radio Buttons

The `<input type="radio">` defines a radio button.

Radio buttons let a user select ONE of a limited number of choices.

---

# Checkboxes

The `<input type="checkbox">` defines a **checkbox**.

Checkboxes let a user select ZERO or MORE options of a limited number of choices.

# Example

A form with checkboxes:

```jsx
<form>  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">  <label for="vehicle1"> I have a bike</label><br>  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">  <label for="vehicle2"> I have a car</label><br>  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">  <label for="vehicle3"> I have a boat</label></form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_checkbox)

This is how the HTML code above will be displayed in a browser:

- [ ]  

I have a bike

- [ ]  

I have a car

- [ ]  

I have a boat

---

# The Submit Button

The `<input type="submit">` defines a button for submitting the form data to a form-handler.

The form-handler is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's `action` attribute.

# Example

A form with a submit button:

```jsx
<form action="/action_page.php">  <label for="fname">First name:</label><br>  <input type="text" id="fname" name="fname" value="John"><br>  <label for="lname">Last name:</label><br>  <input type="text" id="lname" name="lname" value="Doe"><br><br>  <input type="submit" value="Submit"></form>
```

This is how the HTML code above will be displayed in a browser:

First name:Last name:

---

# The Name Attribute for <input>

Notice that each input field must have a `name` attribute to be submitted.

If the `name` attribute is omitted, the value of the input field will not be sent at all.

# Example

This example will not submit the value of the "First name" input field:

```jsx
<form action="/action_page.php">  <label for="fname">First name:</label><br>  <input type="text" id="fname" value="John"><br><br>  <input type="submit" value="Submit"></form>
```

---

1. Aside: to display content aside from the content it is placed in.

<aside>
</aside>

1. A clickable button

<button type="button">Click Me</button>

1. A description list

<dl>
<dt>Coffee</dt>
<dd>Black hot drink</dd>
<dt>Milk</dt>
<dd>White cold drink</dd>
</dl>

1. Details: you can close and open

<details>
<summary>Epcot Center</summary>
<p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</details>

1. Fieldset: for a group related elements in a form

<!DOCTYPE html>
<html>
<body>

<h1>The fieldset element</h1>

<form action="/action_page.php">
<fieldset>
<legend>Personalia:</legend>
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname"><br><br>
<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname"><br><br>
<label for="email">Email:</label>
<input type="email" id="email" name="email"><br><br>
<label for="birthday">Birthday:</label>
<input type="date" id="birthday" name="birthday"><br><br>
<input type="submit" value="Submit">
</fieldset>
</form>

</body>
</html>

1. An iframe element: to display a mini version of the website

<!DOCTYPE html>
<html>
<body>

<h1>The iframe element</h1>

<iframe src="[https://www.w3schools.com](https://www.w3schools.com/)" title="W3Schools Free Online Web Tutorials">
</iframe>

</body>
</html>

1. Label: defines a label for several elements

<!DOCTYPE html>
<html>
<body>

<h1>The label element</h1>

<p>Click on one of the text labels to toggle the related radio button:</p>

<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
<input type="submit" value="Submit">
</form>

</body>
</html>

1. Navigation: to set the navigation links

<nav>
<a href="/html/">HTML</a> |
<a href="/css/">CSS</a> |
<a href="/js/">JavaScript</a> |
<a href="/python/">Python</a>
</nav>

1. Option list: A drop-down list

<!DOCTYPE html>
<html>
<body>

<h1>The option element</h1>

<label for="cars">Choose a car:</label>

<select id="cars">
<option value="volvo">Volvo</option>
<option value="saab">Saab</option>
<option value="opel">Opel</option>
<option value="audi">Audi</option>
</select>

</body>
</html>

1. A div tag

<!DOCTYPE html>
<html>
<head>
<style>
.myDiv {
border: 5px outset red;
background-color: lightblue;

text-align: center;
}
</style>
</head>
<body>

<h1>The div element</h1>

<div class="myDiv">
<h2>This is a heading in a div element</h2>
<p>This is some text in a div element.</p>
</div>

<p>This is some text outside the div element.</p>

</body>
</html>

1. Search

<!DOCTYPE html>
<html>
<body>

<h1>The search Element</h1>

<search>
<form>
<input name="fsrch" id="fsrch" placeholder="Search W3Schools">
</form>
</search>

</body>
</html>