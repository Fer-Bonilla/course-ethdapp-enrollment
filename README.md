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


## Installing instructions


Be sure that nvm, node and npm ares installed

For this project this package are required


NPM
Truffle Framework
NodeJS
Ganache-CLI
Metamask
VueJs


```bash
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
exec $SHELL (Or close and open again the terminal)
command -v nvm
nvm install node
exec $SHELL
command -v npm
npm i -g truffle ganache-cli
```
 Create the project folder.
 ```bash
mkdir ~/blockchain/certifier
cd ~/blockchain/certifier
truffle init
```

Injecting the front end framework to the project

First, we must install the VueJS command line utility as global dependency.

```bash
npm i -g @vue/cli
```

Then we go a level above to install the frontend.

```bash
cd ..
vue create certifier
```

Then we must answer a couple of questions the cli prompts

1. Target directory? → Merge
2. Picking presets → Manually
3. You must use whatever you want, but the recommendation is → Babel, Router, Vuex, CSS Preprocessors
4. Use of history mode → Yes
5. CSS - Pre-processors → SASS/SCSS
6. Prefered places for presets → Dedicated config files
7. Saving presets → As you wish

Then, back inside the project we must install once again `chai`.

```bash
npm i -D chai
```

 To establish the connection to the local blockchain we ran the following command.
 ```bash
ganache-cli
``` 
 And then we modified the file, in order to let truffle how to got a connection to the local blockchain:
 ```bash
truffle.js
```

Then copy all the files from the github repository to the certifier folder
 ```bash
/blockchain/certifier
```

Compile and migrate de contracts
 ```bash
truffle compile
Truffle migrate
```

And then run de dapp
 ```bash
need go to the certifier folder 

npm run serve

```

Then go to http://localhost:8080 for interact with the app
