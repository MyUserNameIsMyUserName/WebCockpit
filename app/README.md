# REST API Auth JWT Example

**Replace API url inside index.php 

**change htaccess to link to new location if needed

---------------------------------------------------

**Start PHP Server in project root**

	php -S localhost:8080

**Create user**
	
	http://localhost:8080/api/create_user.php

With request body data

	{
    	"firstname" : "test",
    	"lastname" : "testic",
    	"email" : "test@dummymail.com",
    	"password" : "555"
	}

**Login user**

	http://localhost:8080/api/login.php

Enter in body
	
	{
    "email" : "test@dummymail.com",
    "password" : "555"
	}

**Test token access**

	http://localhost:8080/api/validate_token.php

Enter in request body

	{
    "jwt": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOlwvXC9sb2NhbGhvc3Q6ODA4MFwvIiwiYXVkIjoiaHR0cDpcL1wvbG9jYWxob3N0OjgwODBcLyIsImlhdCI6MTM1Njk5OTUyNCwibmJmIjoxMzU3MDAwMDAwLCJkYXRhIjp7ImlkIjoiMiIsImZpcnN0bmFtZSI6Ik1pa2UiLCJsYXN0bmFtZSI6IkRhbGlzYXkiLCJlbWFpbCI6Im1pa2VAY29kZW9mYW5pbmphLmNvbSJ9fQ.nyMRPlg0MSI_8xevui3aeW9suDHjBA6PWk05igYT_OY"
	}

**Update user**

	http://localhost:8080/api/update_user.php

Body has the following details

	{
	    "firstname" : "test",
	    "lastname" : "testic",
	    "email" : "test@dummymail.com",
	    "password" : "555",
		"jwt": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOlwvXC9sb2NhbGhvc3Q6ODA4MFwvIiwiYXVkIjoiaHR0cDpcL1wvbG9jYWxob3N0OjgwODBcLyIsImlhdCI6MTM1Njk5OTUyNCwibmJmIjoxMzU3MDAwMDAwLCJkYXRhIjp7ImlkIjoiMiIsImZpcnN0bmFtZSI6Ik1pa2UiLCJsYXN0bmFtZSI6IkRhbGlzYXkiLCJlbWFpbCI6Im1pa2VAY29kZW9mYW5pbmphLmNvbSJ9fQ.nyMRPlg0MSI_8xevui3aeW9suDHjBA6PWk05igYT_OY"
	}					
