QuickUser.js
============

A quick user management class implemented in Javascript. There are two
versions, one that uses a cookie and another that uses HTML 5 local storage. 

The class creates a new user ID, if one wasn't already created, and stores an
array of user information. Additional key / value pairs can be added by the
programmer. No user id or password is required making login unnecessary. Login
credentials could be easily added and tracked, however.

In order to use the library, simply include the QuickUser.js file into your
HTML document.

    <script type="text/javascript" src="quickuser.js"></script>

Then, in your documents JavaScript create an instance of the QuickUser object.

    <script type="text/javascript">
 
      // Load a user using the QuickUser class
      user = new QuickUser();
 
      // Read the user ID that was assigned
      var id = user.get("id");
 
      // Read the number of hits
      var hits = user.get("hits");
 
      // Set your own variable
      user.set("first", "Joel");
 
    </script>

This source code is distributed under the open source MIT License.
