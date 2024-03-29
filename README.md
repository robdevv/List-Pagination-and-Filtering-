# List-Pagination-and-Filtering-
Project 2
 10 steps
Seeking assistance

If you're having trouble with a bug or moving forward with the project:
Reach out to your Slack team.

Pro Tip: A good “Help!” Slack post begins with a friendly greeting, details any important info like the problem you’re having, what you’ve tried so far to fix it, and a link to your repo.

Take a look at this great study guide: List Pagination and Filter Study Guide

Review the unit material.
Practice your Google skills by rephrasing your question in Google until you find helpful results.
No snippets, plugins or libraries, including jQuery

For this project, avoid using the popular jQuery library. All code for this project must be your own, and must be plain JavaScript, often referred to as "vanilla" JavaScript.
Avoid using any other libraries, plugins or code snippets for any aspect of this project, including the pagination.

Create your global variables
This project can be completed with just two global variables
Create a variable to store the student list item elements in the student list.
Pro Tip: Log out the variable storing the list to ensure it equals the list of li items and not the container of the li elements.
Create a variable to store the number of items to show on each “page”, which for this project, is 10.

Display a “page”
Create a function to hide all the students except for the ten you want displayed on a given page.
This function should have two parameters:
The list parameter to represent the actual list of students that you’ll pass in as an argument later when you call this function.
The page parameter to represent the page number that you’ll pass in as an argument later when you call this function.
Inside the function:

Create two variables to store the start index and the end index of the list items to be displayed on the given page. To make this function dynamic and work with a list of any length, a bit of basic math can be used to determine these values.
Start Index = (page parameter * items per page) - items per page
End Index = page parameter * items per page
Loop over the list parameter.
Inside the loop, display any list item with an index that is greater than or equal to the start index variable and less than the end index variable.
Pro Tip: If you call this function in the early stages of building the function, you’ll be able to use log statements and the Chrome dev tools console to test and check that variables, values and indexes are what you think they are.

Project Warm Ups: Creating and using functions, and selecting and manipulating sections of a list can feel confusing at first. For some helpful practice, check out the project Warm Ups List Section Selection and What's the Deal with Functions.
Add pagination links

Create a function that creates and appends functioning pagination links.
This function should accept a single list parameter to represent the actual list of students that you’ll pass in as an argument later when you call this function.
Inside the function:

Create and append the DOM elements for the pagination links.
Use lines 119-137 in the examples/example-meets.html file as your template.
Pay close attention to how elements are nested, any necessary class names or other element attributes, and where your additions should be appended.

You should end up with:
A container DIV element with a class name of “pagination”, and appended to the div element with the class name of page.
A nested UL element containing one LI element for every ten students in the list.
Pro Tip: You can divide list.length by the max number of items per page to figure out how many pages are needed, and you can use a loop that iterates that many times to create the correct number of LI elements.
Each LI element should contain an A element with an href attribute of #, and text set to the page number each link will show. First link is 1. Second link is 2. And so on.
Pro Tip: The loop index can be helpful in setting the text of the pagination links.
Add the active class name to the first pagination link initially.
Add a “click” event listener to each A element. A loop can be helpful here.
When a pagination link is clicked:
The active class name should be removed from all pagination links. A loop can be helpful for this step.
The active class name should be added to the link that was just clicked. The target property of the event object should be useful here.
The function to show a page should be called, passing in as arguments, the global variable for the list items, and the page number that should be shown. The text content of the A element that was just clicked can be helpful here.
Note: Your program needs to work for any number of list items, so your solution needs to be dynamic. You can test that your solution works for any size list by opening the examples/44students.html and examples/64 students.html files, and linking your JS file.
Project Warm Ups: DOM manipulation and updating an indication that a button is active can be tricky at first. For some helpful practice, check out the project Warm Up Fun DOM Manipulation and Where's the Action.

Call your functions
Call the show page function, passing in as arguments, the global variable for the list items, and the number 1 for the first page, which should be shown initially.
Call the append page links function, passing in as an argument, the global variable for the list items.

Add code comments
Replace the code comments in the file with your own code comments.
The key to creating good code comments is to keep them brief, but clear, so that your fellow developers can get an idea of what's going on in your code at a glance, without having to review every line of your code.
Review the "How you'll be graded" section
Check out the "How you'll be graded" section, located above, next to the instructions tab, just below the project title. This section lists specifically what will be considered and checked when your project is being reviewed, and your project grade is being determined.

Quality Assurance and the Student Project Submission Checklist
Open your project in one or more browsers, at least Chrome, and click every button, and test every feature.
Take the time for thorough quality assurance testing. Before you submit your project for review, please check off all of the items on the Student Project Submission Checklist.
Share your project in Slack in the #review-my-project channel to get a preliminary review and catch anything you might have missed.
NOTE: What you submit is what will get reviewed

When you submit your project, a snapshot is taken of your repository, and that is what the reviewer will see. Consequently, the reviewer won't see any changes you make to your repo after you submit the project.
Extra Credit
To get an "exceeds" rating, complete all of the steps below:

 4 steps
Add search component
Dynamically create and append a search bar. Avoid making any changes in the index.html file. You can reference the examples/example-exceeds.html file, lines 16-19, to see an example of the markup you'll create.
Add functionality to the search component
When the "Search" button is clicked, the list is filtered by student name for those that include the search value. For example, if the name Phillip is typed into the box, list all items with a name that includes Phillip. If the letter S is typed in, all items with an S in the name will show.

Pro Tip: To improve the functionality and add to the user experience, consider adding a keyup event listener to the search input so that the list filters in real time as the user types. This would be in addition to making the search button clickable since pasting text into the search bar might not trigger the keyup event.

Project Warm Up: Configuring a search feature can seem complex at first, but it's really just a few fundamental steps. For some helpful practice, check out the project Warm Up Simple Search.

Paginate search results
Display pagination links based on how many search results are returned. For example: if 10 or fewer results are returned, 0 or 1 pagination links are displayed. If 22 search results are returned, 3 pagination links are displayed.

Pro Tip: To paginate the search results, try storing the search results in an array that can act as a list, on which you can call your functions to show a page and append pagination links.

Handle no results returned
If no matches are found by the search, include a message in the HTML to tell the user there are no matches.

Note Don't use the built in alert() method here. The "No results" message must be printed to the page.

NOTE: Getting an "Exceed Expectations" grade.

See the rubric in the "How You'll Be Graded" tab above for details on what you need to receive an "Exceed Expectations" grade.
Passing grades are final. If you try for the "Exceeds Expectations" grade, but miss an item and receive a “Meets Expectations” grade, you won’t get a second chance. Exceptions can be made for items that have been misgraded in review.
Always mention in the comments of your submission or any resubmission, what grade you are going for. Some students want their project to be rejected if they do not meet all Exceeds Expectations Requirements, others will try for all the "exceeds" requirement but do not mind if they pass with a Meets Expectations grade. Leaving a comment in your submission will help the reviewer understand which grade you are specifically going for
