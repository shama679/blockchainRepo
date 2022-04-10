# Blockchain Project 
First of all we need to install node.js on any platform like visual studio.So, after installation of node.js file we need to install pacakages like Lock.json and pacakage.json files.
Then we need to run command distribute.js if is giving some errors like module not found then we need to run another command
(`npm i fs big-number web3 ethereumjs-txt`)
if it is giving again error then, make sure that 
**web3** must be installed.
Then run again distribute.js file and see it is working or not if it is still not working we need to replace file
**Dotenv to  .env**
Now again run command 
**(`node distribute.js`)** probably the error will be gone then.
iF it is working perfect, now we need to put the following Adesses:
 **Infura_Token**
 **Contract_Address**
 **Owener_Address**
**Super_Secret_Private_Key**\
in the **.env** .

You can get all these files from Following Tools:
* **Infura**
* **MetaMask**
* **Remix ID**
* **EtherScan**\
 **DeployedContract.sol** 
We need to run this file in the Remix ID and then need to deploy this after deployed you will get contract address;\
Here in this file you have to change few lines to your own values;\
 **constructor() \{**
       **_name = "MY SPECIAL TOKEN"; \
        _symbol = "MST";**\
Here you need to change "MY SPECIAL TOKEN" with Your own Token Name ;\ and you need to change Symbol as well with your own shortcut name;
And Also you need to change something here;\
**contract ERC20 is Context, IERC20, IERC20Metadata {\
    mapping(address => uint256) private _balances;**\
Here you need to write your name with ERC20 like **MSTERC20**\

**Accounts.txt**
In this file there all accounts where your token will be going to distribute.we can add our own accounts here as well.\
**Contract.js**
This file will keep record of your all address and trancations and everything.\
After doing all these steps you need to again run command **(`node distribute.js`)**  then your tokens will be transfer to those 10 accounts which is in Accounts.txt
