# journal


## Description

This is a note taker by Ben Honken.  It uses express to host a server and then stores your notes.  You may create and save new notes.  You may also view or delete old notes.  Each note has a unique ID equal to its index.  The ID is added as an ID in the html so that the appropriate note can be viewed or deleted on click.  When a note is deleted, all IDs are reassigned to ensure that they remain unique.  Most of the front end was provided, although some required slight modification.  

[requirementsAndSetup](screenshots/requirementsAndSetup.png)
This screenshot shows the setup of requirements, initialization of the starting notes, and setup of the server.  

[getCalls](screenshots/getCalls.png)
This screenshot shows the get calls for the notes.html page, the data, and the index.html page.  The index is a catchall, which is why it is last.  

[post](screenshots/post.png)
This screenshot shows the post call.  It takes in the data from the browser, assigns it an id, pushes it to the serverside database, and saves.  The front end then calls again to repopulate the updated list.  

[delete](screenshots/delete.png)
This screenshot shows the delete call.  The delete call is passed the id of the clicked element, splices that note out of the database, reassigns ids, and saves.  The front end then calls again to repopulate the updated list.  

[deleteFrontEnd](screenshots/deleteFrontEnd.png)
This screen shot shows the ajax call, and particularly how to assign data to the delete request in the front end.  

[getID](screenshots/getID.png)
This screenshot shows how I rewrote the delete and view functions to grab the id of the clicked element and pass them appropriately to the server.  

[listen](screenshots/listen.png)
This screenshot shows how to set up the listener.  

## Usage

As a user, I want to be able to store, organize, and delete my notes so that I can access them from anywhere and keep track of the things I am learning or the tasks I need to complete.  

## Credits

Ben Honken made this.

## License

MIT License

Copyright (c) [2019] [Ben Honken]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
