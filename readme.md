### MAKING A WEBSITE RESPONSIVE
---
# Task Board
---
In this project, you will create a board of to-do items organized into columns. All of the HTML and most of the CSS have been written for you, but the grid property declarations have yet to be added.


Tasks

1.
We will be focusing on laying out the container < div > and the two card-column < div >s within it. Here’s an abbreviated version of those < div >s in index.html:

<!-- <div class="container">
    <div class="card-column future-projects">
        ...
    </div>
    <div class="card-column active-projects">
        ...
    </div>
</div> -->
Right now, the task board looks pretty cluttered. In style.css, let’s make the < div > with class container a grid container so that we can start to arrange these tasks better.


Stuck? Get a hint
2.
That didn’t have any immediate effect, but it allows us to apply grid properties to the container div. Let’s start by giving the .container ruleset three equally sized columns by using the grid-template-columns property.

Note that only 2 of columns will be filled with content at this point.


3.
Now, let’s add a gap of 20 pixels in between the columns.


4.
Inside of each card column, there are 5 rows of task cards. We want the those to be arranged neatly within the columns as well, so let’s make each card column a grid container.

In style.css, within the .card-column ruleset, add a declaration that sets the display property to grid.


5.
Each card column has also has a heading above the 5 task cards. We want the heading to take up 20px and each task card to take up 100px.

Inside the .card-column ruleset, set the grid-template-rows property to have 1 20px row and 5 100px rows. Use the repeat function to make your code clean.


6.
In order to have the task cards spaced evenly in each card, inside .card-column, use the align-content property to set an even amount of vertical space around each card.


7.
Now we want to another card column for Completed Projects to keep track of all of the tasks we’ve already done. Let’s add a third card column that’s like the other two. We already have our container set to have space for three columns, so you just need to add the HTML.

In index.html, uncomment the code for the third card column.


8.
We expect to complete a lot of projects, but we don’t know how many. Since those projects will be added as task cards to the Completed Projects column, it will be helpful to use implicit grid properties instead of the explicit properties we have been using so far. We know the first row with the heading should be explicitly 20px, just as the other heading rows are. Every additional row, if it exists, should be implicitly set.

Inside .card-column, use the grid-auto-rows property to implicitly set rows to 100px.


9.
Good job! Now, feel free to play around with the layout of this site, using the other CSS properties you’ve learned. Once you’re satisfied with your work, press the Next Button to move on.