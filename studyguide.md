# CSE 110 Midterm Study Guide


## Quick Access
* [Lab 1 - VSCode, Markdown and Git](#lab-1---vscode-markdown-and-git)

  * [Lab 1 - Review and Analyis Questions](#lab-1---review-and-analyis-questions)

* [Lab 2 - HTML and DevTools](#lab-2---html-and-devtools)

  * [Lab 2 - Review and Analyis Questions](#lab-2---review-and-analyis-questions)

* [Lab 3 - CSS and Agile](#lab-3---css-and-agile)

  * [Lab 3 - Review and Analyis Questions](#lab-3---review-and-analyis-questions)

 * [Lab 4 - JS, Diagramming and Devtools](#lab-4---js-diagramming-and-devtools)

---

## Lab 1 - VSCode, Markdown and Git

**1. What is the purpose of git clone?** <br>
The purpose of git clone is copy a remote repository into your local machine <br>

**2. What is the syntax of a Git commit with commit message** <br>
`git commit -m "Your message here"`<br>

**3. What does a good commit message look like?** <br>
   It describe what changed for example: <br>
   **Added changes to the `discountedPrices` function in filename.js**<br>

**4. What is the git command for staging changes?**  <br>
   `git add .` <br>

**5. What is the command to publish changes from local to remote repo?** <br>
   `git push` <br>

**6. Why might branching be useful?** <br>
   It lets you work on new features or fixes without changing the main code. ALso, you can pull request if you want to merge it with the main branch<br>

**7. Is there a single branching approach?** <br>
   No, each team can use different strategies like Git flow or trunk-based development <br>

**8. What is the file extension used for a Markdown file** <br>
   `.md`<br>

**9.  Write the markdown to insert an image stored in the same repository** <br>
    `![Alt text](img.png)`<br>

**10. What is the purpose of .gitignore in the repository?** <br>
    It tells Git which files or folders to skip (like temp files or build folders)<br>

**11. Create a heading in markdown (can be any level)** <br>
    `## This is a level two heading`<br>

**12. How to make text bold and italic in Markdown?** <br>
*Italic:* `*text* or _text_` <br>
**Bold:** `**text** or __text__` <br>
***Bold and Italic:** `***text*** or ___text___` <br>

---

### Lab 1 - Review and Analyis Questions
1. **What makes Markdown appealing compared to HTML? What do we trade off?** <br>
<br>

2. **When should you avoid Markdown and opt for HTML directly?** <br>
   <br>

3. **Convert the following into Markdown:** <br>
   <br>

 ```html
<img src="ucsd_cse110.png" alt="CSE 110: Intro to Software Engineering">
<h2>Goals</h2>
<ul>
  <li>Learn Markdown</li>
  <li>Understand HTML</li>
  <li>Compare both</li>
</ul>
<a href="https://example.org/markdown">Read more about Markdown here</a>
```

```
![CSE 110: Intro to Software Engineering](ucsd_cse110.png)

## Goals
* Learn Markdown
* Understand HTML
* Compare both

[Read more about Markdown here](https://example.org/markdown)
```

<br>

4.  **Write the Markdown syntax for a code block that prints “Hello Markdown” to the console in JavaScript.  You need to write the JS code and the markdown here.** <br>

```
```javascript
console.log("Hello Markdown");
```

Markdown syntax: start line with ``` and end line with the same 

<br>

5.  **Name three example use cases for markdown in software engineering projects.** <br>
   * Writing README files <br>
   * Documenting APIs <br>
   * Creating project wikis <br>

6.  **Github has a flavor of Markdown which helps support Software Engineering projects.  Discuss a 2-3 features or small details of Github's flavor of markdown and integration that could be useful to a software project.** <br>
   * You can reference issue and pull requests with #123 <br>
* You can create checklists with - [ ] <br>
* Code block supports syntax highlighting for many coding languages <br>

## Lab 2 - HTML and DevTools
See sample questions in the HTML Lecture Notes <br>

Use of common html tags - p, b, i, u, h1/2/3, ul, ol

---

### Lab 2 - Review and Analysis Questions

1. **Why is it important to have valid mark-up?** <br>
   It helps browser display your site correctly and makes your code easier to maintain and understand<br>

2. **What is the visual difference between <b> and <strong>? Is there another difference we should be concerned with?** <br>
   Both look bold, but `<strong>` also adds meaning for screen reader (it shows importance), while `<b>` is just for style <br>

3. **Why is excessive use of the &nbsp; entity that can force a space in an HTML document a " smell"?** <br>
   <br>

4. **Why is it important to be careful with HTML comment use?** <br>
   <br>

5. **Why are HTML <h1> tags big text in typical browsers?  Is that coming from HTML or CSS?** <br>
   <br>

6. **Write the HTML syntax to include an image of the UCSD logo named ucsd_logo.png.   Mind aspects like accessibility.** <br>
   <br>

7. **Convert the following markdown into HTML** <br>
   ```
    ## Grocery List

   * Eggs
   * Drinks
     1. Soda
     2. Milk
     3. Bottled Water
   * Steak
   ```
    HTML:

    ```html
    <h2>Grocery List</h2>
    <ul>
        <li>Eggs</li>
        <li>Drinks
            <ol>
                <li>Soda</li>
                <li>Milk</li>
                <li>Bottled Water</li>
            </ol>
        </li>
        <li>Steak</li>
    </ul>
    ```
   
   <br>

8. **Given the following mark-up** <br>
   ```
    <div class="paragraph">Visit our partner: 
    <a href="www.partner.com/page" style="color: black; text-decoration: none;">
    Click here
    </a>
    </div>
   ```
   **Explain the improvements that should be made both for markup, correctness, and usability.  If you don't recall from the CSS segment text-decoration controls underlining.** <br>

   Use https:// in the URL so it works properly, and consider keeping underlining for better accessibility. Also, don’t rely only on color to show it’s a link. <br>

9.  **This mark-up might be returned by an LLM or produced by one following a framework tutorial.  Comments on how it should be better?** <br>
    
    ```
    <div class="header">My Site</div>
    <div class="nav">
	    <div class="nav-item">Home</div>
	    <div class="nav-item">About</div>
    </div>
    <div class="main">
	    <div class="section-title">Welcome</div>
	    <div class="text">Thanks for visiting!</div>
    </div>
    <div class="footer">
	    <div class="contact-form">
		    <div class="btn" onclick="submitForm()">Submit</div>
	    </div>
    </div>
    ```
    <br>

    Use semantic tags like `<header>`, `<nav>`, `<main>`, and `<footer>` instead of all `<div>`s. Replace clickable `<div class="btn">` with a real `<button>` for accessibility. <br>

10.  **What is the purpose of the `<!doctype>` statement?** <br>
    <br>

11.  **Why might employing XHTML be useful for someone looking for a rigorous approach to web development?** <br>
    <br>

12.  **What is the idea of tag soup?  How do browsers deal with tag soup?  How does this permissiveness both help and hurt developing for the web.** <br>
    <br>

13.  **Explain the idea of progressive enhancement and what it tends to be used for.** <br>
    <br>

14.  **Explain the idea of graceful degradation and what it ends to be used for.** <br>
    <br>

15.  **Explain the idea of separation of concerns with HTML, CSS, and JS.  Explain the idea of locality of behavior with HTML, CSS, and JS.  Discuss the pros and cons with these ideas.** <br>
    <br>

---

## Lab 3 - CSS and Agile

See Sample questions in lecture notes <br>

1. **What is the use of Github issues in the agile process?** <br>
   <br>

2. **Why might one find incremental PRs an important part of the development environment?** <br>
   <br>

3. **Why should we not push straight to master/main?** <br>
   <br>

4. **What is the main idea behind standup meetings?** <br>
   <br>

5. **Why is it generally better to keep most of the CSS in an external stylesheet instead of using inline styles or internal style blocks?** <br>
   <br>

6. **Common CSS rules** <br>
   
      * **Background color (background-color)** <br>
        * Sets a background color <br>
  
      * **Class selector (.class)** <br>
        * Targets elements with a class
  
      * **ID selector (#id)** <br>
        * Target an element with a specific id
  
      * **Element selector (element)** <br>
        * Targets all <p> elements or any type of elements
  
      * **Text color (color)** <br>
        * Sets the text color
  
      * **Font size (font-size)** <br>
        * Sets the text size
  
---

### Lab 2 - Review and Analysis Questions

1. **Write a CSS comment with the string "CSS needs comments too!" in it.** <br>
   <br>

2. **Write a <link> tag referencing a stylesheet "print.css" to apply when printing out a page.** <br>
   <br>

3. **Write HTML and an inline style for a paragraph containing the text - "I'm big red!" set the text to 3x bigger than the size of the font for the document and the the text color to red.** <br>
   <br>

4. **Write CSS selectors with an empty rule { } for** <br>
   <br>

5. **Write CSS variables to set the text color and the background color. Now write a rule that uses the variables to set the contents of the <body> tag.** <br>
   <br>

6. **Why is it important to use relative measurements in CSS?  What "ilities" can you relate this advice to?** <br>
   <br>

7. **Explain from a software design point of view how CSS nesting improve our ability to write modular components?** <br>
   <br>

8. **Many developers are excited about using Tailwind and its utility classes.  An example of Tailwind class syntax is shown below** <br>
   <br>

9.  **Explain why !important is very useful and also a code smell?** <br>
    <br>

10. **The notes suggest that many linked CSS files or imported sheets may be an anti-pattern.  Explain why.  Again think about ilities here.** <br>
    <br>

---

## Lab 4 - JS, Diagramming and Devtools

1. **Why should you not use var?** <br>
   <br>

2. **How do you write a message to the console?** <br>
   <br>

3. **What is the difference between `const` and `let` keywords?** <br>
   <br>

4. **Given a JSON object, access a member variable/some property from it.** <br>
   <br>

5. **What is the difference between the `==` and `===` operators in JavaScript** <br>
   <br>

6. **Output of arithmetic/comparison operations like `'3' + 2`, `'2' < '12'`** <br>
   <br>

7. **What is the importance of a CI/CD pipeline?** <br>
   <br>

8. **Is it possible to build the pipeline in its entirety?** <br>
   <br>

9.  **Is the process a one-time setup?** <br>
    <br>

---
