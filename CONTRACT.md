# Digital Zimbabwe Gold (dZWG) Smart Contract

## Overview

This document provides a simplified illustrative excerpt of the Digital Zimbabwe Gold (dZWG) smart contract.

dZWG is a Zimbabwe Gold (ZWG; ISO code: ZWG)-pegged digital currency designed as a reserve-backed, blockchain-native settlement layer.

This document is not a full technical specification. It presents a minimal contract interface for conceptual understanding only.

The production implementation of dZWG is significantly more advanced and is maintained separately under controlled development, audit, and governance processes.

---

## Contract Snippet (Illustrative Only)

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

/// @title Digital Zimbabwe Gold (dZWG) - ZWG-pegged digital settlement token
/// @author Simon Kapenda
/// @notice Simplified contract for demonstration purposes only
contract dZWG is ERC20, Ownable {
    constructor() ERC20("Digital Zimbabwe Gold", "dZWG") Ownable(msg.sender) {}

    /// @notice Mint dZWG tokens
    /// @dev Restricted to contract owner in this simplified version
    function mint(address to, uint256 amount) external onlyOwner {
        _mint(to, amount);
    }

    /// @notice Burn dZWG tokens
    /// @dev Restricted to contract owner in this simplified version
    function burn(address from, uint256 amount) external onlyOwner {
        _burn(from, amount);
    }
}
```

---

## Scope and Limitations

This document intentionally omits the full architecture of the production dZWG system.

The production contract includes, but is not limited to:

- upgradeable proxy architecture (UUPS or equivalent)
- role-based access control (granular permissions beyond single owner)
- multisignature governance for administrative actions
- timelock-controlled upgrades and parameter changes
- reserve-linked issuance and redemption controls
- compliance framework (KYC/AML enforcement layers)
- sanctions screening, blacklist, and account freeze mechanisms
- treasury and fee management modules
- oracle integration (if applicable)
- audit-grade event emission and monitoring hooks

---

## Positioning

The dZWG smart contract is not designed as a speculative token contract.

It is part of a broader financial infrastructure stack, where the smart contract functions strictly as the on-chain representation of a ZWG-denominated settlement instrument.

Accordingly, this simplified contract should not be interpreted as the full implementation of the system.

---

## Important Notice

This code is provided strictly for demonstration and educational purposes.

It is not production-ready and must not be used in live environments.

All production deployments of dZWG are subject to formal audit, governance controls, and operational safeguards.
