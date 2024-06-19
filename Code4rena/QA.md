Convert this comment into an issue for an audit report in Markdown. The finding can be short as this is just a low severity issue, do not add any additional headings. Do not replicate or reference the comment, instead, generate a section in a code block as follows:  
  
```  
### [L-01] Title in normal case mentioning high-level impact and naming primary components  

Start with a clear and accurate description of the issue as inferred from the comment and the context, including where appropriate: reasoning, context, relevant code and impact.

References to variable names or similar should be formatted as `code snippets`. Functions must always be formatted with parentheses after their name, as in `functionName()`.

Then, provide a recommendation on how to fix or improve the code in question if necessary.
```

Reply in a code block.