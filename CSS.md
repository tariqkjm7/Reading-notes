# CSS
[CSS:](https://developer.mozilla.org/en-US/docs/Glossary/CSS) **(Cascading Style Sheets)** allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.


![CSS](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRz1-yM3EG36gUtqcMmK293IYm7VkqToBmwzA&usqp=CAU)


## ***What is CSS for ?***
As we have mentioned before, CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

A document is usually a text file structured using a markup language — [HTML](https://tariqkjm7.github.io/Reading-notes/HTML) is the most common markup language, but you may also come across other markup languages such as SVG or XML.
### Three Ways to Insert CSS
***There are three ways of inserting a style sheet:***

* **External CSS :** With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section
* **Internal CSS :** An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the style TAGS + "<>" element, inside the head section.

* **Inline CSS :** An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
### Set the text-color for different elements in different ways:
**example:**

**1-** body {
  // using the color name

  color: red;

}


**2-** h1 {  // using the hexadecimal


  color: #00ff00;

}

**3-** p.ex {  // using the RGB


  color: rgb(0,0,255);

}

![Css colors](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRbj94yahU9Ouu9mk8WHVLvjxUuYOYMQ8xOGA&usqp=CAU)