Convert this comment into an issue for an audit report in Markdown. Use @filename_or_url for context. Provide sound reasoning such as to make a convincing case. Do not replicate or reference the comment, instead, generate a section in a code block as follows:

```
# Title in normal case stating the highest impact in simple terms

Detailed description of this finding as inferred from the comment and the context. Start by providing a summary of the functionalities in play, describing relevant components or functions and how they interact. Go from more general to more specific, until you get to the part of the logic where the root cause of the issue is located. Then, clearly point out the issue and finally outline the scenario with the highest impact. If it has multiple consequences, list them. If there is a higher impact with stated assumptions and a lesser one which applies no matter what, make that distinction.

Include any links from the comment. If there are any quotes in the comment, integrate them into your description. All mentions to function, variable and contract names should be formatted as `code snippets`. Functions must always be formatted with parentheses after their name, as in `functionName()`. Larger code blocks must be formatted using TWO backticks instead of three:

``
function someCode()
``

## Proof of Concept
Illustrate the concept by ways of the simplest scenario leading to the highest impact. If possible, outline the scenario in a step-by-step, Alice and Bob type sequence of events. If there is only one actor, simply use "user" or "attacker". Provide references to relevant code in each of the steps.

## Recommended mitigation steps
Recommendation on how to fix or improve the code in question. Depending on the complexity of the issue, this could range from a detailed exploration of different solutions to a simple code fix. If it is just a simple code fix, provide the fix as a diff in a code block with two backticks.

```

Reply in a code block.