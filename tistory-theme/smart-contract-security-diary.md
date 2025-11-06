# Smart Contract Security Diary: [Vulnerability Name]

**Date:** 2025-01-XX  
**Severity:** 🔴 Critical / 🟠 High / 🟡 Medium / 🟢 Low  
**CWE:** [CWE-XXX](https://cwe.mitre.org/data/definitions/XXX.html)  
**Chain:** Ethereum / BSC / Polygon / Arbitrum / etc.

---

## 📋 Overview

### Project Information
- **Project Name:** [Project Name]
- **Contract Address:** `0x...`
- **Audit Date:** 2025-01-XX
- **Auditor:** Bakaliee Security

### Vulnerability Summary
Brief description of the vulnerability discovered. Explain what the issue is in 2-3 sentences.

---

## 🔍 Findings

### CWE Classification
- **CWE-XXX:** [CWE Name]
- **Category:** [e.g., Reentrancy, Access Control, Integer Overflow]

### Context
Detailed explanation of where and how the vulnerability exists in the codebase.

### Severity Assessment
**Impact:** High / Medium / Low  
**Likelihood:** High / Medium / Low  
**Overall Severity:** Critical / High / Medium / Low

**Justification:**
Explain why this severity rating was assigned based on potential impact and exploitability.

---

## 🧪 Reproduction Steps

### Environment Setup

\`\`\`bash
# Clone the repository
git clone https://github.com/project/repo.git
cd repo

# Install dependencies
npm install

# Install Foundry (if needed)
curl -L https://foundry.paradigm.xyz | bash
foundryup
\`\`\`

### Vulnerable Contract

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract VulnerableContract {
    mapping(address => uint256) public balances;
    
    // Vulnerable function
    function vulnerableFunction() public {
        // Vulnerable code here
    }
}
