# EcommercePaymentWallet
 The "EcommerceWallet" contract is a Solidity smart contract that functions as a simple e-commerce wallet with inventory management. 
 The contract allows users to purchase items from the inventory using Ether (the native cryptocurrency of the Ethereum blockchain).  
 The contract has an owner, who is the creator of the contract and initially has a balance of 10,000 Ether. 
 The inventory is initialized with two items, "item1" and "item2," each having a specific price and quantity available for purchase.  

 The main functionalities of the contract are as follows:  
 Constructor: Initializes the contract owner and sets the initial balance and inventory with predefined quantities and prices.  
 purchase(): Allows users to purchase items from the inventory. Users can specify the item they want to buy and the quantity. The contract checks if the item is available in sufficient quantity and if the user has sent enough Ether to cover the cost. If the conditions are met, the payment is transferred to the contract owner, and the inventory and contract balance are updated accordingly. 
 priceOf(): A helper function to retrieve the price of an item based on its name. It uses string comparison to determine the price of the requested item.  
 deposit(): Allows users to deposit Ether into the wallet. The deposited amount is added to the contract balance.  
 getBalance(): Allows users to check the current balance of the contract.  
 
 The "EcommerceWallet" contract can serve as a payment wallet within this broader e-commerce system. Users could deposit funds into the wallet, and when they make a purchase, the payment can be deducted from the wallet's balance. The smart contract's inventory management ensures that items are deducted from stock when sold, and the owner of the contract receives payments for the sold items.

Scope for the project(Future Implimentation):

We will typically have several other components and smart contracts to handle various aspects, such as:

Product Catalog: A smart contract or database that stores information about the products available for purchase, including their names, descriptions, prices, and other relevant details.

User Management: A system to handle user registration, authentication, and access control.

Shopping Cart: A feature that allows users to add items to their cart before making a purchase.

Order Processing: A mechanism for processing and managing orders, including order status, shipping information, etc.

Payment Gateway: Integration with external payment gateways (e.g., Stripe, PayPal) to handle real-world currency conversions and payment processing securely.

Escrow Mechanism: A way to ensure trust and security in transactions, especially for high-value purchases.

Front-end Interface: A user-friendly interface (e.g., a website or a mobile app) that allows users to browse products, add items to the cart, make purchases, and view order history.

 
 
 Note: The contract uses the Solidity version 0.8.0 and follows the MIT License. Users can interact with the contract functions using a compatible Ethereum wallet or a DApp browser.
