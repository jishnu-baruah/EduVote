# EduVote

EduVote is an education-themed Web3 voting application designed to facilitate secure, transparent, and tamper-proof voting for school and college elections. Leveraging blockchain technology, EduVote ensures that every vote is immutably recorded, fostering trust in student governance and promoting democratic participation.

## Features

- **Secure Voting**: All votes are recorded on the blockchain, ensuring transparency and security.
- **Immutable Records**: Blockchain technology guarantees that votes cannot be tampered with or altered.
- **Educational Focus**: EduVote teaches students the importance of voting and civic engagement in a modern, digital world.

## Installation

### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [Hardhat](https://hardhat.org/)
- Access to a blockchain network (e.g., Volta, Ethereum testnets)

### Steps

1. **Clone the Repository**

   Clone this repository to your local machine:

   ```shell
   git clone https://github.com/your-username/eduvote.git
   cd eduvote
   ```

2. **Install Packages**

   Install the necessary packages using npm:

   ```shell
   npm install
   ```

3. **Compile and Deploy the Smart Contract**

   Compile the smart contract using Hardhat:

   ```shell
   npx hardhat compile
   ```

   Deploy the contract to your chosen blockchain network:

   ```shell
   npx hardhat run --network opencampus scripts/deploy.js
   ```

   After deployment, copy the contract address displayed in the terminal.

4. **Update Contract Address in Constants**

   Open the file where your contract address is stored (usually in a `constants` file, such as `src/constants.js` or `src/config.js`), and update it with the new contract address:

   ```javascript
   export const CONTRACT_ADDRESS = 'your_new_contract_address';
   ```

5. **Configure Environment Variables**

   Create a `.env` file in the root directory and add your private key:

   ```plaintext
   PRIVATE_KEY=your_private_key
   ```

   - **PRIVATE_KEY**: Your wallet's private key (ensure this is kept secure).

   Optionally, you can configure a different blockchain endpoint by modifying the `hardhat.config.js` file.

6. **Start the Application**

   With the contract address updated and environment variables set, start the application:

   ```shell
   npm start
   ```

   The application will run locally, allowing you to interact with the EduVote platform.

## Usage

After starting the application, you can access the EduVote platform through your browser. Follow the on-screen instructions to participate in or manage elections.

## Contributing

Contributions are welcome! If you'd like to contribute to EduVote, please fork the repository and submit a pull request. For major changes, please open an issue to discuss your ideas.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Hardhat**: For providing a robust development environment for Ethereum.
- **Node.js**: For making server-side JavaScript a reality.
- **Blockchain Community**: For the ongoing development of decentralized technologies.

---

This README provides clear instructions on how to update the contract address in the project's constants file and guides users through the setup process.