# ZK-SNARK-Designer

1. **Write a correct circuit.circom implementation:**
   - Develop the circuit in the Circom language, ensuring it accurately represents the desired functionality. 
   - Verify the correctness of the circuit logic by thorough testing and debugging.

2. **Compile the circuit to generate circuit intermediaries:**
   - Use the Circom compiler to compile the circuit.circom file and generate the required intermediaries, including the constraint system and the proving and verifying keys.

3. **Generate a proof using inputs A=0 B=1:**
   - With the compiled circuit and generated intermediaries, use a suitable proving tool such as snarkjs to generate a proof for the specified inputs (A=0, B=1). 
   - Ensure that the generated proof is valid and can be verified correctly.

4. **Deploy a Solidity verifier to Sepolia or Mumbai Testnet:**
   - Write a Solidity smart contract that includes the necessary verification logic to verify the proof generated in the previous step.
   - Deploy this verifier contract to the Sepolia or Mumbai Testnet using appropriate deployment tools such as Truffle or Hardhat.

5. **Call the `verifyProof()` method on the verifier contract and assert output is true:**
   - Once the verifier contract is deployed, interact with it either through a script or directly using a web3 provider.
   - Submit the proof generated earlier along with the inputs (A=0, B=1) to the `verifyProof()` method of the verifier contract.
   - Assert that the output of the verification is true, indicating that the proof is valid.

Make sure to follow best practices for each step, including code organization, documentation, and testing. Additionally, adhere to any specific requirements or guidelines provided for the Final Challenge.
- - -
