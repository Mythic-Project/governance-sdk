# Mythic-Project Governance SDK

The **Governance SDK** is a TypeScript-based library enabling developers to create, manage, and interact with decentralized governance systems, specifically designed for Realms DAO on the Solana blockchain. It simplifies building governance applications by abstracting low-level blockchain operations into intuitive APIs.

---

## **Repository Structure**

### **`dist/`**
- Contains the compiled JavaScript files ready for distribution and deployment.

### **`src/`**
The core of the SDK, written in TypeScript, structured as follows:

#### **Subdirectories and Files**

1. **`client/`**
   - **`GovernanceClient.ts`**  
     The main class for interacting with the governance SDK. It provides methods for initializing governance structures, creating proposals, and managing votes. Designed to simplify interaction with Solana RPC endpoints.
   - **`index.ts`**  
     Exports the `GovernanceClient` and other utilities within the client module.

2. **`instructions/`**
   - **`createProposal.ts`**  
     Handles the instruction for creating new governance proposals. This module generates the necessary transaction for proposal submission to the blockchain.
   - **`castVote.ts`**  
     Implements the logic for casting votes on proposals, including transaction construction and signing.
   - **`initializeGovernance.ts`**  
     Provides instructions to initialize governance structures, including setting up configurations and governance accounts on Solana.
   - **`index.ts`**  
     Serves as an aggregator for all governance-related instructions, making imports and usage easier.

3. **`utils/`**
   - **`validation.ts`**  
     Includes helper functions to validate user inputs, such as proposal names, vote options, and governance configurations.
   - **`transactions.ts`**  
     Contains utility functions for creating, signing, and submitting blockchain transactions.
   - **`constants.ts`**  
     Stores shared constants like program IDs, cluster URLs, and other configuration values.

4. **`types/`**
   - **`governanceTypes.ts`**  
     Defines TypeScript types and interfaces for governance entities, such as `Proposal`, `Vote`, and `GovernanceConfig`. This ensures type safety and clarity across the SDK.
   - **`index.ts`**  
     Centralizes exports for all type definitions.

5. **`index.ts`**
   - Entry point of the SDK, aggregating and exporting all modules, instructions, and utilities.

---

## **Setup Instructions**

### **1. Clone the Repository**
```bash
git clone https://github.com/Mythic-Project/governance-sdk.git
cd governance-sdk
```

### **2. Install Dependencies**
Make sure you have [Node.js](https://nodejs.org/) installed, then run:
```bash
npm install
```

### **3. Build the SDK**
Compile TypeScript into JavaScript:
```bash
npm run build
```

### **4. Run Tests**
Run the test suite to verify functionality:
```bash
npm test
```

---

## **Usage**

This SDK provides an intuitive API to interact with Solana-based governance systems. Import the SDK and use the provided `GovernanceClient` for all operations, including creating proposals, casting votes, and initializing governance configurations.

---

## **Contributing**
This README was createad by a community member of Realms. I don't know if contributions are welcome but If they are, I would follow this format:

### **How to Contribute**
1. Fork the repository.
2. Create a feature branch.
3. Implement your changes, ensuring all tests pass.
4. Submit a pull request with a clear description.

### **Contribution Guidelines**
- Follow the existing code style and structure.
- Write tests for any new features or modifications.
- Include detailed comments and documentation.

---

## **Contact**

For support, feature requests, or bug reports, open an issue on the [GitHub repository](https://github.com/Mythic-Project/governance-sdk/issues).

---

*This README provides a detailed breakdown of the repository structure and its key components, making it easier for developers to understand and contribute.*

*This README was written by a non-team member, there may be mistakes or issues when implementing the code. Follow README at your own risk*
