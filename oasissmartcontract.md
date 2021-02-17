---
description: Use this component to call your own smart contract on Oasis
---

# Smart Contract by Oasis

{% hint style="info" %}
From sharing medical records, to analyzing personal financial information, to training machine learning models, the Oasis platform supports applications that use even the most sensitive data without compromising privacy or performance
{% endhint %}

## Add a Smart Contract component to Thunkable

To add a Smart Contract component to your app:

* Go to your Blocks tab
* Find the `Advanced` drawer of blocks. Click the drop-down menu icon to show the Advanced invisible components
* Click the ⊕ icon next to the `Smart Contracts` drawer

![](.gitbook/assets/advanced-components%20%281%29.png)

You will see a dialog with options to enter certain properties for your Smart Contract component. Click Submit to create the Smart Contract component, or Delete to dismiss the dialog without creating the component.

![](.gitbook/assets/add-smart-contract.png)

### Editing your Smart Contract's properties

Once you have added at least one Smart Contract component to your app, you will be able to view all of your Assistant components under the `Smart Contracts` drawer on the Advanced section of the Blocks tab. 

To edit the properties of a Smart Contract component, click on the ⚙ icon next to the component's name to bring up the properties dialog. You will be able to change the properties and click Submit to save your changes, or click Delete to delete the component.

![](.gitbook/assets/smart-contracts-blocks.png)

## **Method Block**

![](.gitbook/assets/image%20%2873%29.png)

Use this block to call any method of a smart contract that has been deployed to the blockchain.

**Input:**

* Method name \(text\): The name of the method
* Parameters \(type: list\): A list of the parameters that need to be passed into the method
* Value \(Text, optional\): The amount of Gas you want to send to the Smart Contract when you’re calling the method
* Gas \(Number, optional\): \(same as SendTransaction\) The amount of Gas that will be used to write this transaction onto the blockchain. Unused gas will be returned.
* Gas Price \(Text, optional\): The price of gas for this transaction in wei

**Output:**

* transactionHash: The hash of this transaction that was sent
* Events: The events that were emitted while running this blockchain method.
* Error: If there was an error when trying to run the method. Can happen if you’re sending more Gas than you have in your account or you don’t have enough Gas to pay for the method to run and write to the blockchain
* Receipt: The receipt of the completed transaction showing what happened when the transaction was written to the blockchain. This includes any events that were emitted while running the method.

**Example:**

**`{  
        "transactionHash": "0x9fc76417374aa880d4449a1f7f31ec597f00b1f6f3dd2d66f4c9c6c445836d8b",  
        "transactionIndex": 0,  
        "blockHash": "0xef95f2f1ed3ca60b048b4bf67cde2195961e0bba6f70bcbea9a2c4e133e34b46",  
        "blockNumber": 3,  
        "contractAddress": "0x11f4d0A3c12e86B4b5F39B213F7E19D048276DAe",  
        "cumulativeGasUsed": 314159,  
        "gasUsed": 30234,  
        "events": {  
            "MyEvent": {  
                returnValues: {  
                    myIndexedParam: 20,  
                    myOtherIndexedParam: '0x123456789...',  
                    myNonIndexParam: 'My String'  
                },  
                raw: {  
                    data: '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385',  
                    topics: ['0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7', '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385']  
                },  
                event: 'MyEvent',  
                signature: '0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7',  
                logIndex: 0,  
                transactionIndex: 0,  
                transactionHash: '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385',  
                blockHash: '0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7',  
                blockNumber: 1234,  
                address: '0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe'  
            },  
            "MyOtherEvent": {  
                ...  
            },  
            "MyMultipleEvent":[{...}, {...}] // If there are multiple of the same event, they will be in an array  
        }  
    }`**

## **Method Run Only**

![](.gitbook/assets/image%20%2834%29.png)

Use this block to just run a method without writing anything to the blockchain. This can be used for methods that only read from the blockchain. This can also be used to check whether the method will run successfully given the inputs. This is the call method of Web3.

**Input:**

* Method name \(text\): The name of the method
* Parameters \(type: list\): A list of the parameters that need to be passed into the method
* Value \(Text, optional\): The amount of Gas you want to send to the Smart Contract when you’re calling the method
* Gas \(Number, optional\): \(same as SendTransaction\) The amount of Gas that will be used to write this transaction onto the blockchain. Unused gas will be returned.
* Gas Price \(Text, optional\): The price of gas for this transaction in wei

**Outputs:**

* Result \(Any\): This is the value that the method returned.
* Error \(Object\): Any error that occurred while running the method.

## **Estimate Gas**

![](.gitbook/assets/image%20%2840%29.png)

This is similar to the Method\_RunOnly block. The EstimateGas block  does a practice run of the Method with the given inputs and returns an estimate of how much Gas it will cost to run the method.

**Input:**

* Method name \(text\): The name of the method
* Parameters \(type: list\): A list of the parameters that need to be passed into the method
* Value \(Text, optional\): The amount of Gas you want to send to the Smart Contract when you’re calling the method
* Gas \(Number, optional\): \(same as SendTransaction\) The amount of Gas that will be used to write this transaction onto the blockchain. Unused gas will be returned.
* Gas Price \(Text, optional\): The price of gas for this transaction in wei

**Output:**

* GasAmount: How much gas it will cost to run the method.
* Error: Any errors that happened while estimating.

## **Subscribe To Event**

![](.gitbook/assets/image%20%2886%29.png)

Similar to the ****SubscribeToLogs block.

**Input:**

* Event name: Name of the event as specified in the smart contract
* Filter \(optional\): Lets you filter events by indexed parameters, e.g. {filter: {myNumber: \[12,13\]}} means all events where “myNumber” is 12 or 13.
* From Block \(optional\): The block number from which to get events on.
* Topics \(optional\): This allows to manually set the topics for the event filter. If given the filter property and event signature, \(topic\[0\]\) will not be set automatically.

**Output:**

* Callback is called whenever a new event occurs. The following parameters are passed into the callback:
* logEntry \(object\): Is not undefined everytime a new event that matches the topics, addresses, etc. happens. Example

**`{  
    returnValues: {  
        myIndexedParam: 20,  
        myOtherIndexedParam: '0x123456789...',  
        myNonIndexParam: 'My String'  
    },  
    raw: {  
        data: '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385',  
        topics: ['0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7', '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385']  
    },  
    event: 'MyEvent',  
    signature: '0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7',  
    logIndex: 0,  
    transactionIndex: 0,  
    transactionHash: '0x7f9fade1c0d57a7af66ab4ead79fade1c0d57a7af66ab4ead7c2c2eb7b11a91385',  
    blockHash: '0xfd43ade1c09fade1c0d57a7af66ab4ead7c2c2eb7b11a91ffdd57a7af66ab4ead7',  
    blockNumber: 1234,  
    address: '0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe'  
}`**

* * **changedLog \(object\): This output is there every time a log is removed from the blockchain.**
  * **Error \(object\): Is there when an error occurs with the subscription**

\(Please note: Oasis Labs is a beta product. As a result there may be system updates that impact your app's ability to connect to the platform or even loose data during major quarterly upgrades. You can learn more [_here_](http://docs.oasiscloud.io/en/latest/dashboard-quickstart/) about upgrade cycles\)

