# Software Requirements Specification 
# Purpose
The purpose of this source is to describe the railway reservation system which provides the train timing details, reservation, billing and cancellation on various types of reservation. The system reduces the intervention of the user with the ticket counter and cuts the time of  waiting in the queue.

# Scope
The scope of this system in creating Reservation is that, from any Railway Station we can Create Reservation, which is updated automatically in all the stations. Hence, there is no confusion to the Reservation Clerk in all the stations to create the Reservation. This can be possible by maintaining Global Database. Clerks present at different stations can access the global database and the clerks can easily understand the remaining reservation seats. It provides the ability to create reservations from different places for a train.

# Requirements
##	Functional Requirements
- The system is such that it stands up to user expectations.
- The response time of the operation is good. Response to user error and undesired situations has been taken care of.
- The system should safeguard itself against undesired events without human intervention.
- The software should not be architecture specific and should be transferable to other platforms if needed.

## Non-functional Requirements
- The system should provide a layer of security above all the data transfer and all the transactions happening.
- The system should provide reliability of all the separate components, mainly of the database which is updated spontaneously.
- The system should be up and running at the time so that a user should be able to access anytime he/she wants.
- As the database is continuously updated and the changes are getting reflected, it should be well maintained.
- The code and modules should be properly documented and easy for the user to understand.
## User Requirements
- Login/Sign up
- Options to reserve or cancel a ticket.
- Proper user-friendly interface.
- A screen which records all the user transactions.
- Secure payment methods.
