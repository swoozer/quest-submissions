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
