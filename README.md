# Flash Loan Arbitrage Starter

This repository provides a professional-grade foundation for interacting with Aave V3 Flash Loans. It allows developers to borrow millions in liquidity, perform operations, and repay the loan in a single atomic transaction.

## Features
- **Aave V3 Integration**: Uses the latest `IPool` interfaces.
- **Gas Optimized**: Minimalist logic to ensure high profitability for arbitrage.
- **Safety**: Built-in checks to ensure the transaction reverts if the profit doesn't cover the flash loan fee.

## Workflow
1. Call `requestFlashLoan` with the asset and amount.
2. Aave sends funds to the contract.
3. `executeOperation` is triggered—this is where you place your arbitrage/swap logic.
4. Contract automatically repays the loan + fee.



## License
MIT
