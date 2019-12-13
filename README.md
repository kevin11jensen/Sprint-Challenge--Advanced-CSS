Sprint Challenge: Advanced CSS - Space Walkers Web Page

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.
Instructions

Read these instructions carefully. Understand exactly what is expected before starting this Sprint Challenge.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.
Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.
Description

The client for this challenge is Spacewalkers Magazine. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

Click here to review the home design

Click here to review the mobile design
Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

    What is the difference between an adaptive website and a fully responsive website?

    Describe what it means to be mobile first vs desktop first.

    What does font-size: 62.5% in the html tag do for us when using rem units?

    How would you describe preprocessing to someone new to CSS?

    What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section will prevent you from passing this challenge.
Project Set Up

Follow these steps to set up your project:
Git Set up

    Create a forked copy of this project.
    Add your project manager as collaborator on Github.
    Clone your OWN version of the repository (Not Lambda's by mistake!).
    Create a new branch: git checkout -b <firstName-lastName>.
    Implement the project on your newly created <firstName-lastName> branch, committing changes regularly.
    Push commits: git push origin <firstName-lastName>.

Follow these steps for completing your project.

    Submit a Pull-Request to merge Branch into master (student's Repo). Please don't merge your own pull request
    Add your project manager as a reviewer on the pull-request
    Your project manager will count the project as complete by merging the branch back into master.

Preprocessor Set up

    Verify that you have LESS installed correctly by running lessc -v in your terminal, if you don't get a version message back, reach out to your project manager for help.
    Open your terminal and navigate to your preprocessing project by using the cd command
    Once in your project's root folder, run the following command less-watch-compiler less css index.less
    Verify your compiler is working correctly by changing the background-color on the html selector to red in your index.less file.
    Once you see the red screen, you can delete that style and you're ready to start on the next task

Minimum Viable Product

Your finished project must include all of the following requirements:
Import LESS Files

    Navigate to your index.less file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less

You will know everything is working properly when you see the styles enabled for the provided content.
Home Page - Desktop HTML & LESS

    Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

    Add a viewport meta tag to the head of your index.html page

    Review the provided home desktop design file. You are to build the missing navigation system and header image. You have been provided all content necessary in the index.html file

    Navigation Styles: Use the navigation.less file for styling.

    Main Content Styles: Use the home-page.less file for styling

    LESS Mixins: Create and use 2 different mixins to aid your styling. Use the mixins.less file for your mixins

    LESS Parametric Mixin: create a parametric mixin that is used to create the sign up button styles.

    Use at least 2 parameters to create your button

    Create a hover state that swaps the background color and font color of the base button styles.

Mobile Design

    Create a @phone variable that contains a max-width: 500px media query string. Use the @phone variable for all your nested mobile styling.

    Review the provided home mobile design file. Match your mobile styling the best you can using the design file.

    Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.
Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

    Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

    Introduce CSS animations to your site.

    Create a fixed navigation and add some opacity to the background

    Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription





Self-Study questions for Sprint 2



    What is the difference between an adaptive website and a fully responsive website?

	An adaptive website adapts to screen sizing but has no breakpoints so it doesn't
	re-arrange elements at certain sizes like a fully responsive site with breakpoints.
	With breakpoints you can set a specific screen size for elements on your page to 
	move into different places, or just change any element in general, when the user's
	screen reaches a certain size in pixels.

    Describe what it means to be mobile first vs desktop first.

	Desktop first design means using "max-width" in your @media breakpoints because you are
	designing from the desktop version down. You start at the max-width size of a desktop and
	as the user resizes their screen, the website will hit a specified breakpoint as the screen
	is sized down, and the elements on the screen will change according to the max-width of the 
	screeen. It scales down from desktop, to tablet, to mobile in most cases. Mobile first is
	the opposite direction of screen sizing. Instead of sizing down, you are building for a small
	screen first and then sizing up to desktop. For this you would use "min-width" for the 
	@media breakpoints because you are sizing up.

    What does font-size: 62.5% in the html tag do for us when using rem units?

	"font-size: 62.5%" when placed in the html tag, makes all fonts scale down to 62.5% of their
	inherit size which is 16px. The reason we do this because 62.5% of 16px equals 1rem which 
	equals 10px. If 1 rem equals 10px for the entire document, the our math for sizing fonts gets
	much easier because 1.6rem now equals 16px and our font-sizing is fully responsive.

    How would you describe preprocessing to someone new to CSS?

	When you're new to CSS you quickly learn that in order to access elements within elements you
	have to write it out long form. To get to an element within an element that is also within an
	element you have to write out the path to reach it. Instead of doing that, you can use a 
	compiler that automatically writes your CSS for you while you write your code into the 
	compiler using their rules to make your code more readable. In this example, the idea
	of being able to nest your elements within parent elements directly in your CSS, is called:
	nesting.

    What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?
    
	My favorite concept in preprocessing, if I had to pick one, is importing different less files
	to seperate the different sections of the document in CSS. If I want to style the navigation
	I simply go to the "navigation.less" file and style the navigation there. This makes it so I 
	can just look at a few lines of code, or just the code for that individual section, instead 
	of searching through thousands of lines of code. The original index.css file can have 
	thousands of lines of code in it, making it very tedious to have to find certain styled
	sections of your document.
