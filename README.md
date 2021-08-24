docker compose up -d

1. Create the directory that will hold your entire app. From the root directory of your app, create server and front-end directories. cd into the server directory.


2. Create your server and verify that it works.


3. Create a database directory in your server directory.

4. Create your database and verify that it works. Make sure to link your database container's volume and your newly created database directory so that data can persist even after container removal.


5. Connect your database with your server and verify that you are getting back data from a query (notice that you always verify that each step is working before moving on. Keep doing this!). Make sure that your database is dropped (or tables truncated) and seeded with new data every time you start your containers. For example, your database shouldn't contain duplicate seeded entries after starting up your container several times.


6. HINT: Think about how you will automate starting your database and your server and seeding it with data. This will require multiple commands. How can you invoke multiple commands when you start your server?

7. Create a Dockerfile for your server. You should be able to run your server with a docker run ... command after you have built the image.

8. Navigate to the front-end directory and create your React app. Are you still verifying that things are working after every step?


9. Display the result of an AJAX request to your server in a <div>.


10. Create a Dockerfile for your React app.


11. In the root level of your app directory, one level up from your server and front-end directories, create a docker-compose.yml file to create and launch all of your services with a docker-compose up command.
