# NP HTML5, CSS3, and JavaScript 6e
# Tutorial 10, Review

## Instructions:
```
Description	Pts	Your Score
1.  Use your editor to open the lht_events_txt.html and lht_table_txt.js files from the html10 c review folder. Enter your name and the date in the comment section of each file, and save them as lht_events.html and lht_table.js respectively.	2
2.  Go to the lht_events.html file in your editor. Directly above the closing </head> tag, insert script elements that link the page to the lhtjist.js and lht_table.js files in that order. Defer the loading and running of both script files until after the page has loaded.	2
3.  Scroll down the document and, directly after the closing </article> tag, insert a div element with the ID eventList. It is within this element that you will write the HTML code for the table of upcoming theater events. Close the file saving your changes. (Hint: Be sure to review this file and all the support files, noting especially the names of variables that you will be using in the code you create.)	2
4.  Go to the lht_table.js file in your editor. Below the comment section, declare a variable named thisDay containing the date August 30, 2018. You will use this date to test your script.	2
5.  Create a variable named tableHTML that will contain the HTML code of the events table. Add the text of the following HTML code to the initial value of the variable:
    <table id='eventTable'>
    <caption>Upcoming Events</caption> <tr><th>Date</th><th>Event</th><th>Price</th></tr>	4	
6.  Lewis only wants the page to list events occurring within 14 days after the current date. Declare a variable named endDate that contains a Date object that is 14 days after the date stored in the thisDay variable. (Hint: Use the new Date() object constructor and insert a time value that is equal to thisDay.getTime() + 14*24*60*60*1000.)	4	
7.  Create a for loop that loops through the length of the eventDates array. Use i as the counter variable.	2	
8.  Within the for loop insert the following commands in a command block:
    a.  Declare a variable named eventDate containing a Date object with the date stored in the ith entry in the eventDates array.
    b.  Declare a variable named eventDay that stores the text of the eventDate date using the toDateString() method.
    c.  Declare a variable named eventtime that stores the text of the eventDate time using the toLocaleTimeString() method.
    d.  Insert an if statement that has a conditional expression that tests whether thisDay is <eventDate and eventDate < endDate. If so, the event falls within the two-week window that Lewis has requested and the script should add the following HTML code text to the value of the tableHTML variable.
        <tr>
        <td>eventDay @ eventTijne</td>
        <td>description</td>
        <td>price</td>
        </tr>
    where eventDay is the value of the eventDay variable, eventTime is the value of the eventTime variable, description is the ith entry in the eventDescriptions array, and price is the ith entry in the eventPrices array.
9.  After the for loop, add the text of the HTML code </table> to the value of the tableHTML variable.
10.  Insert the value of the tableHTML variable into the inner HTML of the page element with the ID eventList.
11.  Document your code in the script file using appropriate comments.
12.  Save your changes to the file, and then load the lht_events.html file in your browser. Verify that the page shows theater events over a two-week period starting with Friday, August 31, 2018 and concluding with Wednesday, September 12, 2018
```






