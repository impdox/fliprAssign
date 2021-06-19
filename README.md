"# flipr" 
"# flipr" 
# node-flipr

Install the dependencies by running this command-> "npm install"
followed by software or by any enviroment you want to install to like use 
mongo for Mongodb
Mongoose for Mongoose
express for Express.

To run in Development environment use this command-> "npm run dev"

To run in production environment use this command-> "npm run start"

This app has 2 POST request Apis

1st Api:    
You can make post request at "http://localhost:3000/process/devices?name=status" (For local testings)
 where "device" is a collection name of a mongodb passed as parameter, "status" is another collection name of mongodb passed as query parameter,
also you have to pass an json array containing one element, the url of the mongodb in the body, like this ["mongodb+srv://backendconcoxdeveloper:V3jUV7QXqEoAtnhy@cluster0-zhjde.mongodb.net/"] then it will return an object having keys of latest 30 device ids and corresponding arrays containing their latest 50 locations from older to latest order, also send 2 custom headers with the keys "Name" and "Contact"

2nd Api:    
You can make the post request at "http://localhost:3000/location" (For local testings) 
 by passing an array of address names in the body, like this ["Patna, India","Bihar, india","Kollam, india"] It will generate the latitude and longitude of them, also
 it returns the result if success, with the status code 200

note: can be deployed from deployed server too."# flipr" 
