# BirdieBucksBackend
This repository is created for a backend I designed in java for a stock trading android application.

This app was a semester long effort with 2 individuals working on the frontend and myself and another working on the backend.
I was unable to port this over from my school's gitlab so I have just brought over the backend files that I contributed to, and I included a html of the commits from the whole semester.

The backend of this app was developed with springboot and maven through the IntelliJ IDE. The pom.xml has all dependencies necessary to run the application through the main.java in the src folder.
Upon execution a .idea folder will be created with a ton of files as well as a .gitignore file.

The backend had several different types of users being regular users, group leaders, and administrators.
The regular users could view their accounts and portfolios, as well as purchase stocks and be involved in different stock groups where they could communicate with others through websockets.
Group leaders had all of the same functionality but, could lead a group and were able to add, remove, and control the group that they owned. They could also give up their ownership of the group to a different user that was in the group.
Administrators had all the same functionality as above, but could also remove and add stocks to the market, ban users, and have the stocks auto-updated.

There were also many stocks added to the app that the users could purchase and sell to gain "money". Stocks were updated through 2 different apis. The first being AlphaVantage, which gave us access to update data like current price, change in the last 24 hours, news articles about the stocks, and the history of that stock. The other api utilized was called ClearBit. This allowed us to pull images from the web for each stock when they were added or deleted so we could display the logos of each stock to the user.

We used several repositories to store all of our data. This was done through MySQLWorkbench where we connected to our classes server to host the database and were able to view it locally on our machines.
