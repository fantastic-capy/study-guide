# CSE 110 Midterm Study Guide

## Quick Access
* [Lab 1 - VSCode, Markdown and Git](#lab-1---vscode-markdown-and-git)

  * [Lab 1 - Review and Analyis Questions](#lab-1---review-and-analyis-questions)

* [Lab 2 - HTML and DevTools](#lab-2---html-and-devtools)

  * [Lab 2 - Review and Analyis Questions](#lab-2---review-and-analysis-questions)

* [Lab 3 - CSS and Agile](#lab-3---css-and-agile)

  * [Lab 3 - Review and Analyis Questions](#lab-3---review-and-analysis-questions)

* [Lab 4 - JS, Diagramming and Devtools](#lab-4---js-diagramming-and-devtools)

* [Lecture Notes](#lecture-notes)
  
	* [Lecture 1](#lecture-1)
  
	* [Lecture 2](#lecture-2)
   
	* [Lecture 3](#lecture-3)
   
	* [Lecture 4](#lecture-4)
   
	* [Lecture 5](#lecture-5)
   
	* [Lecture 6](#lecture-6)
  
	* [Markdown, HTML, CSS](#markdown-html-css)
   

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
   It lets you work on new features or fixes without changing the main code. Also, you can pull request if you want to merge it with the main branch<br>

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
[Go Back](#cse-110-midterm-study-guide)
---
### Lab 1 - Review and Analyis Questions
1. **What makes Markdown appealing compared to HTML? What do we trade off?** <br>
Markdown is simpler and quicker to use compared to HTML. We trade off full control and advance layout options that HTML offers. <br>

2. **When should you avoid Markdown and opt for HTML directly?** <br>
   Use HTML when you need custom styling, tables, or interactive features not supported by Markdown. <br>

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

Markdown syntax: start line and end line with ```

<br>

5.  **Name three example use cases for markdown in software engineering projects.** <br>
   * Writing README files <br>
   * Documenting APIs <br>
   * Creating project wikis <br><br>


6.  **Github has a flavor of Markdown which helps support Software Engineering projects.  Discuss a 2-3 features or small details of Github's flavor of markdown and integration that could be useful to a software project.** <br>
   * You can reference issue and pull requests with #123 <br>
* You can create checklists with - [ ] <br>
* Code block supports syntax highlighting for many coding languages <br>

---
[Go Back](#cse-110-midterm-study-guide)
---

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
   It often means you're using spaces to fix layout problems instead of using proper CSS <br>

4. **Why is it important to be careful with HTML comment use?** <br>
   Comments can accidentally expose private code or confuse others if not used clearly or removed if not needed <br>

5. **Why are HTML <h1> tags big text in typical browsers?  Is that coming from HTML or CSS?** <br>
   The size comes from default browser CSS, not HTML itself <br>

6. **Write the HTML syntax to include an image of the UCSD logo named ucsd_logo.png.   Mind aspects like accessibility.** <br>
   `<img src =”ucsd_logo.png” alt=”UCSD Logo”>` <br>

7. **Convert the following markdown into HTML** <br>
   Markdown:
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

   Use https:// in the URL so it works properly, and consider keeping underlining for better accessibility. Also, don’t rely only on color to show it’s a link. <br><br>

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

    Use semantic tags like `<header>`, `<nav>`, `<main>`, and `<footer>` instead of all `<div>`s. Replace clickable `<div class="btn">` with a real `<button>` for accessibility. <br><br>

10.  **What is the purpose of the `<!doctype>` statement?** <br>
    It tells the browser what version of HTML to expect so it can render the page correctly <br>

11.  **Why might employing XHTML be useful for someone looking for a rigorous approach to web development?** <br>
    XHTML requires stricter rules, which helps catch errors early and keeps code cleaner. <br>

12.  **What is the idea of tag soup?  How do browsers deal with tag soup?  How does this permissiveness both help and hurt developing for the web.** <br>
    Tag soup is messy or broken HTML. Browsers try to fix and display it anyway, which helps users but can hide developer mistakes. <br>

13.  **Explain the idea of progressive enhancement and what it tends to be used for.** <br>
    It means building a basic, working site first, then adding advanced features for better browsers. <br>

14.  **Explain the idea of graceful degradation and what it ends to be used for.** <br>
    It means building a full-featured site, but making sure it still works in older or simpler browsers. <br>

15.  **Explain the idea of separation of concerns with HTML, CSS, and JS.  Explain the idea of locality of behavior with HTML, CSS, and JS.  Discuss the pros and cons with these ideas.** <br>
* Separation: HTML for structure, CSS for style, JS for behavior—makes code cleaner and easier to manage.<br>
* Locality: Keeping related HTML, CSS, and JS close can make things faster to update but harder to reuse.<br>
* Pros: Better organization or quicker editing depending on the approach.<br>
* Cons: Harder to manage at scale (for locality) or slower to debug (for separation).<br>

    <br>

---
[Go Back](#cse-110-midterm-study-guide)
---

## Lab 3 - CSS and Agile
[See Sample questions in lecture notes](https://houses-pay-526.craft.me/qAdkHygjGuo1Vx) <br>

1. **What is the use of Github issues in the agile process?** <br>
   They help track tasks, bugs, and features so the team knows what to work on<br>

2. **Why might one find incremental PRs an important part of the development environment?** <br>
   Smaller PRs are easier to review, test, and fix reducing errors and merge conflicts<br>

3. **Why should we not push straight to master/main?** <br>
   It can break working code for others, changes should be reviewed first through PRs.<br>

4. **What is the main idea behind standup meetings?** <br>
   Quick daily meetings to share progress, plans, and blockers with the team <br>

5. **Why is it generally better to keep most of the CSS in an external stylesheet instead of using inline styles or internal style blocks?** <br>
   It keeps HTML cleaner, makes style reusable, and is easier to maintain or update <br>

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
[Go Back](#cse-110-midterm-study-guide)
---

### Lab 3 - Review and Analysis Questions

1. **Write a CSS comment with the string "CSS needs comments too!" in it.** <br>
    `/* CSS needs comments too! */`<br>

2. **Write a <link> tag referencing a stylesheet "print.css" to apply when printing out a page.** <br>
   `<link rel="stylesheet" href="print.css" media="print">`<br>

3. **Write HTML and an inline style for a paragraph containing the text - "I'm big red!" set the text to 3x bigger than the size of the font for the document and the the text color to red.** <br>
   `<p style="font-size: 300%; color: red;">I'm big red!</p>`<br>

4. **Write CSS selectors with an empty rule { } for** <br>
   * Selecting all elements in the page <br>
    `* { }`<br>

   * Selecting all `<p>` tags in class `"fancy"` <br>
    `p.fancy { }`<br>
   * Selecting all `<a>` tags which point to secured external links. <br>
    `a[href^="https://"]:not([href*="yourdomain.com"]) { }` <br>

   * Selecting all `<a>` tags within a `<nav>` tag directly in the page `<header>` <br>
    `header > nav > a { }` <br>

   * Selecting `<a>` tags when they are hovered. <br>
    `a:hover { }`<br>

   * Selecting a tag with the id value of `"help-info"`.<br>
    `#help-info { }`<br>

5. **Write CSS variables to set the text color and the background color. Now write a rule that uses the variables to set the contents of the <body> tag.** <br>
```
	:root {
 	  --text-color: #333;
  	  --bg-color: #f9f9f9;
	}

	body {
  	  color: var(--text-color);
  	  background-color: var(--bg-color);
}
```
   <br>

6. **Why is it important to use relative measurements in CSS?  What "ilities" can you relate this advice to?** <br>
Relative units like `em` or `%` help content adapt to different screens and settings. This supports scalability and accessibility.<br>

7. **Explain from a software design point of view how CSS nesting improve our ability to write modular components?** <br>
   Nesting keeps related styles together, reducing repetition. It helps in building components that are easier to reuse and maintain (modularity, readability). <br>

8. **Many developers are excited about using Tailwind and its utility classes.  An example of Tailwind class syntax is shown below** <br>
   Tailwind lets you style directly in HTML using short, reusable classes. This improves speed and consistency, but can clutter HTML.<br>

9.  **Explain why !important is very useful and also a code smell?** <br>
    `!important` forces a style to apply, which is useful for quick fixes. But it's a code smell because it breaks the normal flow and makes debugging harder.<br>

10. **The notes suggest that many linked CSS files or imported sheets may be an anti-pattern.  Explain why.  Again think about ilities here.** <br>
    Having many linked/imported stylesheets increases load times and complexity. It harms maintainability, performance, and scalability. <br>

---
[Go Back](#cse-110-midterm-study-guide)
---

## Lab 4 - JS, Diagramming and Devtools

1. **Why should you not use var?** <br>
   You should not use var because it is function-scoped and hoisted. It is better to use let or const which are block scoped and you will run into less bugs <br>

2. **How do you write a message to the console?** <br>
   `console.log(“Message Here”);` <br>

3. **What is the difference between `const` and `let` keywords?** <br>
   `const` means a variable can’t be reassigned, while `let` can be changed later <br>

4. **Given a JSON object, access a member variable/some property from it.** <br>
   Use dot notation: `object.property` or bracket notation `object[“property”]`<br>

5. **What is the difference between the `==` and `===` operators in JavaScript** <br>
   `==` compares values loosely, ignoring types where `===` compares both values and types <br>

6. **Output of arithmetic/comparison operations like `'3' + 2`, `'2' < '12'`** <br>
   `‘3’ + 2` returns `‘32’` which is string and `‘2’ < ‘12’` returns `false` <br>

7. **What is the importance of a CI/CD pipeline?** <br>
   The importance of a CI/CD pipeline is that it automates testing and deployment, making software updates faster and safer <br>

8. **Is it possible to build the pipeline in its entirety?** <br>
   Yes, you can fully build and up a CI/CD pipeline with the right tools <br>

9.  **Is the process a one-time setup?** <br>
    No, it needs update overtime as the project grows or changes <br>

---
[Go Back](#cse-110-midterm-study-guide)
---

## Lecture Notes

### Lecture 1

 * [Lecture 1: SE Intro - Demystification, Definition, and Defiance](https://houses-pay-526.craft.me/BEtiGoivUaqXO5) <br>

	* [Lecture 1 Slides](lecture1.pdf) <br>

1. Defining Software Engineering in Your Own Words <br>
	* **ANSWER:** Software engineering is the process of designing, building, testing, and maintaining software in a structured and organized way. Unlike programmers who mainly write code, software engineers focus on the whole system and how all parts work together over time. <br>

2. Why So Many Definitions? <br>
	* **ANSWER:** There are many definitions of software engineering because it covers a wide range of tasks, tools, and roles, and people often explain it based on their own experience or focus—some think more about the planning, some about the teamwork, and others about the coding. Also, the field keeps growing and changing, so new ideas and methods keep adding to how we define it.<br>

3. To Professionalize SE or Not? <br>
	* We read a provocative paper about if Software Engineers are engineers or not.  This prompted us to write a personal statement and make a plan to understand what we wanted to be, but in this question we meet this professional engineer point head on.  Do you think it is useful for us to professionalize, to have certification, standards and practices, and so on?  Explain why you think this is a good idea and bad idea.  The best answers may argue both sides to show deep consideration.<br>

4. Externalities and SE <br>
	* Throughout the course the Professor will provide examples of effects far outside the code we write.  The Professor in fact feels that the code aspect is much more predictable and under our control than anything else in the software process and these external effects often can derail all that work.   External effects might be organizational, some might be industry trends and beliefs, some economic, some could be regulatory, and on and on.   To show you understand broader effects to software and its development provide one example from the world or industry you have run across and discuss its effects on software and its creation for 1-3 paragraphs.   <br>

	* This should not be a hard question as examples about.  To get your started consider LLMs, Social media beliefs, VC and financialization effects, regulatory effects (ex. Apple vs EU/ DOJ), power and water use, the implication of crypto, on and on.  <br>  

	* The purpose of this question is to reinforce a broader view of software and its societal intersection that is personal to YOU.<br>

5. Software >>> Code <br>
	* Enumerate 3 - 5 artifacts beyond the source code that is part of software.  Besides listing the artifacts explain why it is important and/or how it is used. <br>

		* Requirements – A list of what the software should do. Helps make sure the right features are built. <br>

		* Design Plans – Pictures or charts that show how the software works. Helps the team plan before coding. <br>

		* Tests – Steps to check if the software works. Helps find and fix problems early. <br>

		* User Guide – Instructions for people using the software. Helps users understand how to use it. <br>

		* Project Schedule – A plan of who does what and when. Keeps the team organized and on time. <br>

6. Could SWE be more a Social Science? <br>
	* Since people are a huge aspect of software engineering is the field more related to social sciences than hard sciences?  Discuss how it is the same and how it is different than social sciences.  You may find it useful to compare SWE with other engineering disciplines like civil, aeronautical, chemical, etc. to what we do and see if they have similar challenges. Finally, ask yourself what it take to do a SWE study and how you would replicate (or not) the findings of a study.  
<br><br>


---
[Go Back](#cse-110-midterm-study-guide)
---

### Lecture 2

* [Lecture 2: Individual Devs](https://houses-pay-526.craft.me/fWTsrhQJjFDYl7) <br>

	* [Lecture 2 Slides](lecture2.pdf) <br>

1. 10x Developers <br>
	* Explain the rough idea of the 10x developer in Software Engineering. How does one typically become a 10x developer? Discuss the pros and cons of a 10x developer. <br>

	* Are you interested in being one of these?  If so what do you think your next steps should be? <br>
 
2. Leprechaun SWE Concepts <br>
	* At the conclusion of the 10x developer segment it was discussed that maybe the rough idea of 10x devs is right, but the specifics and "science" of this is at best dubious.  What should we really take away from this, to ignore the concept or something else entirely.  Explain your thinking.
<br>

3. Tools over people <br>
	* Some people deeply wish that tools and technology will solve developer productivity issues.  Data and history doesn’t seem to suggest that is a good bet.  If that is the case why do you think people keep pushing the tool over people idea?  <br>

	* Provide a modern example of this thinking and at least one thought that may make holding out for a big tool/tech win unlikely. <br>

4. Balanced Engineers <br>
	* What does it mean to be a “T” Shaped engineer?  Provide a short example of how a T shaped engineer might save a project or team.   To personalize this consider some aspect of your personality or interests that has helped you as a dev. <br>

5. The Technical Identity Trap? <br>
	* Complexity of platforms and systems is such that we often need to hyper-specialize to succeed especially in our careers.  Often times this can be both favorable leading to wonderful career opportunities and dangerous making us myopic in our solution findings, insufferable in our preferences, and potentially precarious in our long term career path.   To further your thoughts on that statement read the article here which presents some thoughts on this [https://sean.voisen.org/writing/insert-favorite-technology-here-guy](https://sean.voisen.org/writing/insert-favorite-technology-here-guy) as well as any other points you may find online about this concern.  Now that you have pondered the dangers of specialization provide your own short discussion of a current technology, platform, trend, etc. that you are interested in and discuss the pros and cons of specialization in it.  Make sure to provide both positive and negative thinking about outcomes and be personal in your response. <br>

6. Psychology Challenges for SEs <br>
	* What is impostor syndrome? <br>

	* Why do you think developers get impostor syndrome so commonly? <br>

7. Practice Makes Better <br>
	* Purposeful practice is the way to grow your skill in mosts pursuits.  The attached blog post from the ever insightful Mandy Brown presents a challenge with this growth by practice - the gap between your ability and your taste.  Read the paper and be prepared to explain two things.  <br>

		* What is the gap?  How is challenging? What we should do about it?  <br>
  
		* How might we characterize taste as SWEs?  <br>
  
 		 * Finally note the 3 edits in red.   Take a guess what the words might have been and what some readers might have done with their inclusion.  Why were these words changed or removed?<br>

8. Valuing Failures and Resiliency <br> 
	* If failure is required to learn things describe how to approach failure in a safe way as a learning dev.  For maximum consideration make your answer personal or related to what you experienced on your team or an internship. <br>

9. Industry and Societal Challenges for SEs <br>
	* At times it feels like industry is moving so fast that anything you learn in school or even on a job is out of date before you even master it.  Figuring out coping mechanisms to address the whirlwind of change is a key skill for a software engineer these days.  Describe how you might approach this for your growth beyond this course.  Hint:  Think about dividing your learning efforts and time % wise and topic wise.<br>

10. Explain Individual SE Misconceptions Using System Thinking <br>
	* SEs are smart people and like most people we do things for real reasons.  However, as we have observed in this segment and across the industry there are many misconceptions and beliefs that seem somewhat troubling when we stop and ponder them. The Prof contends that some of our beliefs and misconceptions are likely driven by numerous forces many potentially more systems based including economics, social, regulatory, custom, convention, and more.  See if you can think of an example to support his thoughts.  Avoid just saying someone is ignorant.  If ignorance is a key component explain how that came to pass from a systems point of view.<br>

11. Seniority Path and Titles <br>
	* Write down how many years it should take to reach a Senior Engineer status.  Allow it to be a range.  Now determine what types of skills and experiences would be required to reach that status over time.  Once you have completed this task, read this commentary on titles and seniority.  Do you agree with the premise and the problems mentioned?<br>

12. Good Ideas Still Go Bad? <br>
	* Some behavioral concepts, like having a less fixed mindset (aka a growth mindset) or being agreeable with people, seem pretty innocuous.  However, like all good things, it is possible that they can be twisted into something that might be problematic.  Ed Zitron wrote in The Cult of Microsoft [https://www.wheresyoured.at/the-cult-of-microsoft/](https://www.wheresyoured.at/the-cult-of-microsoft/) about this exact thing and how it can backfire.  Now, see if you can consider one of the ideas of individual behavior that seems generally correct to you and find a way to make it backfire.   <br>

	* Question Outcome: Doing this activity well is learning to think in reverse (bad to good or good to bad).  This ability can help you see nuances rather than fall back on binary thinking. 
<br><br>

---
[Go Back](#cse-110-midterm-study-guide)
---

## Lecture 3

* [Lecture 3: Groups](https://houses-pay-526.craft.me/22hg03hlJlPkBG) <br>

	* [Lecture 3 Slides](lecture3.pdf) <br>

1. Visualizing the Team Life Steps <br>
	* We have discovered that teams go thru a common set of steps.  We will use teams in this class since most software of any importance is built with teams.  To prepare ourselves for this process define the point of the step and write a few short sentences or bullets that describe what specifically would happen in this step.  Be descriptive and personal as what YOU may want to happen. <br>

2. Joining a Team <br>
	* The quality of the process of onboarding a team member onto an existing team highly correlates to new member success.  Describe 2-3 things a team and 2-3 things the joining member can do to help make the process a success.  If you want to think of this in industry terms consider the idea of “on boarding” and what the first days or weeks of your new employment would be like in an idealized world. <br>

3. Your Team <br>
	* Don't need to answer<br>
 
4. Leaving a Team <br>
	* In life, the start, the finish, and the high points of the so-called messy middle is really all we remember.  The same holds for a software teams.  It is assumed, that eventually will join a team beyond school (or in this class you may drop and need to leave the team).  Describe in a bullet list what you should do in an exit and anything the team should do as well.  Hint:  The next question might help you figure this out. <br>

5. How do teams survive members leaving? <br>
	* What kind of approaches should we take to make sure a team can survive the loss of members.  Consider single loss, multiple member loss, and full team loss as separate aspects and be as specific as you can describing artifacts, activities, team practices, etc. that might be employed before, during, and after team member(s) leaves. <br>

6. Characteristics of Good & Bad Teammates <br>
	* The actions and communication patterns of team members will vary.   Describe the characteristics of good teammates as well as the tendencies and actions of bad teammates. <br>

7. Team as Output <br>
	* A software engineering pundit named Jason Gorman says that at the actual result we should focus on is more the team than the product.  This isn’t quite true since shipping software products is our task, but the though is regardless of that outcome a proper team should be produced.  Explain this thought in your own words using an example. <br>

8. The Google Study <br>
	* A Google study was conducted to figure out what makes for high functioning teams and five factors were discovered to be important.  Name and explain each of the five factors.  Now explain which is the most important factor and discuss why it would be important.  
- or - Discuss how the idea of Psych Safety is handled on your CSE SWE team. <br>

9. Bus Factor - Why and Fixes <br>
	* Define bus factor.  Provide an example in the context of your SWE project team and how a bus factor might arise.  Now discuss what you can do mitigate this potential problem. <br>

10. Team Composition and Work Type <br>
	* Various ideas of teams and membership were discussed.  Contrasts were made between members who do all things and those who are specialists.  Discuss both ideas and explain any pro and con ideas with each.  Relating this to the type of work performed might be a useful way to ponder this question. <br>

11. Conways Law <br><br>
	* Conway’s Law suggests that the software architecture and team structure will often be a function of the organizational structure.  If this is a strict rule and we discover that the software architecture is bad, in order to address the poor architecture what might we need to do outside of just focusing on the code itself.

	* A question variation might be just to describe what Conway’s Law is and compare it to organization size or type.
<br><br>

---
[Go Back](#cse-110-midterm-study-guide)
---
 
 ### Lecture 4

 * [Lecture 4: Groups - Work Patterns](https://houses-pay-526.craft.me/kWQ3qUEctR4yNc) <br>

	* [Lecture 4 Slides](lecture4.pdf) <br>

 1. Apply The Play Styles:Imagine if we give you scenarios, pros, cons and descriptions can you match them up to the play styles?  For example, what would be appropriate in a crisis situation?  How might you reduce bus factor via a play style etc. <br>

2. Why is it essential to have a definition of done? <br>


3. Why is documentation so necessary in light of team efficiency and member tenure? <br>


4. What is the concept of promiscuous pairing?  What are good aspects about it?  What are bad aspects about it? <br>


5. The Professor suggests that we should not employ only a single style over the lifetime of software, why is it that many people seem to gravitate to one play style over the other?  Provide some concrete examples if possible. <br><br>

* [Lecture 5: User Centered Design Process](https://houses-pay-526.craft.me/7zdiANnydceeYS) <br>

	* [Lecture 5 Slides Part 1](lecture5pt1.pdf) <br>
 
 	* [Lecture 5 Slides Part 2](lecture5pt2.pdf) <br>

  ---
[Go Back](#cse-110-midterm-study-guide)
---

### Lecture 5

1. UCD Mantra Memorization and Understanding <br>
	* The UCD mantras such as "You are not the user", "Don't make them wait" and many others in the summary can be quite useful to organize thoughts and keep users front of mind as we develop.  Be prepared to cite them in fill in our other forms and explain them succicnctly. <br>

2. User Story Example <br>
   	* Write an example user story for a student using a flash card app.  Be specific and use the common format for full points.  <br>
   
3. Dangerous Pretty Pixels <br>
	* Why should we start with rough wireframes?  What is the purpose of the roughness and what is the outcome we are looking for with the wireframing process?  What are possible problems with using higher fidelity prototypes early in a project process? <br>

4. Recognizing the "We Build Subsystems" Mental Model <br>
	* You are going to build web based software using a tech stack of our choice that will call the OpenAPI to create "Cringe Dad Jokes" on demand. The subsystem mental moedl works from "safe" green areas Decomposition and Execution, up to yellow Form, orange Distribution, and red ("difficult to econtrol") Environment. Outside are groups of people. Demonstrate you understand the model by giving an example of choices you might make at each level. Present a risk for each level. Be specific in your examples as even the short app description contains enough information to be concrete about concerns. <br>

5. The RAIL Model <br>
	* Explain the RAIL model explanding the acronym and providing the values.  Explain why each value is important.<br>

6. Evaluting the User -ilities <br>
	* Your software may have characteristics in the form of -ilities also known as non-functional requirements.  Name the 6 ilities mentioned that are very user effecting and their meanings and provide an example of how you might verify each point.  (Hint: think about testing designs, analytics, monitors, interviews, etc.)<br>

7. "Spooking the Animals" and Other UCD Dangers <br>
	* Numerous examples of how we must be careful with thinking and interacting with end users to get good outcomes were talked about.  Explain the idea of "Spooking the Animals" meant and what the Prof's worry and solution.  If you can think of other fun examples along other lines that might lead a UCD process astray you can note them.  A question about this may reward more points if a student can show nuance in how they think about user focused design challenges. <br>

8. The T Shaped Engineer <br>
	* The idea of the T Shaped Engineer was presented in a previous section.  In this section we discussed the importance of user centeredness in the design and development process.  How would a balanced T shaped engineer have advantages over a narrower T shaped tech focused engineer?  For those, not confident in the UCD sticking to the narrow focus how will ensure end user acceptance of our software?  Instead of us being involved who would do this work and what will be the concerns or risks we might have by not being involved in UCD processes? <br>

9. AI for UCD <br>
	* Some folks have proposed that AI can be used to user centered design activities including user studies and focus.  Discuss how AI might be useful and how it very much might not be for the UCD effort? <br>

10. Accessibility for All Even Bots!?! <br>
	* When people think of accessibility they often think of extremes such as a blind user using the web.  Explain how accessibility might be more a range and use yourself showing how you may have accessibility needs now or in the future. <br>

	* Is it possible that accessibility efforts can help those who may not need it?  Explain with a specific example if you can. <br>

	* How can accessibility efforts potentially be helpful to AI?  Explain with a specific example if you can.  (Hint: Think of image understanding or content structure)
<br><br>

* [Lecture 6: Process Models Overview](https://houses-pay-526.craft.me/bzm9y0vVAxD6w9) <br>

	* [Lecture 6 Slides](lecture6.pdf) <br>

 ---
[Go Back](#cse-110-midterm-study-guide)
---

### Lecture 6

1. The AI Revolution and Process Models <br>
	* If AI is a big change like dotCom was that spurred Agile what would imagine the process model to be adopted would be? <br>
 
 	* Would the activities change in the SDLC or would we just change the emphasis of steps? <br>

2. The People Counter Argument <br>
	* If we could have some form of Taylorism Scientific Software Engineering and just swap out one dev for another dev, what would be required?  Think formality and definition?  If you consider the nature of what we actually do as SWEs does this actually make sense to you?  Why or why not and be concrete in an example. <br>

3. Risk, Time, and Money <br>
	* Much of the ideas of this segment seem to be about lowering risk and making the outcome more predictable in that we get the software on time and at the agreed upon amount of money.   This does not seem unique to software.  Using the idea of a house or other constructive efforts discuss what we might do to lower risk and improve predictability.  Then provide some examples of the effort despite best intentions not going right.  Be specific and vivid to see how this all may go back to a sense of betting. <br>

4. Which process model makes sense? <br>
 	* Given a particular description of a domain, organization, team, type of software, etc. can you make reasonable suggestions for what type of formality and process we should employ.  <br>

	* This is a fairly common sense type of question, if you allow yourself to think with at a broader level.  For example, do you think a very regulated environment would be ok with a process model with few artifacts?  If you were in a start-up environment would a heavy planning and documentation approach make sense?  <br>
 
5. The Cone of Uncertainity <br>
	* The cone of uncertainity seems to express a simple idea, explain what it is attempting to explain.  Now express why it always being reducing in size might not be accurate view of project reality.  Provide specific statements to show you are applying this to a real world software development situation.
<br>

6. Applied Iron Triangle <br>
	* You are presented a diagram of the Iron Triangle filled in or not and you need to explain how it relates to your team project.  You may be asked to do calculations such as developer availability (person hours) and relate it to features showing how estimating effort now becomes very important despite the fact that estimates often can't be precisely done without <br>

7. Thinking in Bets <br>
	* Much of engineering, software or other forms, is about managing risk.  We would like to accomplish some task and there is likely some risk that we will not succeed.  In some sense, our choices during our engineering process are like bets.  To show your understanding of how you might employ Thinking in Bets write a concrete example of a Software Project decision you might need to make and frame it with the idea of a cost,  a reward, and some % risk.  Provide an example, of a good bet and a bad bet so you demonstrate the thought model.
<br><br>

---
[Go Back](#cse-110-midterm-study-guide)
---

### Markdown, HTML, CSS

* [Lecture: Markdown](https://houses-pay-526.craft.me/I8G9rRG3qhNH9u) <br>

* [Lecture: HTML](https://houses-pay-526.craft.me/jKugncuIJRjTOT) <br>

* [Lecture: CSS](https://houses-pay-526.craft.me/qAdkHygjGuo1Vx) <br>

---
