# Smart contract to create your own token and add it to your ERC20 Wallet like Metamask

This Project contains a smart contract that allows you to create your own token and add it to your ERC20 Wallet like Metamask.

### Files
`smartcontract/webmafiatoken.sol` : This File is an smart contract which is importing/extending the ERC20 standard from OpenZeppelin.

This File has a smart contract Named WebMafia which Extends ERC20 standard.

`contract WebMafia is ERC20`

This contract contains a constructor function to initialize the contract with the Token name and symbol. Which calls ERC20 constructor function with same name to utilise all the standard functionality of ERC20 standards.

`constructor(string memory _name, string memory _symbol) ERC20(_name, _symbol) {`
        `_mint(msg.sender, 10 * 10 ** 18);`
`}`

This contract can be deployed on the Rinkby network.
Initilise the contract contrator with Name and Symbol before deployment.

You will be able to create your contract. These coins could not easily be autotracked in your wallet as they are commonly used ERC20 tokens. You can import your coins using import contract using the deployed contract address.