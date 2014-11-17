MongoLogin
==========

Instead of using the built in session manager in python to display certain pages, this project attempts to create it's own session manager by storing 'authenticated' in the databse for each user. If authenticated is true then the user is logged in.

Modular, lightweight, powerful.

- **addUser**(name, password[, dbname[, dbCollectionName])

	Checks if username already exists in correct database and collection. If so, returns False. Otherwise registers a user under the given username and password.
- **login**(name, password[, dbname[, dbCollectionName])

	Check if username and password match in the correct database and collection. If so, returns True and updates *authenticated* to True. Otherwise, returns false.
- **logout**(name[, dbname, [dbCollectionName]])
	Sets the authenticated boolean of user to False.
- **updateUser**(name, authenticated[, dbname[, dbCollectioName])

	If the user is authenticated (logged in), this method can alter different variables of the user. If the change was successful, returns True. If it failed or the user wasn't authenticated, returns False.
- **isInDatabase**(name[, dbname, [dbCollectionName])

	If the user is located in the correct database and collection, returns True. Otherwise, return False.
=======
mongo-login-decorator
=====================
>>>>>>> bc0cf13981c118bf38d5b578adb76387dc54eea5
