Convert the selected code comment(s)/code into a Codehawks vulnerability report using the Markdown structure below. The input comment describes a potential vulnerability found during a security review.

Focus on providing clear, concise, and accurate information based *only* on the provided context (selected code/comment and any `@` referenced files/symbols). Ensure the reasoning is sound and directly supports the finding.

Format the entire response as a single Markdown code block.

```markdown
## Title
*Provide a concise and descriptive title stating the core issue and its highest impact.*

## Summary
*Provide a brief (2-3 sentence) overview of the vulnerability. Describe the issue, the affected component(s), and the main consequence if exploited.*

## Vulnerability Details
*Offer a detailed explanation of the vulnerability.*
*   Start with necessary background on the relevant contracts, functions, and logic flow.
*   Clearly explain the root cause of the vulnerability.
*   Show how the vulnerability can be triggered, step-by-step if possible.
*   Include relevant code snippets using Markdown formatting (e.g., ` ``solidity ... `` `). Format inline code like `functionName()` or `variableName`.*

## Impact
*Describe the consequences of the vulnerability being exploited.*
*   Be specific about what an attacker could achieve (e.g., steal funds, cause denial of service, manipulate state, bypass checks).
*   If possible, quantify the potential impact (e.g., potential value locked at risk).
*   Distinguish between different levels of impact if applicable (e.g., guaranteed vs. conditional impact).

## Tools Used
*List the tools used to identify and analyze the finding. Always include "Manual Review". Add others if applicable (e.g., Slither, Foundry, Hardhat, VS Code Extensions).*
*   Manual Review

## Recommendations
*Provide clear, actionable steps to fix the vulnerability.*
*   Suggest specific code changes or logical adjustments.
*   Explain how the recommendation resolves the identified issue.
*   If multiple solutions exist, briefly discuss trade-offs if relevant.
```
