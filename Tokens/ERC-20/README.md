# ERC-20

ERC-20 is a standard interface for fungible tokens, like voting tokens, staking tokens or virtual currencies.

## What is a Token?

Token in Ethereum can represent virtually things.

- reputation pointes in an online platform
- skills of a character in a game
- lottery tickets
- financial assets like a share in a company
- a fiat currency like USD
- an ounce of gold
- etc.

## What is ERC-20

ERC-20 introduce a standard for Fungible Tokens, in other words, they have a property that makes each Token be exactly the same (in type and value) as another Token.
For example, an ERC-20 Token acts just like the ETH, meaning that 1 Token is and will always be qual to all the other Tokens.

The ERC-20, proposed by Fabian Vogelsteller in November 2015, is a Token standard that implements an API for tokens within Smart Contracts.

### What ERC-20 provides

- transfer tokens from one account to another
- get the current token balance of an account
- get the totalsupply of the token available on the network
- approve whether an amount of token from an account can be spent by a third-party account

### Methods

```solidity
function name() public view returns (string)
function symbol() public view returns (string)
function decimals() public view returns (uint8)
function totalSupply() public view returns (uint256)
function balanceOf(address _owner) public view returns (uint256 balance)
function transfer(address _to, uint256 _value) public returns (bool success)
function transferFrom(address _from, address _to, uint256 _value) public returns (bool success)
function approve(address _spender, uint256 _value) public returns (bool success)
function allowance(address _owner, address _spender) public view returns (uint256 remaining)
```

### Events

```solidity
event Transfer(address indexed _from, address indexed _to, uint256 _value)
event Approval(address indexed _owner, address indexed _spender, uint256 _value)
```

## Reference

## OpenZeppelin

### Tokens

### ERC-20 Implementation

## Others

ABI: Application Binary Interface
