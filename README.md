0x8256dc13c4426072

<b> Chapter 1 Day 1 Quest </b>
- A blockchain is an open, decentralized database where anyone can view, store, and interact with data using SmartContracts. There are many different blockchains, including FLOW and Ethereum.
- A SmartContract consists of coding that enables a user to make transactions on the blockchain. It also sets the "rulebook" of how the data on the blockchain can and cannot be manipulated.
- Scripts allow you to view data on the blockchain. They do not cost money. Transactions allows you to change data on the blockchain and costs money ie. "gas."

<b> Chapter 1 Day 2 Quest </b>
- Cadence Programming Language Pillars
 1. Safety and Security --> Keep users' $$ and assets protected!
 2. Clarity --> Prevents miscommunication!
 3. Approachability --> Easy-to-read for all developers!
 4. Developer Experience --> User-friendly!
 5. Resource Oriented Programming

<b> Chapter 2 Day 1 Quest </b>

![image](https://user-images.githubusercontent.com/104751516/167507952-e67f0586-3b8d-4408-b388-aafd85f28830.png)

pub contract JacobTucker {
  pub let is: String
  init () {
    self.is = "the best"
  }
}

![image](https://user-images.githubusercontent.com/104751516/167507899-73cb7aaa-f7e2-42ce-905d-42f8b3d461bb.png)

import JacobTucker from 0x03

pub fun main(): String {
  return JacobTucker.is
}

![image](https://user-images.githubusercontent.com/104751516/167507739-6fec588c-f323-429f-a39d-c35ae1abd31c.png)


<b> Chapter 2 Day 2 Quest </b>
1. We wouldn't call changeGreeting in a script because scripts are only used to view the contract and cannot make changes to or modify the contract.
2. AuthAccount allows the contract to access or "look inside" an account. This occurs after the account owner deploys or signs the transaction.
3. The prepare phase simply accesses data in an account. The execute phase calls functions and changes the data on the blockchain.


![image](https://user-images.githubusercontent.com/104751516/170792606-cbdd3df3-14dc-4ec3-b562-e42460f8d53c.png)

<br></br>

import HelloWorld from 0x01

pub fun main(): Int {
  return HelloWorld.myNumber
}

![image](https://user-images.githubusercontent.com/104751516/170792797-90856cd0-66b1-4933-9641-cd3e5909dc15.png)

![image](https://user-images.githubusercontent.com/104751516/170792859-bda1655c-c0d5-4027-89c2-13a859a1920c.png)

<br></br>

import HelloWorld from 0x01

transaction(myNewNumber: Int) {
  prepare(signer: AuthAccount) {}

  execute {
    HelloWorld.updateMyNumber(newNumber: myNewNumber)
  }
}

![image](https://user-images.githubusercontent.com/104751516/170794031-774ddbec-b4f4-461a-8311-cdc439df96dc.png)

![image](https://user-images.githubusercontent.com/104751516/170794060-196a9b88-a66d-44a2-8414-2318a3332715.png)

<br></br>
<b> Chapter 2 Day 3 Quest </b>

1.
![image](https://user-images.githubusercontent.com/104751516/170807913-9917d91e-9219-4d06-b251-51666460e2f5.png)

![image](https://user-images.githubusercontent.com/104751516/170808127-ece01a57-2e92-4830-a108-48398e7e2e6f.png)

2.
![image](https://user-images.githubusercontent.com/104751516/170811676-28572258-dea4-4120-9c55-4eaf177a3ca2.png)

![image](https://user-images.githubusercontent.com/104751516/170811700-499c7f0a-2c4b-41ed-b8b3-3d8ec2014717.png)

<br></br>

3. The force unwrap operator ! allows the function to return an optional, where if the type is defined then the optional type is removed and if the type is nil then the entire program aborts. For example, setting Int? = 0 returns 0, but setting Int? = nil returns ERROR.

![image](https://user-images.githubusercontent.com/104751516/170812058-1c47a79d-ef30-48db-bc6c-dcc63eda7dcf.png)
![image](https://user-images.githubusercontent.com/104751516/170812080-a8accab1-46c4-47ba-9ea9-ff282ba56a20.png)

<br></br>

![image](https://user-images.githubusercontent.com/104751516/170812119-80915162-b82d-4548-b9a8-b3d1ab053548.png)
![image](https://user-images.githubusercontent.com/104751516/170812140-dc2d192a-1f00-4c8e-a691-43fb816d6f7f.png)

<br></br>

4. The error message ("mismatched types. expected String, got String?") means that the function returned an optional value - String or nil - when it was expecting only String values. We are getting this message because accessing elements of a dictionary returns optionals. In order to fix it, we will need to add the force unwrap operator (!) into the return command as shown below.

![image](https://user-images.githubusercontent.com/104751516/170812402-d2b8d0a8-3186-4c15-a348-d434141be6c9.png)

![image](https://user-images.githubusercontent.com/104751516/170812413-ac7f23dd-e1ff-44f3-abca-fa9020b8c958.png)

<br></br>
<b> Chapter 2 Day 4 Quest </b>

