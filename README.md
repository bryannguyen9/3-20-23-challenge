# Horiseon Landing Page Accessibility Code Refactor

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |  

## Description 

[Visit the Deployed Site](bryannguyen9.github.io.3-20-23-challenge)

This project was started with the goal in mind to make this landing page more accessible to those with disabilities. This is the Horiseon Social Solution Services landing page that focuses primarily on search engine optimzation, online repuatation management, and social media marketing. The end result was a code refactoring of the landing page that created a more accessible and intuitive page that did not visually change or alter functionality. 

This solves the problem of meeting accessibility standards for Horiseon as they are trying to be more impactful, accessible, and welcoming to all reaches around the world.

In this project I learned a lot about the methodology and thinking behind code refactoring, as well as HTML semantic elements that brought extra functionality and accessibility to HTML pages.

My project stands out because of the clean addition to nav links, section instead of div tags, and alt attributes to images that create a more dynamic experience for those with accessibility needs or that use screen readers.

Again here is a link to my fully deployed website: 
![Site Landing Page](bryannguyen9@github.io/3-20-23-challenge)

## Table of Contents

* [Code Refactor Example](#code-refactor-example)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Author Info](#author-info)
* [Credits](#credits)
* [License](#license)

## Code Refactor Example

What are the steps required to install your project? Provide a step-by-step description of how to get the development environment running.

```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

Converting the above non-semantic div with the class of 'header' to an appropriate [<header> semantic element](https://www.w3schools.com/html/html5_semantic_elements.asp). 

```html
      <header>
        <h1>Hori<span class="seo">seo</span>n</h1>
            <nav>
                <ul>
                    <li>
                        <a href="#search-engine-optimization">Search Engine Optimization</a>
                    </li>
                    <li>
                        <a href="#online-reputation-management">Online Reputation Management</a>
                    </li>
                    <li>
                        <a href="#social-media-marketing">Social Media Marketing</a>
                    </li>
                </ul>
            </nav>
    </header>
```

This change require some additional modification to the CSS selector: 

```css
.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}
```

No longer targeting the element on the page with the class of 'header' but instead the css selector targeting the 'header' element 

```css
header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

```

<!--Ended here-->

## Usage 

Provide instructions and examples for use. Include screenshots as needed. 

To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:

```md
![alt text](assets/images/screenshot.png)
```


## Learning Points 


This is a good place to Explain what you Learned by creating this application.
This is a great way to remind about all of the Complex Skills you now have.
If the user is less experienced than you:
They will be impressed by what you can do!

If the user is more experienced than you:
They will be impressed by what you can do!

Remember, it is easy to forget exactly how Valuable and Impressive your skills are, as well as How Much You’ve Learned!
So quantify that here!


## Author Info

```md
### Farley Wittles 


* [Portfolio](https://youtu.be/bHX54GCrDB4)
* [LinkedIn](https://youtu.be/bHX54GCrDB4)
* [Github](https://youtu.be/bHX54GCrDB4)
```

The user has looked through your whole README, and gotten familiar with your application. 
This is where you take credit, and make it easy for them to learn more about you!
Direct them to the following:
- Your GitHub Profile
- Your LinkedIn
- Your Portfolio Website
- And Anything Else You Want!

Give credit where credit is due! 

If you Pseudocode or Pair Program with someone else, give them kudos in your Contributors section!


## Credits

List your collaborators, if any, with links to their GitHub profiles.

If you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.

If you followed tutorials, include links to those here as well.


## License

The last section of a good README is a license. This lets other developers know what they can and cannot do with your project. If you need help choosing a license, use [https://choosealicense.com/](https://choosealicense.com/)


---

🏆 The sections listed above are the minimum for a good README, but your project will ultimately determine the content of this document. You might also want to consider adding the following sections.

## Badges

![badmath](https://img.shields.io/github/languages/top/nielsenjared/badmath)

Badges aren't _necessary_, per se, but they demonstrate street cred. Badges let other developers know that you know what you're doing. Check out the badges hosted by [shields.io](https://shields.io/). You may not understand what they all represent now, but you will in time.

## Features

If your project has a lot of features, consider adding a heading called "Features" and listing them there.

## Contributing

If you created an application or package and would like other developers to contribute it, you will want to add guidelines for how to do so. The [Contributor Covenant](https://www.contributor-covenant.org/) is an industry standard, but you can always write your own.

## Tests

Go the extra mile and write tests for your application. Then provide examples on how to run them.

---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.

* **User Story**: This is a short, simple description of a feature told from the perspective of the person who is requesting the new capability, usually a user or customer of the system. This follows an AS AN / I WANT / SO THAT format. For example, "AS A shopper visiting an online store, I WANT to place items in a shopping cart, SO THAT I can purchase them." 

* **Acceptance Criteria**: These are the requirements that you must meet to satisfy the scope of work. They are not exhaustive, but they do entail the minimum aspects of a working solution. Consider this a checklist of baseline requirements. Acceptance criteria can be presented in various ways. In this case, we'll use a common format called **scenario-oriented criteria** which expresses each requirement in a WHEN / THEN format. Don't worry if this doesn't make sense now; it will become very familiar to you after you complete a couple of Challenges. 

* **Mock-up**: This is an image or animation that demonstrates the design and functionality of the web application that you'll build for the Challenge.

* **Submission**: You'll submit your completed Challenge for review. In the real world, when a developer finishes working on a project, another developer reviews the code, providing feedback on errors and making sure that all of the acceptance criteria have been met. For each Challenge, you will need to be your Quality Assurance. Check to make sure you have met all acceptance criteria prior to your submission for review.

## Your Task

This week is an odd-numbered week, so your Challenge is an on-the-job ticket&mdash;meaning that you'll begin with starter code that you need to modify. 

**Refactoring** existing code (improving it without changing what it does) to meet a certain set of standards or to implement a new technology is a common task for front-end and junior developers. For this particular Challenge, a marketing agency has hired you to refactor an existing site to make it more accessible. 

> **Important**: When working with someone else's code, you should adhere to the **Scout Rule**&mdash;always leave the code a little cleaner than when you found it.

An increasingly important consideration for businesses, web **accessibility** ensures that people with disabilities can access a website using assistive technologies like video captions, screen readers, and braille keyboards. Accessibility is good for business&mdash;for one thing, accessible sites rank higher in search engines like Google. It also helps companies avoid litigation, which might arise if people with disabilities can't access a website.

Accessibility can include complex requirements, but your tech lead has given you a small list of specific criteria for this project. These criteria are documented in the Acceptance Criteria section.

To impress clients, you should always exceed expectations and improve the codebase for long-term sustainability. For example, check that all links are functioning correctly. You can also increase the efficiency of the CSS by consolidating the selectors and properties, organizing them to follow the semantic structure of the HTML elements, and including comments before each element or section of the page.

Are you ready to begin? Here are this week's Challenge requirements.

## User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the icon and image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## Mock-Up

The following image shows the web application's appearance and functionality:

![The Horiseon webpage includes a navigation bar, a header image, and cards with text and images at the bottom of the page.](./Assets/01-html-css-git-homework-demo.png)

> **Note**: This layout is designed for desktop viewing, so you may notice that some of the elements don't look like the mock-up at a resolution smaller than 768px. Eventually you'll learn how to make elements responsive so that your web application is optimized for any screen size.

## Getting Started

Follow these instructions to create your project and deploy it to GitHub Pages:

1. Create a new repository on your GitHub account and clone it to your computer.

2. When you're ready to deploy, use the `git add`, `git commit`, and `git push` commands to save and push your code to your GitHub repository.

3. Navigate to your GitHub repository in the browser and then select the Settings tab on the right side of the page.

4. On the Settings page, scroll down to the GitHub Pages section. Then, in the section labeled Source, select the `main` branch as your source.

5. Navigate to <your-github-username.github.io/your-repository-name> and you will find that your new webpage has gone live! For example, if your GitHub username is "lernantino" and the project is "css-demo-site", then your URL would be <lernantino.github.io/css-demo-site>.

You can also refer to this [YouTube video on enabling GitHub Pages](https://youtu.be/P4Mu1t5rIXg) for more guidance.

> **Important**: It might take a few minutes for GitHub pages to display your site correctly. If your project does not deploy or display correctly, check that all file paths in your application are relative and use the right casing. GitHub is case-sensitive, an inccorect capital or lowercase letter could cause problems in deployment.

Be sure to add, commit, and push your work to see the most up-to-date version of your app!

## Grading Requirements

> **Note**: If a Challenge assignment submission is marked as “0”, it is considered incomplete and will not count towards your graduation requirements. Examples of incomplete submissions include the following:
>
> * A repository that has no code
>
> * A repository that includes a unique name but nothing else
>
> * A repository that includes only a README file but nothing else
>
> * A repository that only includes starter code

This Challenge is graded based on the following criteria: 

### Technical Acceptance Criteria: 40%

* Satisfies all of the preceding acceptance criteria plus the following code improvements:

  * Application's links all function correctly.

  * Application's CSS selectors and properties are consolidated and organized to follow semantic structure.

  * Application's CSS file is properly commented.

### Deployment: 32%

* Application deployed at live URL.

* Application loads with no errors.

* Application GitHub URL submitted.

* GitHub repository contains application code.

### Application Quality: 15%

* Application resembles mock-up provided in the Challenge instructions (at least 90%).

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming conventions.

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Repository contains quality README file with description, screenshot, and link to deployed application.

## Review

You are required to submit the following for review:

* The URL of the deployed application.

* The URL of the GitHub repository, with a unique name and a README that describes the project.

---
© 2022 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.