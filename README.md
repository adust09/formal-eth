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

## Projects
### Cryptography

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| KZG Commitment | Polynomial Commitment | [✅](https://github.com/tobias-rothmann/Polynomial-Commitment-Schemes) | Isabelle/HOL |

### Protocol

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| Ethereum PoS | L1 | [✅](https://github.com/ConsenSys/eth2.0-dafny) | Dafny |
| Casper FFG | L1 | [✅](https://github.com/runtimeverification/casper-proofs) | Rocq |
| RANDAO | L1 | [✅](https://github.com/runtimeverification/rdao-smc) | Maude, PVeStA |
| Staking deposit contract | L1 | [✅](https://github.com/runtimeverification/deposit-contract-verification) | K Framework |
| [Cairo (language)](https://github.com/starkware-libs/cairo-lang) | zkVM (language) | [✅](https://github.com/starkware-libs/formal-proofs) | Lean |
| [Jolt](https://github.com/a16z/jolt) | zkVM | [🏗️ WIP](https://github.com/GaloisInc/zk-lean) | Lean |

### Application

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| [Uniswap V3](https://github.com/Uniswap/v3-core) | DEX | ✅ | Isabelle/HOL based custom tool |
| [Uniswap V4](https://github.com/Uniswap/v4-core) | DEX | [✅](https://certora.cdn.prismic.io/certora/Z4UNepbqstJ99YI5_InformedeSeguridadUniswapV4.pdf) | Certora Prover |
| Compound V3 | Lending | [✅](https://certora.cdn.prismic.io/certora/e7ca6508-fad8-4a41-8588-b3312d8b750e_Compound+Report.pdf) | Certora Prover |


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

## Vulnerability Detection

### Specific Vulnerability Research

- **[Reentrancy Verification](https://github.com/ConsenSys/mythril)** - Reentrancy attack verification using Z3 SMT solver
- **[SmartScan](https://github.com/smartdec/smartcheck)** - Formal verification framework detecting 14 types of vulnerabilities

### Common Vulnerability Patterns

- **Integer Overflow/Underflow** - Mathematical verification of arithmetic operations
- **Reentrancy Attacks** - State machine verification and call graph analysis
- **Access Control** - Permission model verification
- **Time Dependencies** - Temporal logic verification


## Educational Resources

### Tutorials and Guides

- TBD

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
