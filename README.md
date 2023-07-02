# require-assert-and-revert-functions-in-solidity
Metacrafters Assessment


This is a simple Solidity smart contract that allows the owner to set, increment, and decrement a number.

## Functions

### setNumber(uint _number)

This function allows the owner to set the value of myNumber. It takes an input parameter _number of type uint256. The _number must be greater than 0, otherwise the transaction will revert with an error message.

### incrementNumber()

This function allows the owner to increment the value of myNumber by 1. It first stores the current value of myNumber in a variable oldNumber, then increments myNumber by 1. After the increment, it asserts that myNumber is greater than oldNumber. If this assertion fails, the transaction will revert.

### decrementNumber()

This function allows the owner to decrement the value of myNumber by 1. It first stores the current value of myNumber in a variable oldNumber, then decrements myNumber by 1. If myNumber becomes negative after the decrement, the transaction will revert with an error message.

## State Variables

### myNumber

This state variable of type uint256 represents an unsigned integer. It stores the current value of the number.

## Constructor

The contract does not have a constructor defined explicitly, so it will use the default constructor provided by Solidity. The default constructor initializes myNumber to 0.

## Usage

1. Deploy the contract to a blockchain network.
2. Call the setNumber function with the desired number as the input parameter to set the value of myNumber.
3. Call the incrementNumber function to increment the value of myNumber by 1.
4. Call the decrementNumber function to decrement the value of myNumber by 1.

