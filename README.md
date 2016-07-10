# VeronaSched

Changing day codes for future years->
Follow a simple format for the day codes. They will be stored as an array of integers and are located in the school year java class. The format is MONTH DAY CODE. Month is either a 1 or 2 digit number (1 for January and 11 for November). Day is always a two digit number (EX: 02 or 25 or 13) and is directly appended to the end of the month. Finally, there is the code which corresponds to the day type (Day 2, late starts, etc…). This too is appended to the end of the month and day to form a complete day code.

Changing bell schedules for different times and formats->

In the bell schedule java class, you will find a bunch of bell schedules listed as instance variables under the class header which are arrays of String values. The arrays are then set in the many “if” statements based on the day type and advisory schedule (A or B lunch). If these bell schedules have changed since the previous year, simple alter the start and end times. Make sure that between the class name and the start/end times there is a “space colon span”. This is important because the list view in the schedule fragment uses string manipulation (.substring(start, end) to separate the name from the class times.

Saving classes in the settings fragment->

We are using a try catch system to save the classes to a file. This involves serialization and file input/output streams. Make sure that the you use the write to file class to write from the file. This is because file input and output steams require the class to extend Activity to have writing privileges to a file, and it ensures that the context of the file never changes. Simple use the methods already provided in the write to file class to access these

SQL Database->

We used a SQL database for storing the advisory and A+ customization for the user. This is used rather than a file output/input stream because of the ease of use to write to the SQL database. To access this database (in the MySqlHelper.java class) you need to make an object of this class to have access to the predefined methods we made in this java class. With SQL databases, remember that the queries are case sensitive and require a very specific format, so make sure to research this query format before messing with this class.

Git and bitbucket->

Always make sure that you are backing up to the bitbucket page. This will save you a lot of time and is a nice reference for version and is easy to revert back to old versions. We recommend that you look up videos on youtube to gain an understanding for bitbucket.

Any questions, email Nick B, nicklt80@gmail.com, or Jack B, guitar423@gmail.com

What is this repository for?

This repository holds the information need to make the greatest VAHS scheduling app in the history.

How do I get set up?

Setup is very easy, all you have to do is download the project and open it in Android Studio. Then you build the project and move the APK file to your phone or an emulator on your computer.

Contribution guidelines

Please contact the Admins before you make any changes to the code being specific in what exactly you want to change or add.

Who do I talk to?

Jack Butler (guitar423@gmail.com) or Nick Buchert (nickctl80@gmail.com)
