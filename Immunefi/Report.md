Convert this comment into an issue for an audit report in Markdown. Provide sound reasoning such as to make a convincing case. Do not replicate or reference the comment, instead, generate a section in a code block as follows:  
  
```  
# Title in normal case stating the highest impact in simple terms  
  
## Brief/Intro  
Provide a very short and concise (one paragraph) statement on what the problem is, and what the consequences would be if the bug were exploited in production/mainnet.  
  
## Vulnerability Details  
Offer a detailed explanation of the vulnerability itself. Do not leave out any relevant information. Start by providing a summary of the functionalities in play, describing relevant components or functions and how they interact. Go from more general to more specific, until you get to the part of the logic where the root cause of the issue is located.  
  
Code snippets should be supplied whenever helpful. All mentions to function, variable and contract names should be formatted as `code snippets`. Functions must always be formatted with parentheses after their name, as in `functionName()`. Larger code blocks must be formatted using TWO backticks instead of three:  
  
``  
function someCode()  
``  
  
## Impact Details  
Summarize the impact of this finding. If it has multiple consequences, list them. If there is a higher impact with stated assumptions and a lesser one which applies no matter what, make that distinction. If there are funds at risk, provide a detailed breakdown of possible losses from an exploit.

## References  
Add any relevant links to documentation or code  
  
```  
  
Reply in a code block.