# MetaMask ETH Bank
### Starter Next/Hardhat Project

After cloning the github, you will want to do the following to get the code running on your computer.

1. Inside the project directory, in the terminal type: npm i
2. Open two additional terminals in your VS code
3. In the second terminal type: npx hardhat node
4. In the third terminal, type: npx hardhat run --network localhost scripts/deploy.js
5. Back in the first terminal, type npm run dev to launch the front-end.

After this, the project will be running on your localhost. 
Typically at http://localhost:3000/

## Smart Contract (Assessment.sol)
The Assessment.sol file contains the Solidity smart contract for the bank. It includes the following functionalities:
- constructor(uint initBalance): Initializes the contract with an initial balance set by the deployer (owner).
- getBalance(): Returns the current balance of the contract.
- deposit(uint256 _amount): Allows the owner of the contract to deposit funds into the bank.
- withdraw(uint256 _withdrawAmount): Allows the owner of the contract to withdraw funds from the bank, provided the balance is sufficient.

## How the Application Works
1. When the application loads, it checks for the presence of MetaMask. If MetaMask is detected, the user is prompted to connect their wallet.
2. Once the user connects their wallet, the application fetches the user's account address and displays it on the homepage.
3. The user's account balance (in ETH) is also displayed on the homepage.
4. The user can deposit and withdraw funds using the provided input fields and buttons.
5. Transaction history is displayed below the balance section, showing the type of transaction (deposit or withdraw), the amount, and the date.
