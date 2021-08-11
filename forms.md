# Forms


Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information.HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.Whether you are adding a simple search box to your website or you need to create more complicated insurance applications, HTML forms give you a set of elements to collect data from your users. **In this note we will learn:**

* How to create a form on your website
* The different tools for collecting data
* New HTML5 form controls

## Why Forms?

The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

##  Form Controls
* adding text:

Text input (single-line)Used for a single line of text such as email addresses and names.
* Password input:

Like a single line text box but it masks the characters entered.

* Text area:

Text area (multi-line)For longer areas of text, such as messages and comments.

* making choices:  

Radio buttonsFor use when a user must select one of a number of options.

* Checkboxes:

Check boxes When a user can select and unselect one or more options.

* Drop-down boxes:

When a user must pick one of a number of options from a list.

* submitting Forms:

Submit buttonsTo submit data from your form to another web page.

* Image buttons:

Similar to submit buttons but they allow you to use an image.

* uploading files:

File uploadAllows users to upload files (e.g. images) to a website.






## Form structure 

**(form)Form** controls live inside a (form) element. This element should always carry the actionattribute and will usually have a method and id attribute too.

**action** Every (form) element requires an action attribute. Its valueis the URL for the page on the server that will receive the information in the form when it is submitted.

**method** Forms can be sent using one of two methods: get or post.With the get method, the values from the form are added to the end of the URL specified in the action attribute.


## text input 

The (input) element is used to create several different form controls. The value of the typeattribute determines what kind of input they will be creating.


**type = text**   When the type attribute has a value of text, it creates a single-line text input.

**name**  When users enter information into a form, the server needs to know which form control each piece of data was entered into. (For example, in a login form, the server needs to know what has been entered as the username and what has been given as the password.) Therefore, each form control requires a name attribute. The value of this attribute identifies the form control and is sent along with the information they enter to the server.

![img](data:image/png;base64,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)