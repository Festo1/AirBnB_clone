# AirBnB Clone - The Console

This is a **clone of the AirBnB website**, implementing a custom command-line interface for managing objects like users, places, amenities, and reviews. 

## Getting Started

To launch the console application:

```
./console.py
```

## Description of the project

*The AirBnB clone project aims to create a replica of the Airbnb website and functionality. It will consist of:*

- **A custom command-line interface that allows manipulating data without a visual interface, like a shell. This will be used for development and debugging.**

- **A front-end website with both static and dynamic functionality.**

- **A comprehensive database to manage backend functions like storing data.**

- **An API that facilitates communication between the front-end website and backend database and logic.**

`The final product will be a full web application with a front-end website interfacing with a robust back-end through a custom API. The back-end will include a command interpreter for debugging and a database. The goal is to replicate core Airbnb functionality like user accounts, listing rentals, reviews, payments etc.`

## Aims & Objectives of this project
Once launched, you can use commands like:

- `create`: Create a new object (ex: `create User`)
- `Retrieval of an object from a file storage, a database etc… `
- `Perform operations on objects (count, compute stats, etc…)`
- `show`: Show an object's details (ex: `show User my_id`) 
- `all`: Display all objects of a type (ex: `all Users`)
- `update`: Update an object's attributes (ex: `update User my_id email "new@email.com"`)
- `destroy`: Destroy an object (ex: `destroy User my_id`)

## The created objects
**The list of the objects (instances) that can be created are as follows:**
- BaseModel
- User
- City
- Amenity
- State
- Review
- Place

### Further Resources:
* [HBNB videos](https://www.youtube.com/playlist?list=PLlLHfkTcnvmPOp6jv_89tRpJUMFrP-Wbi)
* [Holberton Airbnb overview](https://www.youtube.com/watch?v=QTwmCB_AWqI)
* [The Airbnb Console](https://www.youtube.com/watch?v=jeJwRB33YNg)
* [Airbnb ORM](https://www.youtube.com/watch?v=ZwCD8cNZk9U)
* [Airbnb API](https://www.youtube.com/watch?v=LrQhULlFJdU)
* [Final product](https://www.youtube.com/watch?v=m-cfupVumos)
* ```Other resource```
* [cmd module](https://docs.python.org/3.8/library/cmd.html)
    * ```packages concept page```
    * [Python packages](https://docs.python.org/3.4/tutorial/modules.html#packages)
    * [uuid module](https://docs.python.org/3.8/library/uuid.html)
    * [datetime](https://docs.python.org/3.8/library/datetime.html)
    * [unittest module](https://docs.python.org/3.8/library/unittest.html#module-unittest)
    * [args/kwargs](https://yasoob.me/2013/08/04/args-and-kwargs-in-python-explained/)
    * [Python test cheatsheet](https://www.pythonsheets.com/notes/python-tests.html)
    * [ AirBnB website.](https://www.airbnb.com/)

Type `help` to see all available commands.

## Commands Implemented
**Description of the command interpreter**
| Commands  | Description |
| ------------- | ------------- |
| ```quit```  | This command quits or exits the console  |
| ```EOF```  | This command quits or exits the console interpreter when pressed ```Ctrl+D``` |
| ```help``` or ```help <command>```  | Displays all commands or Displays instructions for a specific command (Ex: ```help``` or ```help quit```).
| ```create <class>```  | Creates an object of type, saves it to a JSON file, and prints the objects ID (Ex: ```create BaseModel``` or ```BaseModel.create()```)
| ```show <class> <ID>```  | Shows string representation of an object (Ex: ```show BaseModel 1234-1234-1234``` or ```BaseModel.show("1234-1234-1234"```))
| ```destroy <class> <ID>```  | Deletes an objects based on the class name and id (Ex: ```destroy BaseModel 1234-1234-1234``` or ```BaseModel.destroy("1234-1234-1234")```).
| ```all or all <class>```  | Prints all string representations of all objects or Prints all string representations of all objects of a specific class (Ex: ```all BaseModel``` or ```all or User.all()```).
| ```update <class> <id> <attribute name> "<attribute value>"```  | Updates an object with a certain attribute (new or existing) (```Usage: update <class name> <id> <attribute name> "<attribute value>```).
| ```<class>.all()```  | Same as all ```<class>```
| ```<class>.count()```  | Retrieves the number of objects of a certain class (```Usage: <class name>.count(), Example: User.count()```).
| ```<class>.show(<ID>)```  | Same as show ```<class> <ID>```
| ```<class>.destroy(<ID>)```  | Same as destroy ```<class> <ID>```
| ```<class>.update(<ID>, <attribute name>, <attribute value>```  | Same as update ```<class> <ID> <attribute name> <attribute value>```
| ```<class>.update(<ID>, <dictionary representation>)```  | Updates an objects based on a dictionary representation of attribute names and values


## Authors

- Festo - Initial console implementation
- Festo - FileStorage and additional console commands

AUTHOR:
Festo Wampamba
