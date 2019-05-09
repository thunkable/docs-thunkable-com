---
description: >-
  Use the Blockchain Wallet to add information about your account to the
  application including identity and wallet amount
---

# Blockchain Wallet by Oasis

{% hint style="info" %}
From sharing medical records, to analyzing personal financial information, to training machine learning models, the Oasis platform supports applications that use even the most sensitive data without compromising privacy or performance
{% endhint %}

## **Get Account Address**

![](.gitbook/assets/image%20%2826%29.png)

**Output:**

* Address \(type: text\): Each time an app with the Blockchain Wallet component is installed, the app gets a new blockchain account. Each blockchain account on Oasis has an address that identifies it, and is of the form “0xc38f0DFC19816706eF10bC9E362cF5C1138Bd6d3”

## Get Balance

![](.gitbook/assets/image%20%2848%29.png)

**Input:**

* Address \(type: text\): The address of the blockchain account whose balance you want to know.

**Output**

* Balance \(type: text\): The balance of the blockchain account whose address was provided. You can find out the account balance of any blockchain account on the Oasis blockchain using this block. The unit of this balance is just called “Gas” for now. While the balance is a number, because the balances can be really small or really big, we return it to you as a String \(Text\).
* Error \(type: Object\): Is not undefined if there was an error while trying to retrieve the balance of the account.

## **Get Transaction**

![](.gitbook/assets/image%20%2819%29.png)

Every time you write to the blockchain, a transaction is generated. This could be sending Gas from one account to another or running a smart contract method that writes new data to the blockchain.

**Input:**

* TransactionHash \(type: Text\): The way you identify transactions is through a unique “hash.” Each hash maps to exactly one transaction. When you send a transaction to the blockchain, the blockchain will return to you a transaction hash with which you can get more information about the transaction.

**Output:**

* Error \(type: object\): Is not undefined if there was an error while trying to retrieve the transaction object.
* TransactionObject \(type: Object\): This object contains information about the transaction, such as who was Gas sent to and who was it sent from, or how much did it cost to send. Here is an example transaction object:
  * **`{     "hash": "0x9fc76417374aa880d4449a1f7f31ec597f00b1f6f3dd2d66f4c9c6c445836d8b",     "nonce": 2,     "blockHash": "0xef95f2f1ed3ca60b048b4bf67cde2195961e0bba6f70bcbea9a2c4e133e34b46",     "blockNumber": 3,     "transactionIndex": 0,     "from": "0xa94f5374fce5edbc8e2a8697c15331677e6ebf0b",     "to": "0x6295ee1b4f6dd65047762f924ecd367c17eabf8f",     "value": '123450000000000000',     "gas": 314159,     "gasPrice": '2000000000000',     "input": "0x57cb2fc4" }`**

## **Get Transaction Receipt**

![](.gitbook/assets/image%20%2821%29.png)

Similar to the GetTransaction block, this block also retrieves information about the transaction. The main difference is that the receipt is only available once the transaction is fully a part of the blockchain and it tells you exactly what happened when you wrote something to the blockchain. GetTransaction will get you information about what is supposed to happen after you’ve submitted the transaction, but the blockchain is still working on writing it down.

**Input:**

* TransactionHash \(type: Text\): The way you identify transactions is through a unique “hash.” Each hash maps to exactly one transaction. When you send a transaction to the blockchain, the blockchain will return to you a transaction hash with which you can get more information about the transaction.

**Output:**

Receipt and Error. Here’s an example of the Receipt:

**`{  
  "status": true,  
  "transactionHash": "0x9fc76417374aa880d4449a1f7f31ec597f00b1f6f3dd2d66f4c9c6c445836d8b",  
  "transactionIndex": 0,  
  "blockHash": "0xef95f2f1ed3ca60b048b4bf67cde2195961e0bba6f70bcbea9a2c4e133e34b46",  
  "blockNumber": 3,  
  "contractAddress": "0x11f4d0A3c12e86B4b5F39B213F7E19D048276DAe",  
  "cumulativeGasUsed": 314159,  
  "gasUsed": 30234,  
  "logs": [{  
         // logs as returned by getPastLogs, etc.  
     }, ...]  
}`**

