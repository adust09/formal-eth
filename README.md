# Awesome Ethereum Formal Verification [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome Ethereum formal verification tools, projects, and resources

Formal verification is a mathematical approach to proving the correctness of smart contracts and blockchain protocols. This list focuses on formally verified Ethereum-related projects, tools, and academic research.

## Contents

- [Formal Verification Tools](#formal-verification-tools)
- [Verified Projects](#verified-projects)
- [Security Reports](#security-reports)
- [Academic Research](#academic-research)
- [Vulnerability Detection](#vulnerability-detection)
- [Educational Resources](#educational-resources)
- [Tools by Category](#tools-by-category)
- [Contributing](#contributing)
- [License](#license)

## Formal Verification Tools

### Production-Ready Tools

- **[Certora Prover](https://www.certora.com/)** - Advanced formal verification tool for EVM, Solana, and Stellar chains
- **[Microsoft VeriSol](https://github.com/microsoft/verisol)** - Microsoft's formal verifier for Solidity smart contracts
- **[K Framework (KEVM)](https://github.com/kframework/evm-semantics)** - Ethereum verification using K specifications
- **[Coq-of-Python](https://github.com/formal-land/coq-of-python)** - Converts Ethereum's Python implementation to Coq for formal verification

### Emerging Tools

- **[HEVM](https://github.com/dapphub/dapptools/tree/master/src/hevm)** - Ethereum Virtual Machine for symbolic execution and formal verification
- **[Manticore](https://github.com/trailofbits/manticore)** - Symbolic execution tool for analysis of smart contracts
- **[Mythril](https://github.com/ConsenSys/mythril)** - Security analysis tool for Ethereum smart contracts

## Verified Projects

### Core Infrastructure

- **[ENS (Ethereum Name Service)](https://ens.domains/)** - Formally verified using K Framework
- **[Ethereum 2.0 Deposit Contract](https://github.com/ethereum/deposit_contract)** - Verified by Runtime Verification
- **[EIP-1559](https://eips.ethereum.org/EIPS/eip-1559)** - Fee market mechanism with formal analysis

### DeFi Protocols

- **[DJED Stablecoin](https://djed.one/)** - Formally verified algorithmic stablecoin
- **[Sarcophagus Protocol](https://sarcophagus.io/)** - Verified using Certora
- **[Compound Protocol](https://compound.finance/)** - Partially verified money market protocol

### Layer 2 Solutions

- **[Polygon Hermez](https://hermez.io/)** - ZK-rollup with formal verification components
- **[StarkNet](https://starknet.io/)** - STARK-based rollup with mathematical proofs

### Zero-Knowledge Virtual Machines (zkVMs)

- **[Ethproofs](https://github.com/ethproofs/ethproofs)** - SNARKifying Ethereum with zkVM security and performance metrics
- **[ZKSMT](https://github.com/usenix-security)** - Virtual machine for proving SMT theorems in zero knowledge
- **[Ceno zkVM](https://github.com/scroll-tech/ceno)** - Non-uniform, segment and parallel zero-knowledge virtual machine framework
- **[RISC Zero](https://github.com/risc0/risc0)** - General-purpose zkVM with formal verification components</search>
</search_and_replace>

## Security Reports

### Audit Portfolios

- **[Certora Security Reports](https://www.certora.com/reports)** - Comprehensive formal verification and audit reports for major Web3 protocols
- **[Runtime Verification Reports](https://runtimeverification.com/smartcontract)** - Formal verification reports for blockchain projects
- **[Trail of Bits Publications](https://blog.trailofbits.com/)** - Security research and formal methods applications

## Academic Research

### Research Projects

- **[Ethereum Formal Verification Overview](https://github.com/leonardoalt/ethereum_formal_verification_overview)** - Comprehensive overview of formal verification in the Ethereum ecosystem
- **[EthBench](https://github.com/ucsb-seclab/ethbench)** - Formal verification benchmark for Ethereum smart contracts
- **[Awesome Web3 Formal Verification](https://github.com/saeidshirazi/Awesome-Smart-Contract-Security-Tools)** - Curated list of Web3 formal verification resources

### Academic Papers

- **[A Survey of Smart Contract Formal Verification](https://arxiv.org/abs/1909.07633)** - Comprehensive survey of formal verification techniques
- **[Formal Verification of Smart Contracts](https://dl.acm.org/doi/10.1145/3243734.3243795)** - ACM survey on smart contract verification
- **[Security Analysis of Smart Contracts](https://ieeexplore.ieee.org/document/8449446)** - IEEE paper on formal methods for smart contract security

### zkVM Research Papers

- **[A Parameterized Framework for the Formal Verification of Zero-Knowledge Virtual Machines](https://dl.acm.org/doi/10.1145/3658644.3690184)** - ACM SIGPLAN 2024 paper on formal verification of zkVMs in Coq
- **[ZKSMT: A VM for Proving SMT Theorems in Zero Knowledge](https://www.usenix.org/conference/usenixsecurity24)** - USENIX Security 2024 paper on virtual machines for zero-knowledge proofs
- **[Ceno: Non-uniform, Segment and Parallel Zero-Knowledge Virtual Machine](https://eprint.iacr.org/2024/387)** - IACR ePrint on novel zkVM framework leveraging succinct proofs
- **[A Survey on the Applications of Zero-Knowledge Proofs](https://arxiv.org/abs/2402.04878)** - Comprehensive survey including formally verified zero-knowledge virtual machines

## Vulnerability Detection

### Specific Vulnerability Research

- **[Reentrancy Verification](https://github.com/ConsenSys/mythril)** - Reentrancy attack verification using Z3 SMT solver
- **[SmartScan](https://github.com/smartdec/smartcheck)** - Formal verification framework detecting 14 types of vulnerabilities
- **[ERC Properties HEVM](https://github.com/dapphub/erc20-formal-verification)** - Formal verification of ERC properties using HEVM

### Common Vulnerability Patterns

- **Integer Overflow/Underflow** - Mathematical verification of arithmetic operations
- **Reentrancy Attacks** - State machine verification and call graph analysis
- **Access Control** - Permission model verification
- **Time Dependencies** - Temporal logic verification

### zkVM Security Verification

- **[zkVM Constraint Verification](https://github.com/ethproofs/ethproofs)** - Security and performance metrics for zkVM implementations
- **[Zero-Knowledge Proof Soundness](https://eprint.iacr.org/2024/387)** - Formal verification of zkVM proof systems
- **[Circuit Satisfiability Verification](https://github.com/risc0/risc0)** - Mathematical verification of zkVM circuit constraints
- **[Trusted Setup Verification](https://github.com/scroll-tech/ceno)** - Formal analysis of zkVM trusted setup procedures

## Educational Resources

### Tutorials and Guides

- **[Formal Verification Tutorial](https://github.com/runtimeverification/verified-smart-contracts)** - Step-by-step guide to formal verification
- **[Certora Documentation](https://docs.certora.com/)** - Comprehensive documentation for Certora Prover
- **[K Framework Tutorial](https://github.com/kframework/k/tree/master/k-distribution/tutorial)** - Learning K for blockchain verification

### Courses and Workshops

- **[Formal Methods for Smart Contracts](https://www.coursera.org/learn/formal-methods)** - Online course on formal verification
- **[Runtime Verification Workshops](https://runtimeverification.com/workshops)** - Regular workshops on formal methods

## Tools by Category

### Static Analysis
- Slither
- Securify
- SmartCheck

### Dynamic Analysis
- Echidna
- Harvey
- ContractFuzzer

### Symbolic Execution
- Manticore
- SAGE
- KLEE

### Model Checking
- TLA+
- CBMC
- SPIN

### Zero-Knowledge Virtual Machines
- RISC Zero
- Ceno zkVM
- Ethproofs
- Plonky2

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

### Guidelines

1. **Quality over quantity** - Only include high-quality, actively maintained projects
2. **Provide descriptions** - Each entry should have a clear, concise description
3. **Verify links** - Ensure all links are working and point to the correct resources
4. **Follow format** - Maintain consistent formatting throughout the list
5. **Stay relevant** - Focus on Ethereum and EVM-compatible formal verification

### How to Contribute

1. Fork this repository
2. Create a new branch for your additions
3. Add your entry in the appropriate section
4. Ensure your addition follows the format
5. Submit a pull request with a clear description

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.

---

**Note**: This list is continuously updated. If you find any broken links or outdated information, please open an issue or submit a pull request.
