### Purpose
Send and receive money!

### Method

At this point, doing:

```
eth.getBalance(eth.accounts[0])
```
should show one Ether, i.e. 1000000000000000000 Wei

Now look at the spreadsheet https://docs.google.com/spreadsheets/d/1fW_NYpddcuL1QKFtrIyYDkHIYHIFjabMfMfGzG7co0o/edit?usp=sharing

Find the person above you and make a note of their address.
Send them 0.1 Ether!

    eth.sendTransaction({from:eth.accounts[0], to:"<the recipient>", value:100000000000000000});

You will end up with a transaction ID, e.g. 0xb983404b383361f27c1016eb7adcd422b0540d8fabf73fec0d5e9181a4fbaa49
Put that into etherscan to check it has been "mined"

https://testnet.etherscan.io/tx/0xd7041f44b65a1b8a98c5a3111106211420a78bafe449dae7f718a2a8c911a706

YOu will probably see a "Pending" state.
Eventually it will show with a "Block" number, which means it has been added to a block in the blockchain. It is now "mined"!

Once it is mined, check your balance

    eth.getBalance(eth.accounts[0])

You should see it go down by approx 0.1 Ether. Eventually you will receive 0.1 Ether. So when all is done you are back where you started, i.e. with 1 Ether. Or are you?

Your address ("wallet") is becoming like a bank statement or a ledger.It has all the inputs and outputs:

https://testnet.etherscan.io/address/0xec1a21b4079ac5ede878c829ea0174b12e74166b
    
## Learning Points

Your address is like a wallet, which holds value.

It is also like a bank account, which keeps track of activity (money in and out) in a ledger

Your address and the transactions are public. Anyone can see what it has been doing

Transactions cost money: You are paying the "miners" to do the work of adding your transaction to the blockchain. 



