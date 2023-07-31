# EcommercePaymentWallet
 The "EcommerceWallet" contract is a Solidity smart contract that functions as a simple e-commerce wallet with inventory management. The contract allows users to purchase items from the inventory using Ether (the native cryptocurrency of the Ethereum blockchain).  The contract has an owner, who is the creator of the contract and initially has a balance of 10,000 Ether. The inventory is initialized with two items, "item1" and "item2," each having a specific price and quantity available for purchase.  The main functionalities of the contract are as follows:  Constructor: Initializes the contract owner and sets the initial balance and inventory with predefined quantities and prices.  purchase(): Allows users to purchase items from the inventory. Users can specify the item they want to buy and the quantity. The contract checks if the item is available in sufficient quantity and if the user has sent enough Ether to cover the cost. If the conditions are met, the payment is transferred to the contract owner, and the inventory and contract balance are updated accordingly.  priceOf(): A helper function to retrieve the price of an item based on its name. It uses string comparison to determine the price of the requested item.  deposit(): Allows users to deposit Ether into the wallet. The deposited amount is added to the contract balance.  getBalance(): Allows users to check the current balance of the contract.  Note: The contract uses the Solidity version 0.8.0 and follows the MIT License. Users can interact with the contract functions using a compatible Ethereum wallet or a DApp browser.