You can see that it includes things like status, gasUsed, and logs that you can only get once the transaction has been processed and you can see what happened.

## **Send Transaction**

![](.gitbook/assets/image%20%283%29.png)

Sends Gas from the user’s account to another account. This waits for the transaction to become a part of the blockchain and for the receipt to be ready before calling the next callback block.

**Inputs:**

* To address \(type: text\): the address to which you want to send Gas
* Value \(type: text\): the amount of gas you want to send.
* Gas \(type: number, optional\): The amount of gas to use for the transaction \(unused gas is refunded\).
* Gas Price \(type: text, optional\): The price of gas for this transaction in wei

**Outputs:**

* transactionHash: the hash of this transaction that was sent
* Receipt: The receipt of the completed transaction showing what happened when the transaction was written to the blockchain
* Error: If there was an error when trying to send the transaction. Can happen if you’re sending more Gas than you have in your account or you don’t have enough Gas to pay for the transaction to happen.

## **Send Transaction Without Receipt**

![](.gitbook/assets/image%20%284%29.png)

This sends the transaction and returns the TransactionHash immediately and does not wait for the blockchain to finish writing the transaction. This block is helpful if you want to just send the transaction and want to do other things while waiting for the transaction to be written to the blockchain.

**Inputs:**

* To address \(type: text\): the address to which you want to send Gas
* Value \(type: text\): the amount of gas you want to send.
* Gas \(type: number, optional\): The amount of gas to use for the transaction \(unused gas is refunded\).
* Gas Price \(type: text, optional\): The price of gas for this transaction in wei

**Outputs:**

* transactionHash: the hash of this transaction that was sent
* Receipt: The receipt of the completed transaction showing what happened when the transaction was written to the blockchain
* Error: If there was an error when trying to send the transaction. Can happen if you’re sending more Gas than you have in your account or you don’t have enough Gas to pay for the transaction to happen.

## **Send Transaction Run Only**

![](.gitbook/assets/image%20%2820%29.png)

This is useful when you want do a practice run of sending a transaction. Sometimes you want to make sure the transaction will go through with the gas price and gas that you’ve specified etc. This block won’t actually write the transaction onto the blockchain and so using this block won’t cost you any Gas.

**Inputs:**

* To address \(type: text\): the address to which you want to send Gas
* Value \(type: text\): the amount of gas you want to send.
* Gas \(type: number, optional\): The amount of gas to use for the transaction \(unused gas is refunded\).
* Gas Price \(type: text, optional\): The price of gas for this transaction in wei

**Outputs:**

* transactionHash: the hash of this transaction that was sent
* Receipt: The receipt of the completed transaction showing what happened when the transaction was written to the blockchain
* Error: If there was an error when trying to send the transaction. Can happen if you’re sending more Gas than you have in your account or you don’t have enough Gas to pay for the transaction to happen.



## **Subscribe To Logs**

![](.gitbook/assets/image%20%2837%29.png)

You can use this block to subscribe to specific events on the blockchain**.**

**Input:**

* From block \(optional\): The number of the earliest block to start listening from
* Address \(Text or List\): An address or a list of addresses to only get logs from particular account\(s\).
* Topics \(List\): An array of values which must each appear in the log entries. The order is important, if you want to leave topics out use null, e.g. \[null, '0x00...'\]. You can also pass another array for each topic with options for that topic e.g. \[null, \['option1', 'option2'\]\]

**Output:**

* Callback is called whenever a new event occurs. The following parameters are passed into the callback:
  * logEntry \(object\): Is not undefined every time a new event that matches the topics, addresses, etc. happens.
  * changedLog \(object\): Is there every time a log is removed from the blockchain.
  * Error \(object\): Is there when an error occurs with the subscription.

\(Please note: Oasis Labs is a beta product. As a result there may be system updates that impact your app's ability to connect to the platform or even loose data during major quarterly upgrades. You can learn more [_here_](http://docs.oasiscloud.io/en/latest/dashboard-quickstart/) about upgrade cycles\)

\*\*\*\*

\*\*\*\*

\*\*\*\*

\*\*\*\*

\*\*\*\*

\*\*\*\*

\*\*\*\*

\*\*\*\*

