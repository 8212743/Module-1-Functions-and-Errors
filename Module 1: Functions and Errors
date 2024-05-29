// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract AssertionExample {
    uint256 public someValue;

    function setValue(uint256 _value) public {
        // Use require() to validate inputs
        require(_value != 0, "Value cannot be zero");
        
        // Use assert() to check for conditions that should never be false
        assert(_value != 999);
        
        // Set the value
        someValue = _value;
    }
    
    function setValueWithRevert(uint256 _value) public {
        // Use revert() to revert the transaction with a custom error message
        if (_value == 999) {
            revert("Cannot set value to 999");
        }
        
        // Set the value
        someValue = _value;
    }
}
