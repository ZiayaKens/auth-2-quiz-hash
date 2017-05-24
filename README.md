# Storing Passwords Quiz
## Would you like salt with your hash?


With your partner, in words both of you will understand 6 months from now, answer the following questions.

> A customer hires you to consult on a web app.  You notice that they are storing their passwords in plaintext.  What advice would you give the customer.  This advice should outline the risks of the current solution, and give a list of best practices for a new solution.

storing passwords in plain text makes it easier for hackers to gain access to accounts. Its like a one step process, where when they aquire the passwords, they have to do no additional work to use them. A suggesting would be to use a hashing algorythm to allow for safer password storing because you aren't not storing the exact password. An additional tip would be to "salt" the password before hashing it. salting the password eliminates the possibiliy of a password existing in the dictionary ( when passwords are a word in the database/dictionary, hackers often have a quicker time discovering the password) salting adds a string to the password(same string every time) and the hashing algorythm converts the password to a random string of a set length.

> You are tasked for creating a RFP (request for proposal) for a new cryptographic hashing algorithm.  What requirements would you put in place for this new algorithm.

the hash should always be the same length of characters. The hash should changed drastically when there is only a small change in the password. No two passwords should create the same hash. The hashing algorythm should be one way. The hashing algorythm should take a long time to complete(ex. 1 hash every 30 seconds)
