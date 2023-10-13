# My API

# API Name
Sample Name API

This API provides functionality to manage and interact with a list of names. It allows users to perform actions such as inserting, updating, retrieving, and deleting names in a database.
 

## API Description
The Name API is designed to offer a simple way to manage a list of names in a database. It includes endpoints for creating, reading, updating, and deleting names. It can be used in applications where you need to handle name-related data.


## API Endpoints
Insert Name
Endpoint: '/postName'
Method: POST
Description: Adds a new name to the database.
Request Payload: JSON data containing "fname" and "lname".
Response: JSON response with a status message ("success" or "error").

Get Names

Endpoint: '/getName' (http://127.0.0.1/api/public/getName)
Method: GET
Description: Retrieves a list of names from the database.
Response: JSON response with a status message ("success" or "error") and an array of name objects.
 
Update Name

Endpoint: '/updateName' (http://127.0.0.1/api/public/postUpdate)
Method: POST
Description: Updates an existing name in the database based on an ID.
Request Payload: JSON data containing "id," "fname," and "lname."
Response: JSON response with a status message ("success" or "error").

Delete Name

Endpoint: '/deleteName' (http://127.0.0.1/api/public/postDelete)
Method: POST
Description: Deletes a name from the database based on an ID.
Request Payload: JSON data containing "id."
Response: JSON response with a status message ("success" or "error").


## Request Payload
{
	“lname”: “hortizuela”,
	“fname”:”manny”
}


## Response
Success Respone
{“status”:”success”,”data”:{{“lname”; “hortizuela”, “fname”:”manny”}}}

 Error Response
 {"status": "error",
    "message": "An error message here"}


## Usage
1: Inserting a New Name
Suppose you want to add a new name to your database. You can use the "Insert Name" endpoint to achieve this. Let's say you want to add the name "Manny Hortizuela."
http://127.0.0.1/api/publi/postName

2. If you want to retrieve a list of names from the database. You can use the "Get Names" endpoint for this purpose.
http://127.0.0.1/api/publi/getName

3.Updating a Name
Suppose you need to update a name in the database. You can use the "Update Name" endpoint. For example, you want to change "Manny Hortizuela" to "Manuel Hortizuela".
http://127.0.0.1/api/publi/updateName

4.Deleting a Name
If you need to remove a name from the database, you can use the "Delete Name" endpoint. For instance, you want to delete "Manuel Hortizuela."
http://127.0.0.1/api/publi/deleteName

## License
No License


## Contributors
Professor Manny Hortizuela Provided the parts: Codes, Database, API, JSON, etc.

List
contributors or give credit to any external libraries or resources used.


## Contact Information

For inquiries and support, please contact at princesgapasin07@gmail.com
