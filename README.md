You have just been hired by a tech startup that is planning on releasing a new e-mail service to its clients. They have asked you to create a prototype of this service using your Python skills. The final version of this prototype should do the following:
  - Allow the user to register for a new account. When they register, they will supply a username and password, which will need to be validated. The username will also need to be unique (i.e. only one person can have a given username). If the user registers successfully their information will need to be stored in a permeant storage mechanism (in this case, a file)
  - The user should also be able to log into their account. This part of the system will ask the user for a username and password and match it up against the one the company has on file for them. Note that the company plans on having millions of clients, so this information must be cross-referenced against a file and cannot be 'hard-coded'.
  - The user should be able to send messages to any other user on the system. To send a message the system will ask the user for the name of a recipient and a message to send (one line of text). If the recipient is registered the message will be delivered through a file.
  - The user should be able to read messages that have been sent to them (and only them)
  - The user should be able to delete all of the messages that have been sent to them (and only them)

In order to do this the software engineers at the company have outlined a series of functions that will need to be built to create the prototype. Your job is to build these functions and test them as you go - don't skip ahead! When all of the necessary functions are built you will use them to construct the prototype e-mail system

After creating your functions, Here's what your program should do:
  - Present the user with a menu of choices - login, register or quit
  - If they choose to quit you should immeidately end the program.
  - If they choose to register you should prompt them for a username and a password. Ensure that the username and password are valid using your functions. Then ensure that the username has not already been taken. If all of these items are OK you can go ahead and register the user for an account and return them back to the main menu.
  - If they choose to login you should prompt them for a username and a password. If the username and password is correct they should be logged in. They then should receive a new menu of options (hint - user a nested 'while' loop for this):
      - Present the user with the options to read messages, send messages, delete messages or logout
      - If they choose to logout they should return to the main menu
      - If they choose to read messages you should display their messages
      - If they choose to delete messages you should delete all their messages
      - If they choose to send a message you should prompt them for a recipient username and a message. If the recipient is unknown you should reject the message. If they are known,            you should send a message to that user using your function.
