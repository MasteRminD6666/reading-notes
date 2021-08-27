# Form basics

To create a form in HTML, you use the <form> element:
  

  
<form action="/signup" method="post" id="signup"> 
</form>
----
  
Code language: HTML, XML (xml)
The <form> element has two important attributes: action and method.

action is a URL that will process the form submission. In this case, it is /signup
method is the HTTP method to submit the form with. Typically, it is the post or get method. The post method sends data to the server as the request body while the get method appends the form data to the action URL with a ? operator.
In JavaScript, the form is represented as the HTMLFormElement object. The HTMLFormElement has the following corresponding properties:

- Action – the URL that will process the form data. It is equivalent to the HTML action attribute
- Method – can be get or post, which is equivalent to the HTML method attribute.
  

 ----
  
The HTMLFormElement element also provides the following useful methods:
  

- submit() – submit the form.
- reset() – reset the form.
  
  -----
  
  
### Referencing forms
  
To reference the <form> element, you can use the getElementById() method if the form has an id attribute:
  
-----
  
let form = document.getElementById('subscribe');
Code language: JavaScript (javascript)
  
-----
  
  
An HTML document can have multiple forms, not just one. The document.forms property returns a collection of forms on the document:

-----
  
document.forms
Code language: JavaScript (javascript)

-----
You can reference each form by numeric index. The following statement returns the first form in the document:
  
-----

document.forms[0]
Code language: CSS (css)
Submitting forms
Typically, a form has a submit button so that when you click it, the form data is sent to the action URL on the server for further processing.

To create a submit button, you use <input> or <button> element with the type submit:

<input type="submit" value="Subscribe">
Code language: HTML, XML (xml)
Or

<button type="submit">Subscribe</button>
Code language: HTML, XML (xml)
If the submit button has focus and you press the Enter keyboard, the form is also submitted.

When you submit the form this way, the submit event fires right before the request is sent to the server. It gives you the chance to validate the form data and decide whether to continue to submit the form or not.

To attach an event listener to the submit event, you use the addEventListener() method:

let form  = document.getElementById('signup');

form.addEventListener('submit', (event) => {
    // handle the form data
});
Code language: JavaScript (javascript)
If you want to stop the form from being submitted, you call the preventDefault() method inside the submit event listener:

form.addEventListener('submit', (event) => {
    // ...
    // stop form submission
    event.preventDefault();
});
Code language: PHP (php)
Generally, you call the event.preventDefault() method if the form is invalid.

To submit the form from JavaScript, you call the submit() method:

form.submit()
Code language: CSS (css)
Note that the form.submit() does not cause the submit event to fire, therefore, you should validate data before calling this method.

Accessing form fields
To access elements of a form, you can use the DOM methods like getElementsByName(), getElementById(), querySelector(), etc.

Additionally, you can use the elements property of the form object. The form.elements property returns a collection of input elements on the form.
  
  
![img](https://www.javascripttutorial.net/wp-content/uploads/2020/02/javascript-form.png)
  
### Submitting the form without providing any information will result in the following error:
  
![img](https://www.javascripttutorial.net/wp-content/uploads/2020/02/javascript-form-validation.png)
 
### Submitting with the name but invalid email address format will result in the following error:
  
![img](https://www.javascripttutorial.net/wp-content/uploads/2020/02/javascript-form-validation-email.png)
  

  

