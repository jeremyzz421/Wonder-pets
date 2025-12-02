_**SortiTech:Smart Waste Sorting and Collection System**_

**DESCRRIPTION/OVERVIEW**

This Java console based application should enable users to be more mindful about the surroundings by demonstrating the functionality of a simple waste management system. The program enables the user to classify waste with three categories; biodegradable, non-biodegradable, and recyclable. This will educate people on proper separation of wastes and the users are taught how each type of waste is to be disposed.

The system also has the capability of handling the collection schedules and one can set or change the time in which the waste is supposed to be collected in their household or community. It gives users an option of the day or hour of preferred collection and updates it whenever it is necessary. The application maintains a definite record of the cumulative amount of waste to each category and it updates this record whenever the new waste is added. It also consolidates the waste it has accumulated such that users can easily check the amount of waste they have accumulated over the years.

Besides, the program comes with a simple and easy to use menu allowing users to navigate through the menu with ease. It takes the user through the steps and thus the system is easy even to the ones who are still learning about waste management. To encourage proper management of waste, the application will also verify whether a waste category is approaching capacity limit. When a bin is nearly full or full, the system will issue a warning message to inform a user to do something, as either to schedule a collection or minimize further production in the form of waste. This will stop overflow and promote good environmental practices.

**OOP Concepts applied**

`Abstraction` The WasteRecord group conceals hard things. It hides facts of waste types out of view. You are looking at easy stuff, not difficult stuff.It just gives the bare minimum of any record, i.e.: it gives the date and the amount subtracted over, plus the abstract displayRecord() method. All the individual types of waste are then able to determine how to present their respective information without the program having to be aware of the details.

`Inheritance` WasteRecord is the predecessor of PlasticRecord.  WasteRecord provides it with all of its fields.  It has date & amountReduced.  It gets any base methods too.  PlasticRecord possesses everything that base class provides...It avoids the repetition of code and simplifies the task of creating new waste-record types in the future.

`Polymorphism` The displayRecord() method is defined in the abstract class, but implemented in different ways in each of the subclasses. It is a form of runtime polymorphism: the program can work with different record types using the WasteRecord reference, but on executing the displayRecord() method, it executes the one that is specific to a subclass (such as PlasticRecord).

`Encapsulation` Both the date and the amountReduced are not directly exposed but through getters and setters. This safeguards the inner values of the object and makes sure that they can be altered only in a regulated, foreseeable manner.

### Program Structure

Main Class: SortiTechSystem
This is the main controller of the entire application. It does the following functions:

• shows program introduction and help section.

• Introduction of user menu to navigate.

• Manages the addition, deletion, searching, sorting and displaying of waste records.
Stores store all the plastic wastes in an array of PlasticRecord[].

•	Processes user input and verifies it.

The program flow is done using different menus.

The upper limit is also established to 100 records in the class and records the number of records saved.



Abstract Class: WasteRecord
This is the type of category that this class provides the model of any kind of waste records.
It contains:

•	The date of the record

• The amount of waste reduced

•	Something to set values.

• Manipulators and lockers to regulate data entry.

•	A displayRecord() method that would be subclassed and would implement formatting.

This makes them consistent throughout all the records of waste data regardless of the type of waste being used.


Subclass: PlasticRecord
Boasts of a particular form of waste-plastic waste.

It will expand WasteRecord and will offer the practical implementation of the displayRecord() procedure.

It enables the program to store a lot of information, including the number of plastic that has been reduced on any specific date.
The system can be repeated to accommodate biodegradable and recyclable waste when the system is extended.

Data Handling and Storage

The data about the waste is held in an array of the fixed-size objects of PlasticRecord.

RecordCount is a variable that is used in keeping a count of the number of entries.

Only, there are possibilities to add records, to search them by date, delete them, sort them, and make them listed.

Sorting One simple bubble sort algorithm sorts by descending plastic reduction amount.
This system enables this structure to have a clean and organized history of waste reduction.

