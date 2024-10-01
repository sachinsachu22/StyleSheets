# Contract MarginManager 

## Intro

The `MarginManager` contract is a simple Solidity smart contract designed to manage two margin values, `marginBox1` and `marginBox2`. It allows users to set these values while enforcing certain conditions to ensure data integrity.

## Features
> Set two margin values with constraints.
> Retrieve the current margin values.
> Ensures that both margins are greater than zero and are not equal.
> Validates that `marginBox1` is greater than `marginBox2`.

##  Functions used

### 1. `setMargin(uint256 _marginBox1, uint256 _marginBox2)`
Sets the values of `marginBox1` and `marginBox2`. The function enforces the following rules:

>Both margin values must be greater than zero.
>The two margin values must not be equal.
>`marginBox1` must be greater than `marginBox2`.

**Parameters:**
>`_marginBox1`: The value for the first margin box.
>`_marginBox2`: The value for the second margin box.

**Reverts:**
> If either margin is less than or equal to zero.
> If the two margin values are equal.
> If `marginBox2` is greater than or equal to `marginBox1`.

### 2. `getMargins()`

Returns the current values of `marginBox1` and `marginBox2`.

**Returns:**
>A tuple containing the values of `marginBox1` and `marginBox2`.

## Usage
To interact with the `MarginManager` contract:

1. Deploy the contract to a compatible Ethereum network.
2. Call the `setMargin` function with two positive margin values.
3. Use the `getMargins` function to retrieve the current margin values.

## License
This contract is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Author

Created by Sachin. 
Mail ID:sachinsachu25134@gmail.com
Date:1/10/2024
## Thank you
