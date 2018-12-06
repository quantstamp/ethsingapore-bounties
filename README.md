# Submission instructions

Please send all materials to `@yoheioka` on Telegram.

# Quantstamp Prize for ETH Singapore Bounty

## Project description

Improve the usability of the Quantstamp protocol for smart contract analysis. The project is broken into three sub-projects. A team can choose to work on any (one or more) of these.

### Improving presentation of the audit reports ($1000)
The Quantstamp protocol reports are JSON files that contain information about the analyzed contract and outputs of security analyzers such as Mythril and Oyente (other analyzers will be added in the future). The raw JSON reports are hard to interpret by non-technical audience. Furthermore, the reports can contain duplicate vulnerabilities as they are detected by multiple analyzers. A successful developer of this bounty would improve the presentation of the Quantstamp protocol reports and/or make progress towards removing the vulnerability duplicates.

#### Resources
1. Betanet UI: https://betanet.quantstamp.com/start 
1. Sample Report: https://s3.amazonaws.com/qsp-protocol-reports-dev/d614a6ae-aac6-480e-af3c-eb59dae1f046.json
1. JSON description of the analyzer report: https://s3.amazonaws.com/qsp-protocol-schema/qsp-v1-report.json
1. Sample audit contract (works when submitted to QSP network): https://s3.amazonaws.com/qsp-protocol-test-contracts/abc7d7d2eff-86cb-4167-8a62-4b99a87b7f50.sol
1. Sample output of analyzers on various smart contracts:
https://consensys.net/diligence/evm-analyzer-benchmark-suite/ 

### Enabling decentralized exchange methods ($1000)
The Quantstamp protocol is powered by the QSP token. As the users might not have QSP tokens handy, the protocol could benefit from an interface that allows users to pay with any ERC20 token that will be automatically converted to QSP for the purposes of requesting the audit. The Kyber decentralized exchange provides means for doing so. There may also be other solutions. A successful developer of this bounty would extend the Quantstamp protocol smart contract with such functionality.

#### Resources
1. Kyber network documentation: https://developer.kyber.network/docs/ArchitectureOverview/
https://github.com/KyberNetwork/smart-contracts/blob/master/integration.md
1. QSP protocol smart contract: 
https://etherscan.io/address/0x74814602062af64fd7a83155645ddb265598220e#code
1. Protocol steps instructions: https://s3.amazonaws.com/qsp-protocol-schema/betanet-instructions.pdf 

### Improving betanet web UI ($1000)
Security audits from the Quantstamp protocol can be requested via the web UI provided on betanet.quantstamp.com or via direct interaction with the smart contracts. The current web UI has many limitations and can be improved significantly. For example, a user cannot check the status or results of past audits, a user has to `approve` QSP (minimum 1000) even if he or she has done so in the past and has not spent it, and a user cannot refresh the page at any point during the process even though it may seem like the site is hanging. A successful developer of this bounty will build a more user friendly and resilient web UI that resolves the aforementioned issues.

#### Resources
1. https://betanet.quantstamp.com/start
1. Protocol instructions: https://s3.amazonaws.com/qsp-protocol-schema/betanet-instructions.pdf
1. Protocol smart contract source code
https://etherscan.io/address/0x74814602062af64fd7a83155645ddb265598220e#code
1. Quantstamp's Canonical UI-Library https://github.com/quantstamp/qs-ui-lib

### Interfaces for QSP protocol ($1000)
Security audits from the Quantstamp protocol can be requested via web UI provided on betanet.quantstamp.com or via direct interaction with the smart contracts. To simplify the usage and encourage the practice of analyzing smart contracts for security vulnerabilities, the Quantstamp protocol could be integrated directly into the development tools such as Github CI, Truffle, Embark, Remix IDE, and others. A successful developer of this bounty will develop plugins that will enable developers to trigger a security audit directly from such dev tools.

#### Resources
1. Protocol instructions: https://s3.amazonaws.com/qsp-protocol-schema/betanet-instructions.pdf
1. Protocol smart contract source code
https://etherscan.io/address/0x74814602062af64fd7a83155645ddb265598220e#code
1. Truffle: https://truffleframework.com/
1. Remix: https://github.com/ethereum/remix-ide
1. Embark: https://embark.status.im/ 

## Requirements
1. A link to the open-source code must be provided, including instructions how to install dependencies, build, and run
1. A short presentation file must describe your project
1. The contract address(es) of your deployed demo must be provided, either on a testnet of your choice (Kovan, Rinkeby or Ropsten) or on Ethereum mainnet; instructions on how to interact with the contract(s) are appreciated

## Judging Criteria
1. Technicality
1. Originality
1. Practicality
1. WOW Factor
