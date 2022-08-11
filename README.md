# MongoDB_Python_Tutorial
- ✅ Optional Database Environment Additional MongoDB inIt can be driven by Datalake data.
- ✅ Libraries can be run to work with MongoDB.
- ✅ can run Operation Database functionality such as Insert,Can Update, Upsert, Delete
### download and install “PyMongo” using the command “python -m pip install pymongo”

### connect MongoDB to Python

from pymongo import MongoClient
import pprint
printer = pprint.PrettyPrinter()
connection_string = "URL"
client = MongoClient(connection_string)

### Python MongoDB Create Database

client[“ Database_Name ”]  or client.Database_Name

### Python MongoDB Create Collection

    	database_name[“Collection_Name”]  or database_name.Collection_Name

## Python MongoDB Insert Document
	2 method insert_one(), insert_many()

Collection_Name.insert_one({document})
Collection_Name.insert_many({document},{document},...)

### Python MongoDB Update
	2 method update_one(), update_many()

	Collection_Name.update_one({query},{"$set":{newvalues})
Collection_Name.update_many({query},{"$set":{newvalues})

### Python MongoDB Upsert

	Collection_Name.update_one({query},{"$set":{newvalues} , upsert=True )

### Python MongoDB Delete Document
	2 method delete_one({query}) ,delete_many({})

### Python MongoDB Find/Read Document 
	2 method Collection_Name.Find_one({query}) , Collection_Name.Find({})



