# AddressBook
Description :-
    In this project, each person's contact information including name, phone number, and email address will 
be saved in an organized structural array.

    To select the sort of activity we need to perform, we will declare distinct methods in this example for 
creating,listing, searching, editing, and deleting contacts. These functions will be called inside a switch case. 

REQUIREMENTS :
                1. FILE POINTERS
                2. ARRAYS
                3. STRUCTURES
                4. STRINGS
                5 PREDEFINED functions
                

# Load contact from file: -
    In this function we are calling the file pointer to get data from the txt file, in which contact is saved already.
In the txt file we are giving a delim as comma(,),to segregate name, phone number and email to save in structure array.

For example the file containing the contact details as 
Isabella White 			,5552461357  			  ,isabella.white@example.com	

to separate the name we use strtok function and store in in the name array.

# Create Contact :-
      In creating contact first thing is to check if the conatact is present or not.if the contact is present 
it have to print "ERROR : NAME OR PHONE OR EMAIL ID ALREADY EXISTS".

For Example in create contact I am giving name as John Doe by using STRNCMP FUNCTION it will check the whole array
if the name is present or not ,if same name found it will print "Name already exists".

Input   : John Doe
output : Name already exists

# Search Contact :-
    In search we trying to get the details of the particular person like name,phone number ,email.

For Example I am trying to search Alice Johnson
 
at the time of getting the output it print entire person details like

Output : Name: Alice Johnson  Phone Number: 6321234567  Email: alice.johnson@example.com

# List Contacts: -

This function lists all the contacts stored in the system. If no contacts are present, 
it informs the user that the contact list is empty.

Output Example:

Contact 1: Name: John Doe, Phone: 1234567890, Email: john.doe@example.com
Contact 2: Name: Alice Johnson, Phone: 6321234567, Email: alice.johnson@example.com

If the contact if not fount it have to print : No contacts available.


# Edit Contact :-

This function allows the user to modify the phone number and email of an existing contact. 
The system searches for the contact by name, and if found, prompts the user to input new phone and email details. 
If the contact is not found, the system prints an appropriate message.
Input: Name of the contact to edit, followed by new phone number and email address.

Output Example:
Input:
Name: John Doe
New Phone: 9876543210
New Email: john.new@example.com

Output:
Contact updated successfully.

If the contact is not found it have to print : -
Contact not found.


# Delete Contact :-

This function deletes a contact from the system. 
The user specifies the contact’s name, and the system removes it if found. 
The system then shifts the remaining contacts to maintain a continuous list.

Input: Name of the contact to delete.
Output Example:
Input:
John Doe
Output:
Contact deleted successfully.

If the contact is not found it have to print :-
Contact not found.

# Save contacts to the file :-

    After completing this all operations we need to store the modified contacts in a txt file.

