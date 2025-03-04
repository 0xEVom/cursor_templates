Convert this comment into an issue for an audit report in Markdown. Use @filename_or_url for context. Provide sound reasoning such as to make a convincing case. Do not replicate or reference the comment, instead, generate a section in a code block as follows:  
  
```  
# Title should use normal case and just mention high-level impact and name primary components  
  
## Description  
Detailed description of this finding as inferred from the comment and the context. Walk through the part of the logic where the root cause of the issue is located, clearly point out the root cause and finally outline the scenario with the highest impact. Do not omit any information provided in the comment.

Include any links from the comment. If there are any quotes in the comment, integrate them into your description. All mentions to function, variable and contract names should be formatted as `code snippets`. Functions must always be formatted with parentheses after their name, as in `functionName()`. Code blocks must be formatted using TWO backticks instead of 3, as in:

``
some function() {
}
``

However, do not include any code blocks from the existing code in your output as those will be linked to the report on submission.

## Proof of Concept  
Illustrate the concept by ways of the simplest scenario leading to the highest impact. If possible, outline the scenario in a step-by-step, Alice and Bob type sequence of events. If there is only one actor, simply use "user" or "attacker". Provide references to relevant code in each of the steps.  
  
## Recommendation  
Recommendation on how to fix or improve the code in question. Depending on the complexity of the issue, this could range from a detailed exploration of different solutions to a simple code fix. If it is just a simple code fix, provide the fix as a diff in a code block with two backticks.  
  
```