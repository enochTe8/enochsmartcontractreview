# Decentralized Voting System

## Overview
This project is a decentralized voting system implemented as a smart contract on the Ethereum blockchain. The contract allows the owner to create proposals, and users can vote "Yes" or "No" on these proposals. The voting results are stored on the blockchain, ensuring transparency and immutability.

## Voting Mechanism
1. **Proposal Creation**: Only the contract owner can create proposals. Each proposal has a unique ID, description, and vote counts for "Yes" and "No" votes.
2. **Voting**: Users can vote on active proposals. Each user can vote only once per proposal. Votes are recorded as either "Yes" or "No".
3. **Vote Counting**: The contract keeps track of the number of "Yes" and "No" votes for each proposal. Users can query the proposal details to see the current vote counts.
4. **Ending Proposals**: The owner can end a proposal, making it inactive and preventing further votes.

## Deployment
To deploy the contract, follow these steps:
1. Install [Remix IDE](https://remix.ethereum.org/).
2. Create a new file and paste the Solidity code from `DecentralizedVotingSystem.sol`.
3. Compile the contract using the Solidity compiler.
4. Deploy the contract to the Ethereum network using a wallet like MetaMask.

## Interaction
Once deployed, you can interact with the contract using the following functions:
- `createProposal(string memory description)`: Creates a new proposal with the given description. Only the owner can call this function.
- `vote(uint proposalId, bool vote)`: Casts a vote on the specified proposal. Users can vote "Yes" (true) or "No" (false).
- `endProposal(uint proposalId)`: Ends the specified proposal, making it inactive. Only the owner can call this function.
- `getProposal(uint proposalId)`: Returns the details of the specified proposal, including the description, "Yes" votes, "No" votes, and active status.

## Skills Demonstrated
- Smart contract design for governance.
- Understanding of decentralized systems.
- Deployment and interaction with Ethereum.

