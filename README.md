The primary audience is the one who wishes to get an update on annual car shows in Los Angeles.
The project has an option for an user to add, edit or delete shows. The post will be tracked for any edit changes, and all of edit history will be shown on the detail page. I will also implement a Google API to display a corresponding map for each show. On a show page, I will add a RSVP option by placing attending, not attending, and maybe attending buttons. The project will have an <*add*> route for adding a new show, a <*search*> route that searches for any shows with a delete button next to each show, and a <*detail*> route inside the search route that gives an edit button, map and detailed information about a selected show. In addition, the detail page has a function to mark the user's RSVP status. The <*edit*> route inside the detail route helps the user to make any edits and to display all of the edit history.

The add route will make a request via the POST/api/shows endpoint and add a new show.
The search route will make a request via the GET/api/shows endpoint to get a list of shows, and DELETE/api/shows/:id endpoint to delete a show. The detail route will make a request via the GET/api/shows/:id endpoint to get information about a show.
When the user clicks the edit button, the edit route will hit the PUT/api/shows/:id endpoint, and any changes will be displayed.
The request payloads: when the POST, GET, PUT, DELETE requests successfully execute,
The response payloads: the data that contains id, title, address, date, url, photo, description, and so on will respond.
If there are unsuccessful responses, the errors element will respond.

* I plan on using momentjs to display date and time and sorting shows in an ascending order.
