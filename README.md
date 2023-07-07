# require-assert-and-revert-functions-in-solidity
Metacrafters Assessment

# MyContract

This is a smart contract written in Solidity version 0.8.0. It contains three functions for testing different error handling mechanisms: RequireTest, AssertTest, and RevertTest.

## RequireTest

solidity
function RequireTest(uint _number) public pure {
    require(_number > 20, "Number must be greater than 20");
}


The RequireTest function checks if the input _number is greater than 20 using the require statement. If the condition is not met, it will revert the transaction with the error message "Number must be greater than 20".

## AssertTest

solidity
function AssesrtTest(uint _number) public pure {
    assert(_number == 20);
}


The AssertTest function uses the assert statement to validate if the input _number is equal to 20. If the condition is false, it will throw an exception and revert the transaction.

## RevertTest

solidity
function RevertTest(uint _number) public pure {
    if (_number < 20) {
        revert("Number must be greater than 20");
    }
}


The RevertTest function checks if the input _number is less than 20 using an if statement. If the condition evaluates to true, it will revert the transaction with the error message "Number must be greater than 20".

->Please note that all these functions are declared as pure, meaning they don't modify any state variables and can be called without making a transaction on the blockchain.
