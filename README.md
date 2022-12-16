# Horiseon-Code-Refactor

## Technology Used

<table>
    <tr>
        <th>Technology Used</th>
        <th>Resource URL</th>
    </tr>
    <tr>
        <td>HTML</td>
        <td><a href="https://developer.mozilla.org/en-US/docs/Web/HTML">https://developer.mozilla.org/en-US/docs/Web/HTML</a></td>
    </tr>
    <tr>
        <td>CSS</td>
        <td><a href="https://developer.mozilla.org/en-US/docs/Web/CSS">https://developer.mozilla.org/en-US/docs/Web/CSS</a></td>
    </tr>
    <tr>
        <td>Git</td>
        <td><a href="https://git-scm.com/">https://git-scm.com/</a></td>
    </tr>
</table>

## Description

<a href="https://isglad.github.io/refactoring-marketing-site/">Visit the Deployed Site</a>

This project is a codebase modification of an existing Horiseon website homepage. This code refactor does not change the displayed styling of the page, only the underlying code to make the website more accessible and long-term sustainable. 

## Table of Contents

* [Code Refactor Example](#code-refactor-example)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Credits](#credits)
* [License](#license)

## Code Refactor Example

```html
<div class="search-engine-optimization">
    <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
    <h2>Search Engine Optimization</h2>
    <p>
        The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
    </p>
</div>
```
Converting the above non semantic div to an appropriate semantic element article provided clear description of what the section is about, and adding the id attribute to it enabled the functionality to the navigation link, Search Engine Optimization, in the header element. Also, adding explanatory comments clearly specifies what part of the code has changed.

```html
<!-- changed non semantic div element to a semantic element article and added id attribute -->
<article id ="search-engine-optimization" class="search-engine-optimization">
    <!-- added alt attribute to image tag -->
    <img src="./assets/images/search-engine-optimization.jpg" class="float-left" alt="search engine tools"/>
    <h2>Search Engine Optimization</h2>
    <p>
        The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
    </p>
</article>
```

## Usage

Once deployed, the website application looks like the below image. The layout is designed for traditional desktop web browser and is not designed for smaller screens yet. This website's image shows its appearance and functionality. 

![Horiseon site langing page](./assets/images/site.gif)


## Learning Points

- Use of HTML semantic element that clearly describes its meaning to both browser and developer.
- Structure HTML elements to follow a logical order.
- Verify and ensure that accessible alt attributes are added to image elements.
- Verify and ensure that heading levels (H1-H6) are sequentially ordered.
- Set a concise and descriptive title inside the head element.
- Provide explanatory comments to each line changed.
- Enable navigation links functionality.
- Consolidate CSS selectors and properties to increase its efficiency.

## Credits

Collabortors on this project are instructional staff, TAs and winter cohort 2022 of the University of Calfornia Berkeley Coding Bootcamp.

## License

MIT License

Copyright (c) [2022] [Gladys Ange Isingizwe]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
