import os  # Importing the os module to interact with the operating system
import time  # Importing the time module to add delays

toDoList = []  # Initialising an empty list to store to-do items

def printList():
    """Function to print the current to-do list"""
    print()  # Print a blank line for better readability
    for items in toDoList:  # Iterate through each item in the to-do list
        print(items)  # Print each item
    print()  # Print another blank line for better readability

while True:  # Infinite loop to keep the programme running

    menu = input("ToDo List Manager\nDo you want to view, add, edit, remove or delete the to-do list?\n")  # Display menu and get user input
    if menu == "view":  # If user chooses to view the list
        printList()  # Call the function to print the list


    elif menu == "add":  # If user chooses to add an item
        item = input("What do you want to add?\n").title()  # Get the item to add and capitalise it
        toDoList.append(item)  # Add the item to the to-do list


    elif menu == "remove":  # If user chooses to remove an item
        item = input("What do you want to remove?\n").title()  # Get the item to remove and capitalise it
        check = input("Are you sure you want to remove this?\n")  # Confirm the removal
        if check[0].lower() == "y":  # If the user confirms (case insensitive)
            if item in toDoList:  # Check if the item is in the list
                toDoList.remove(item)  # Remove the item from the list

    elif menu == "edit":  # If user chooses to edit an item
        item = input("What do you want to edit?\n").title()  # Get the item to edit and capitalise it
        new = input("What do you want to change it to?\n").title()  # Get the new value and capitalise it
        for i in range(len(toDoList)):  # Iterate through the list
            if toDoList[i] == item:  # If the item is found
                toDoList[i] = new  # Update the item with the new value
                break  # Exit the loop once the item is found and updated
        else:
            print("The item was not found")  # Print a message if the item was not found

    elif menu == "delete":  # If user chooses to delete the entire list
        toDoList = []  # Clear the to-do list
    time.sleep(1)  # Wait for 1 second before clearing the screen
    os.system('clear')  # Clear the screen 
