# Blockchain Loan Tracker

Blockchain Loan Tracker is a decentralized application (dApp) built on Ethereum that allows users to manage loans using smart contracts. The application provides separate dashboards for users and administrators to interact with the blockchain.

## Features

- **User Dashboard**: 
  - View loan details.
  - Repay loans.

- **Admin Dashboard**: 
  - Create new loans.
  - View loan details.

- **Smart Contract Integration**: 
  - Uses Ethereum smart contracts to manage loan creation, repayment, and status tracking.

## Project Structure

blockchain-loan-tracker/
├── .gitignore                # Git ignore file
├── package.json              # Backend dependencies and scripts
├── truffle-config.js         # Truffle configuration for deploying smart contracts
├── build/                    # Compiled smart contracts
│   ├── contracts/            # ABI and bytecode of deployed contracts
├── contracts/                # Solidity smart contracts
│   ├── LoanTracker.sol       # Main smart contract for loan tracking
├── migrations/               # Deployment scripts for smart contracts
│   ├── 1_deploy_loan_tracker.js
├── test/                     # Smart contract tests
│   ├── LoanTracker.test.js   # Unit tests for LoanTracker contract
├── loan-tracker-frontend/    # React frontend for the application
│   ├── .env                  # Environment variables for the frontend
│   ├── .gitignore            # Git ignore file for frontend
│   ├── package.json          # Frontend dependencies and scripts
│   ├── README.md             # Frontend documentation
│   ├── public/               # Static assets for the frontend
│   │   ├── index.html        # HTML template for React app
│   │   ├── favicon.ico       # Favicon for the app
│   ├── src/                  # React source code
│   │   ├── App.js            # Main React component
│   │   ├── App.css           # Styling for the app
│   │   ├── index.js          # Entry point for React app
│   │   ├── components/       # Reusable React components
│   │   ├── services/         # API and blockchain interaction logic
│   ├── build/                # Production build of the React app
│   │   ├── static/           # Minified JS, CSS, and assets
│   │   ├── index.html        # Production HTML file

## Installation

To set up the project locally, run the following commands:

1. Clone the Repository

```bash
git clone <https://github.com/Sahilph46x/SmartLoan_Tracker.git>
cd blockchain-loan-tracker
```

2. Install Backend Dependencies

```bash
npm install
```

3. Compile Smart Contracts

Use Truffle to compile the smart contracts:
```bash
truffle compile
```

4. Deploy Smart Contracts

Deploy the smart contracts to a local blockchain (e.g., Ganache):

```bash
truffle migrate
```

5. Run Smart Contract Tests

Execute the tests to ensure the smart contracts work as expected:

```bash
truffle test
```

6. Set Up the Frontend

Navigate to the loan-tracker-frontend directory:

```bash
cd loan-tracker-frontend
```
Install the frontend dependencies:

```bash
npm install
```

7. Configure Environment Variables

Create a .env file in the loan-tracker-frontend directory and add the required environment variables, such as the blockchain network URL and contract address.

8. Run the Frontend in Development Mode

Start the React development server:

```bash
npm start
```

Open http://localhost:3000 in your browser to view the app.

9. Build the Frontend for Production

To create a production build of the React app:

```bash
npm run build
```

The production-ready files will be available in the build directory.

10. Deploy the Application
Deploy the production build to a hosting service of your choice (e.g., AWS, Netlify, or Vercel).
