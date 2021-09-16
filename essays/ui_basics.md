---
layout: essay
type: essay
title: UI Basics Technical Essay
# All dates must be YYYY-MM-DD format!
date: 2021-09-15
labels:
  - Information Technology
  - Web development
  - WOD
  - BrowserHistory
---



Overall, BrowserHistory1, 2, and 3 were not excessively difficult. I was able to complete each WOD in Rx time by the second attempt. Fortunately, I was able to recall the HTML and CSS syntax from the lessons on basic web development from ICS 101. I was still familiar with the header, image, and paragraph tags and could confidently use them to structure the webpage without needing additional help. 

Though BrowserHistory1 took the longest to complete, it was the least difficult of the 3. The purpose of BrowserHistory1 was to create the basic structure and content of the webpage. The only necessary document was an HTML document. The document used four essential elements: headers, paragraphs, images, and lists. I was familiar with these elements and their corresponding tags and had no difficulty ordering them and pasting their content between them. After learning about Intellisense that Visual Studio provides, I quickly created an Emmet Boilerplate without manually typing it out. The automatic Emmet Boilerplate completion allowed me to build the actual content right away and improved my overall efficiency. I stumbled on one area in BrowserHistory1, linking the Table of Contents to their corresponding section on the page. After a quick Google search, I learned that you could include a unique ID attribute for each header and link the Table of Contents items to the corresponding section in the page using their class name. For example, your header would look like this:

```html
<h2 id="internet_explorer">History of Internet Explorer</h2>
```

And your Table of Content list item would look like this:

```html
<li><a href="#internet_explorer">Internet Explorer</a></li>
```

BrowserHistory2 was slightly more complex than the previous. In addition to referencing elements in the CSS document, I needed to link the Google Fonts API to the HTML document properly. The Google Font API allows you to pull font files from the Google database and use the font style in your webpage. When I first viewed the Google API website, I was unsure where to locate the URL that I could paste into my document to reference the API and pull the font. I needed the API URL and the syntax for referencing the font in the CSS document. However, after further investigation, I figured out that the URL and CSS syntax is accessed by clicking on the tiles menu icon in the top right corner of the webpage. 

!["Google Fonts API"](./google_fonts.jpg)

I also needed to remind myself that the CSS document will cache itself within the browser, and a forced refresh is necessary if you want to see updated CSS configurations. 

BrowserHistory3 was not difficult. After placing each web browser section within their own 'Div' containers, I used the float attribute to position each section side by side. 

```css
div {
    width: 300px;
    float: left;
    padding: 0px 10px 0px 10px;
}
```
