# CISC 327

Project Requirements
The product you are to design and build is the Simple Interactive Banking System
(“SimBank”). SimBank consists of two parts:
 - the Front End, a ATM banking transaction acceptor for simple ATM-style
banking transactions
 - the Back Office, an overnight batch processor to maintain and update a
master accounts file
Both parts will be run as console applications, that is, they are to be invoked from a
command line and use text and text file input/output only (this is important for
assignments later in the project, so don’t ask for exceptions). We avoid user interfaces
in this course so that we can concentrate on software quality control practices without
the distractions of graphics, look and feel.

The Front End
The Front End reads in a list of valid account numbers (1), processes a stream of
transactions one at a time (2), and writes out a summary file of transactions at the end
of the day (3)

Informal Customer Requirements for the Front End
The Front End handles a sequence of transactions, each of which begins with a single
transaction code (word of text) on a separate line
The Front End must handle the following transaction codes:
login - start a Front End session (processing day)
logout - end a Front End session
create - create a new account (privileged transaction)
delete - delete an existing account (privileged transaction)
deposit - deposit to an account (ATM transaction)
withdraw - withdraw from an account (ATM transaction)
transfer - transfer between accounts (ATM transaction)
