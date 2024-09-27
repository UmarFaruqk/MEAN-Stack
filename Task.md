# MEAN STACK
The MEAN stack is a JavaScript-based framework for developing scalable web applications. The term MEAN is an acronym for MongoDB, Express, Angular and Node

1. MongoDB (Document database) - Stores and allows to retrieve data.
2. Express (Back-end application framework) - Makes requests to Database for Reads and Writes.
3. Angular (Front-end application framework) - Handles Client and Server Requests
4. Node.js (JavaScript runtime environment) - Accepts requests and displays results to end user

## IN THIS PROJECT WE ARE GOING TO IMPLEMENT A SIMPLE BOOK REGISTER WEB FORM USIN MEAN Stack.

1. We create an Instance on our EC2 Engine 
2. Connect the instance to our Terminal using the following command ![reference image](/Pictures/pic1.PNG)
3. Now we use Nodejs to set up the express routes and AngularJS controllers using *sudo apt update* and *sudo apt upgrade* and you should see this ![reference image](/Pictures/pic2.PNG) and this ![reference image](/Pictures/pic3.PNG)
4. We the add certificates using the following command ![reference image](/Pictures/pic4.PNG)
5. Then finally we install NodeJS using ![reference image](/Pictures/pic5.PNG)
6. Next we install MongoDB because our record book needs to contain  book name, isbn number, author, and number of pages so we first run this command ![reference image](/Pictures/pic6.PNG) and ![reference image](/Pictures/pic7.PNG)
7. We then run the installation command ![reference image](/Pictures/pic8.PNG) and start the server ~[reference image](/Pictures/pic9.PNG)
8. We then verify the service is up and running using *sudo systemctl status mongod* and we should see this ![reference image](/Pictures/pic10.PNG)
9. Next we install the  Node package manager using *sudo apt install -y npm* and you should see this ![reference image](/Pictures/pic11.PNG)
10. The we install a *body-parser* package to help process JSON files passsed in request to the server using *sudo npm install body-parser* you should see this ![reference image](/Pictures/pic12.PNG)
11. Create a directory Books and Initialize npm project ![reference image](/Pictures/pic13.PNG) add a file to it named *server.js* then *vim server.js* and paste the following code ![reference image](/Pictures/pic14.PNG) save and exit
12. Next we will install Express and set up routes to the server, here we will use express to pass book information from our MongoDB database and we will also use  Mongoose package which provides a straight-forward, schema-based solution to model your application data. We run *sudo npm install express mongoose* ![reference image](/Pictures/pic15.PNG) 
13. In the Books folder we create a folder named *apps* and then create a file named routes.js ![reference image](/Pictures/pic15.PNG) now *vim routes.js* and pastes the following codes ![reference image](/Pictures/pic16.PNG)
14. Again in the *apps* folder create a folder named *models* and create a file named *books.js* ![reference image](/Pictures/pic17.PNG) then paste teh following codes ![reference image](/Pictures/pic26.PNG) 
15. Now we create an access routes with AngularJS so we can connect our web page with Express and perform actions on our book register but first we go back to our *Boosk* directory using *../..* 
16. Then we create a folder called *public* and then create a file in it called *scripts.js* ![reference image](/Pictures/pic18.PNG), *vim scripts.js* and paste the following codes ![reference image](/Pictures/pic19.PNG)
17. Create another file in the *public* folder called *index.html* the *vim index.html* and paste the following code ![reference image](/Pictures/pic20.PNG)
18. Now *cd ..* to the *Books* folder  and run *node server.js* you should see this ![reference image](/Pictures/pic21.PNG) which means the server is up and running but for us to access it in our browser we need to add port *3300* to our security group on the instance console ![reference image](/Pictures/pic23.PNG)
19. You can launch another terminal to test what *curl* command returns locally ![reference image](/Pictures/pic22.PNG)
20. After adding  port *3300* to the security group inbound rule we can now access our Book Register web Application from the internet using a browser of your choice and if everything is okay you should see this ![reference image](/Pictures/pic25.PNG) well i adsded a register to test if it works and as you can see it does 
    
## THANKS FOR FOLLOWING THIS CLASS I HOPE YOU ENJOYED THE RIDE 

