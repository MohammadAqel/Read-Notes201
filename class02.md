


# HTML

### Hypertext Markup Language (HTML) is the standard markup language for documents designed to be displayed in a web browser. It can be assisted by technologies such as Cascading Style Sheets (CSS) and scripting languages such as JavaScript.

*Web browsers receive HTML documents from a web server or from local storage and render the documents into multimedia web pages. HTML describes the structure of a web page semantically and originally included cues for the appearance of the document.*

*HTML elements are the building blocks of HTML pages. With HTML constructs, images and other objects such as interactive forms may be embedded into the rendered page. HTML provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items. HTML elements are delineated by tags, written using angle brackets. Tags such as <img /> and <input /> directly introduce content into the page. Other tags such as <p> surround and provide information about document text and may include other tags as sub-elements. Browsers do not display the HTML tags, but use them to interpret the content of the page.*

*HTML can embed programs written in a scripting language such as JavaScript, which affects the behavior and content of web pages. Inclusion of CSS defines the look and layout of content. The World Wide Web Consortium (W3C), former maintainer of the HTML and current maintainer of the CSS standards, has encouraged the use of CSS over explicit presentational HTML since 1997.*

# CSS

*Cascading Style Sheets, fondly referred to as CSS, is a simply designed language intended to simplify the process of making web pages presentable. CSS allows you to apply styles to web pages. More importantly, CSS enables you to do this independent of the HTML that makes up each web page.
CSS is easy to learn and understood but it provides powerful control over the presentation of an HTML document.*

## WHY CSS?

#### CSS saves time : You can write CSS once and reuse same sheet in multiple HTML pages.

#### Easy Maintainence : To make a global change simply change the style, and all elements in all the webpages will be updated automatically.

#### Search Engines : CSS is considered as clean coding technique, which means search engines won’t have to struggle to “read” its content.

#### Superior styles to HTML : CSS has a much wider array of attributes than HTML, so you can give a far better look to your HTML page in comparison to HTML attributes.

#### Offline Browsing : CSS can store web applications locally with the help of offline catche.Using of this we can view offline websites.

### CSS Syntax

#### A CSS comprises of style rules that are interpreted by the browser and then applied to the corresponding elements in your document.

#### A style rule set consists of a selector and declaration block.

# JavaScript

*JavaScript is a programming language that adds interactivity to your website. This happens in games, in the behavior of responses when buttons are pressed or with data entry on forms; with dynamic styling; with animation, etc. This article helps you get started with JavaScript and furthers your understanding of what is possible.*

### What is JavaScript?

*JavaScript ("JS" for short) is a full-fledged dynamic programming language that can add interactivity to a website. It was invented by Brendan Eich (co-founder of the Mozilla project, the Mozilla Foundation, and the Mozilla Corporation).*

*JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more!*

*JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort. These include:*

1. Browser Application Programming Interfaces (APIs) built into web browsers, providing functionality such as dynamically creating HTML and setting CSS styles; collecting and manipulating a video stream from a user's webcam, or generating 3D graphics and audio samples.

2. Third-party APIs that allow developers to incorporate functionality in sites from other content providers, such as Twitter or Facebook.

3. Third-party frameworks and libraries that you can apply to HTML to accelerate the work of building sites and applications.It's outside the scope of this article—as a light introduction to JavaScript—to present the details of how the core JavaScript language is different from the tools listed above. 
You can learn more in MDN's JavaScript learning area, as well as in other parts of MDN.

# Decisions and Loops

### Conditional Statements : Very often when you write code, you want to perform different actions for different decisions.

*You can use conditional statements in your code to do this.*

### In JavaScript we have the following conditional statements:

1. Use if to specify a block of code to be executed, if a specified condition is true

2. Use else to specify a block of code to be executed, if the same condition is false

3. Use else if to specify a new condition to test, if the first condition is false

4. Use switch to specify many alternative blocks of code to be executed

### Comparison Operators : Comparison operators are used in logical statements to deter mine equality or difference between variables or values.