Menu Navigation Flow
The show takes the user through various strata of menus:
1.	Introduction Screen
Shows the title and the description of the display and developer credits.
2.	Main Menu

•	Begin

•	Help

•	Exit

3.	Tracker Menu
House the house of all important system functions, viz.,
•	Add Record

•	Record Delete Search Record

•Records sorting

•	Display All Records 

•	Back to Main Menu 
This design makes this system very simple to use and run even by users who are not very experienced.

### How to Run the Program
1. Accessing the Main Menu
Once the program is launched, the initial screen you will be greeted with is the Main Menu which will serve as the primary navigation control in the entire system. It consists of three options:
Start
Help
Exit
This is what each option is supposed to be:
Start – Heading in this option, you will be directly taken to the SortiTech Tracker Menu. It is in this place that you can add new data, search saved entries, sort your information or show all your records you have in store.
Help – This is useful to those who are new. It provides a brief description of what the program can do, what it provides and how each aspect of the system functions.
Exit - This would entirely kill the program. This is what you have to choose in case you are over with the system.
The Main Menu acts as a reference point to what you are going to do next, therefore, the appropriate choice made here would dictate what aspect of the system you are going to enter into.
2. SortiTech Tracker Menu entrance.
On selecting the start option under the main menu it will take you to the sortiTech Tracker Menu which is the primary working area of the program.
The following are the features incorporated in this section of the system on managing your plastic waste reduction records. The choices can be the following:
Add Record
Delete Record
Search Record
Sort Records
Display All Records
Back to Main Menu
All these options are some of the key functions that can be offered by the SortiTech System.
3. Adding a New Record
Assuming that you clicked on Add Record, the program requests you to enter two items of information:
The date of waste reduction
Weight of plastic decreased (grams)
After entering this information, the system saves the record and puts it in its list of records stored.
Here is the feature that is used when you want to track your progress or document a new day of plastic waste reduction.
4. Deleting an Existing Record
In the event that you select the Delete Record, the program would prompt you to provide a particular date.
It will then go through the list of records present, to locate a record with the identical date. When a match is discovered in the program, the whole record is deleted.
This option is helpful when:
And you have filled in the wrong details.
You would like to clean up or update data that you have in storage.
You must do away with outdated entries.
5. Finding a Particular Record
Search Record option You can use the Search Record feature to find a particular entry by typing in the date you are interested in.
The system will scan all the already saved records against a date similar to the one you have entered.
In case there is a record on that date, the program will display:
The date of the entry
The amount of plastic decreased on this day.
This is handy when you have to refer to an earlier entry but you do not have to scroll through the entire list.
6. Sorting All Saved Records
The selection of Sort Records will reorganize all the records stored so as to come in order.The sorting organization typically contains the most amount of plastic that has been reduced at the top, down to the bottom. This option is useful when:
You would like to know which day had the most reduction.
You would like to look at your performance patterns.
This list is required to be organized to report.
Sorting will allow data to be more readable and understandable.

7. Viewing the Saved Records.
Choosing Display All Records will result in the list of all plastic reduction entries that are already in the system. Each record will contain:
The date it was recorded
The amount of grams decreased in that date.
It is a perfect choice in case you need to have a general overview of all of your inputs or you need to check whether your information has been stored properly.
8. Returning to the Main Menu
To get out of the tracker and back to the primary navigation screen, you will only have to use Back to Main Menu.
This will get you out of the SortiTech Tracker Menu and back to the first page where you have the options to Start, Help and Exit.
This is useful when:
You are interested in making changes to the program.
You want to go back to Help
You are done with entering data and want to exit the system in a decent way.
9. A Graceful Farewell to the Program.
To completely close the SortiTech System, go back to the Main Menu and choose Exit. This will not allow the program to execute and close the console window at once.
It will have Exits on the Main Menu that will make sure that:
The program gets a safe termination. There are no unfinished functions. You move on to your desktop or command prompt without failures.

### Sample output














