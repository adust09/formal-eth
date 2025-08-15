# Awesome Ethereum Formal Verification [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome Ethereum formal verification tools, projects, and resources

Formal verification is a mathematical approach to proving the correctness of smart contracts and blockchain protocols. This list focuses on formally verified Ethereum-related projects, tools, and academic research.

## Contents

- [Awesome Ethereum Formal Verification ](#awesome-ethereum-formal-verification-)
  - [Contents](#contents)
  - [Projects](#projects)
    - [Cryptography](#cryptography)
    - [Protocol](#protocol)
    - [Application](#application)
  - [Formal Verification Tools](#formal-verification-tools)
    - [Production-Ready Tools](#production-ready-tools)
    - [Emerging Tools](#emerging-tools)
  - [Security Reports](#security-reports)
    - [Audit Portfolios](#audit-portfolios)
  - [Academic Research](#academic-research)
    - [Research Projects](#research-projects)
    - [Academic Papers](#academic-papers)
  - [Vulnerability Detection](#vulnerability-detection)
    - [Specific Vulnerability Research](#specific-vulnerability-research)
  - [Contributing](#contributing)
    - [Guidelines](#guidelines)
    - [How to Contribute](#how-to-contribute)
  - [License](#license)

## Projects
### Cryptography

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| KZG Commitment | Commitment Scheme | [✅](https://github.com/tobias-rothmann/Polynomial-Commitment-Schemes) | Isabelle/HOL |
| Merkle Tree | Commitment Scheme | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| Binius | Commitment Scheme | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| Sumcheck | Interactive Oracle Proof | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| FRI | Interactive Oracle Proof | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| STIR | Interactive Oracle Proof | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| WHIR | Interactive Oracle Proof | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |
| Spartan | Interactive Oracle Proof | [🏗️ WIP](https://github.com/Verified-zkEVM/ArkLib) | Lean |

### Protocol

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| Ethereum PoS | L1 | [✅](https://github.com/runtimeverification/beacon-chain-verification), [✅](https://github.com/ConsenSys/eth2.0-dafny) | Rocq, Dafny |
| Casper FFG | L1 | [✅](https://github.com/runtimeverification/casper-proofs) | Rocq |
| RANDAO | L1 | [✅](https://github.com/runtimeverification/rdao-smc) | Maude, PVeStA |
| Staking deposit contract | L1 | [✅](https://github.com/runtimeverification/deposit-contract-verification) | K Framework |
| [EIP1559](https://eips.ethereum.org/EIPS/eip-1559) | EIP | [✅](https://ieeexplore.ieee.org/document/9842730) | UPPAAL |
| [Cairo (language)](https://github.com/starkware-libs/cairo-lang) | zkVM (language) | [✅](https://github.com/starkware-libs/formal-proofs) | Lean |
| [Jolt](https://github.com/a16z/jolt) | zkVM | [🏗️ WIP](https://github.com/GaloisInc/zk-lean) | Lean |
| [SP1](https://github.com/succinctlabs/sp1) | zkVM | [🏗️ WIP](https://medium.com/veridise/verifying-sp1-circuit-determinism-with-picus-a-collaboration-between-veridise-and-succinct-985c7a6dd9b5) | Picus |
| [RISC Zero](https://github.com/risc0/risc0) | zkVM | [🏗️ WIP](https://github.com/NethermindEth/risczero-fv) | Zirgen, Lean |
| [Intmax2](https://github.com/InternetMaximalism/intmax2) | Zk Rollup | [✅](https://github.com/NethermindEth/FVIntmax) | Lean |
| CBC Casper | (L1) | [✅](https://github.com/LayerXcom/cbc-casper-proof) | Isabelle/HOL |

### Application

| Name | Category | Formal Verification | Stack |
| ---- | ---- | ---- | ---- |
| [Uniswap V3](https://github.com/Uniswap/v3-core) | DEX | ✅ | Isabelle/HOL based custom tool |
| [Uniswap V4](https://github.com/Uniswap/v4-core) | DEX | [✅](https://certora.cdn.prismic.io/certora/Z4UNepbqstJ99YI5_InformedeSeguridadUniswapV4.pdf) | Certora Prover |
| Compound V3 | Lending | [✅](https://certora.cdn.prismic.io/certora/e7ca6508-fad8-4a41-8588-b3312d8b750e_Compound+Report.pdf) | Certora Prover |
| Euler Finance V2 | Lending | [✅](https://github.com/euler-xyz/fee-flow/tree/main/formal-verification) | Certora Prover |
| [DJED](https://github.com/DjedAlliance/Djed-Solidity)  | Stablecoin | [✅](https://iohk.io/en/research/library/papers/djed-a-formally-verified-crypto-backed-pegged-algorithmic-stablecoin/) | LUSTRE, Isabelle/HOL |
| AMM | DEX | [✅](https://github.com/danielepusceddu/lean4-amm) | Lean |


## Formal Verification Tools

### Production-Ready Tools

- **[Certora Prover](https://www.certora.com/)** - Advanced formal verification tool for EVM, Solana, and Stellar chains
- **[Microsoft VeriSol](https://github.com/microsoft/verisol)** - Microsoft's formal verifier for Solidity smart contracts
- **[K Framework (KEVM)](https://github.com/kframework/evm-semantics)** - Ethereum verification using K specifications
- **[Coq-of-Python](https://github.com/formal-land/coq-of-python)** - Converts Ethereum's Python implementation to Rocq(Coq) for formal verification
- **[Act](https://github.com/ethereum/act)** - Formal specification language for Ethereum smart contracts

### Emerging Tools

- **[HEVM](https://github.com/dapphub/dapptools/tree/master/src/hevm)** - Ethereum Virtual Machine for symbolic execution and formal verification
- **[Manticore](https://github.com/trailofbits/manticore)** - Symbolic execution tool for analysis of smart contracts
- **[Mythril](https://github.com/ConsenSys/mythril)** - Security analysis tool for Ethereum smart contracts

## Security Reports

### Audit Portfolios

- **[Certora Security Reports](https://www.certora.com/reports)** - Comprehensive formal verification and audit reports for major Web3 protocols
- **[Runtime Verification Reports](https://runtimeverification.com/smartcontract)** - Formal verification reports for blockchain projects
- **[Trail of Bits Publications](https://blog.trailofbits.com/)** - Security research and formal methods applications

## Academic Research

### Research Projects

- **[Ethereum Formal Verification Overview](https://github.com/leonardoalt/ethereum_formal_verification_overview)** - Comprehensive overview of formal verification in the Ethereum ecosystem
- **[EthBench](https://github.com/seresistvanandras/EthBench)** - Formal verification benchmark for Ethereum smart contracts
- **[Awesome Web3 Formal Verification](https://github.com/johnsonstephan/awesome-web3-formal-verification)** - Curated list of Web3 formal verification resources

### Academic Papers

- **[A Survey of Smart Contract Formal Verification](https://arxiv.org/abs/2008.02712)** - Comprehensive survey of formal verification techniques

## Vulnerability Detection

### Specific Vulnerability Research

- **[Reentrancy Verification](https://www.mdpi.com/2079-9292/12/10/2152)** - Reentrancy attack verification using Z3 SMT solver
- **[SmartScan](https://www.jatit.org/volumes/Vol103No3/4Vol103No3.pdf)** - Formal verification framework detecting 14 types of vulnerabilities

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
