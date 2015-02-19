# s15_pivnik_data_lecture_notes12

Scaling With Traditional Databases:

Web analytics application

 -You might build a table with a column for id, user_id, url, pageview and another column of the types of data 

 -Deploy the system and it's a big success. Too big even.

 -Multiple clients tracking multiple pages.....errors begin.....clients are timing out when they attempt to notify your system of a page view. 

 -Decide the problem is that it's inefficient to have one ipdate to the database, asking it to update multiple rows with each request. 

 -You insert a queue beteween your web server and the code that will update the database.
 
 -Not a true solution. "band-aid" fix.
 

Solution:

 -The database is the BOTTLENECK, all users are still going through database.
 
 
 -So, two approaches. First is called "Vertical Scaling". Eventually will fail if you keep gaining popularity.
 
 -
