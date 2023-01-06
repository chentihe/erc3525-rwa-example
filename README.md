# ERC3525 Example
## ERC3525
[EIP3525](https://eips.ethereum.org/EIPS/eip-3525) is new token standard proposed by Solv Finance.  It brings a new concept to abstract fungible token by using **<id - slot - value>** constructure. In this example, slot can be seen as a container of a real world asset, user can mint a ERC-3525 with a value which is binding with token id.
## Metadata Descriptor
Since every SFT(Solv Finance called ERC-3525 Semi-Fungible-Token) has different value, it is suggested to use metadata contract to generate metadata on-chain, so that the image can be displayed dynamically. Moreover, you can integrate with chainlink to fetch off-chain data and render on your SFT image.
## Test
All unit test is written on the test folder, you can see the test result by following below steps.  
This is forge project, make sure you install [foundry](https://book.getfoundry.sh/) in advance.
1. clone the project
```bash
$ git clone https://github.com/chentihe/erc3525-rwa-example.git
$ cd erc3525-rwa-example
```
2. install denpendencies
```bash
$ forge install
$ forge remappings
```
3. run unit test
```bash
$ forge test
```
