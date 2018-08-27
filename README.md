# solidity-porject

# Project description

Enrollment system for online courses, where you can see the course offer and apply for a course and pay with Ethers. Also the system can emit certifications when the course conditions are accomplished.

The course creation and certification issuer is a specific address in the Ethereum blockchain. The users can apply in the system by them self and pay the fee for the course enrollment with a Ethereum account. 

This project can be usefull for an online course system mangamentm like coursera, udemy and others.


## User histories:

UserHistory1:
As a System administrator can create courses specifying parameters like:
- Course_name
- Course_id
- Total_hours 
- Teacher (Etehereum Address)
- Price
- Start_date
- End_date
The system verify de address with the admin address for validate the course creation.


UserHistory2:
As a user can look the course lisk and select the course and enroll to the course, acepting the conditions and registering the follow information:
- FisrtName
- Lastname
- email
- Phonenumber
The user can pay with ether the enrollment process to the course and can receive a mail with the confirmation.

The first project version include

Create courses and enrrol students using Ethereum smartcontracts and web3.js in a http aplication server.