*JavaScript if else and else if : Use the if statement to specify a block of JavaScript code to be executed if a condition is true. Use the else statement to specify a block of code to be executed if the condition is false.Use the else if statement to specify a new condition if the first condition is false.*

# How to Write a Git Commit Message

*A project’s long-term success rests (among other things) on its maintainability, and a maintainer has few tools more powerful than his project’s log. It’s worth taking the time to learn how to care for one properly. What may be a hassle at first soon becomes habit, and eventually a source of pride and productivity for all involved.*

*In this post, I am addressing just the most basic element of keeping a healthy commit history: how to write an individual commit message. There are other important practices like commit squashing that I am not addressing here. Perhaps I’ll do that in a subsequent post.*

*Most programming languages have well-established conventions as to what constitutes idiomatic style, i.e. naming, formatting and so on. There are variations on these conventions, of course, but most developers agree that picking one and sticking to it is far better than the chaos that ensues when everybody does their own thing.*

### A team’s approach to its commit log should be no different. In order to create a useful revision history, teams should first agree on a commit message convention that defines at least the following three things:

1. Style: Markup syntax, wrap margins, grammar, capitalization, punctuation. Spell these things out, remove the guesswork, and make it all as simple as possible. The end result will be a remarkably consistent log that’s not only a pleasure to read but that actually does get read on a regular basis.

2. Content: What kind of information should the body of the commit message (if any) contain? What should it not contain?

3. Metadata: How should issue tracking IDs, pull request numbers, etc. be referenced?

*Fortunately, there are well-established conventions as to what makes an idiomatic Git commit message. Indeed, many of them are assumed in the way certain Git commands function. There’s nothing you need to re-invent. Just follow the seven rules below and you’re on your way to committing like a pro.*

### The seven rules of a great Git commit message

1. Keep in mind: This has all been said before.
2. Separate subject from body with a blank line.
3. Limit the subject line to 50 characters.
4. Capitalize the subject line.
5. Do not end the subject line with a period.
6. Use the imperative mood in the subject line.
Wrap the body at 72 characters.
7. Use the body to explain what and why vs.

*Before now, I only used git commit -m "Fix X to allow Y to use Z" on my personal projects with just a subject and no extra description. This is great for small and clear fixes like git commit -m "Fix typo in README.md, but in cases of more extensive changes, you would need to add some extra details.*

### Editor method

*Run git commit without a message or option and it'll open up your default text editor to write a commit message.*

#### To configure your "default" editor:

*git config --global core.editor nano
This would configure Git to use nano as your default editor. Replace "nano" with "emacs," "vim," or whatever your preference is.*

*In the opened editor, the first line is the subject (short description), leave a blank line after it, and everything else is the extended description (body).*


## How to write good commit messages

*There are several conventions used by different teams and developers to write good commit messages. I'll only outline some general rules and tips for writing commit messages–you have to decide what convention you want to follow. And if you work for a company or contribute to open source, you have to adapt to their convention :).*

*For consistency, you can use one convention for work and another for personal projects as you might change jobs sometime, and the convention might also change.*

*Be sure to check out this thread for some amazing commit message conventions or add yours to help someone make a decision.*

*Here's a great template of a good commit message originally written by Tim pope*

#### Looks great, right? Here's how you can make yours great too:

1. Specify the type of commit:

. feat: The new feature you're adding to a particular application.
. fix: A bug fix.
. style: Feature and updates related to styling.
. refactor: Refactoring a specific section of the codebase.
. test: Everything related to testing.
. docs: Everything related to documentation.
. chore: Regular code maintenance.[ You can also use emojis to represent commit types].

2. Separate the subject from the body with a blank line.
3. Your commit message should not contain any whitespace errors.
4. Remove unnecessary punctuation marks.
5. Do not end the subject line with a period.
6. Capitalize the subject line and each paragraph.
7. Use the imperative mood in the subject line.
8. Use the body to explain what changes you have made and why you made them.
9. Do not assume the reviewer understands what the original problem was, ensure you add it.
10. Do not think your code is self-explanatory.
11. Follow the commit convention defined by your team.