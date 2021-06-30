Create Fake Json Server
We will be using the Fake Json Server for storing and retrieving our data locally. I am using it because our application is small and we will be storing and retrieving the data later on. Install Json Server with following command.


npm install -g json-server
Create a folder named Server and create a file named db.json to record our data. We create a users collection in db.json which will be holding our users data later on.


{
 "users": []
}
Next thing you need to do is to create json-server.json file to the root of the project and it will hold port for our server.


{ 
"port": 5000
}
For running the json server you run following command on your terminal. Keep your server running.


json-server --watch server/db.json
