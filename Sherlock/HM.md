Convert this comment into an issue for an audit report in Markdown. Use @filename_or_url for context. Provide sound reasoning such as to make a convincing case. Do not replicate or reference the comment, instead, generate a section in a code block as follows:

```
# {actor} will {impact} {affected party}

## Summary

A summary with the following structure: **{root cause} will cause [a/an] {impact} for {affected party} as {actor} will {attack path}**

## Root Cause

In case it’s a mistake in the code: **In {link to code} the {root cause}**

_Example:_ _- In `stake.sol:551` there is a missing check on transfer function_ _- In `lp.sol:12` the fee calculation does division before multiplication which will revert the transaction on `lp.sol:18`_

In case it’s a conceptual mistake: **The choice to {design choice} is a mistake as {root cause}**

_Example:_ _- The choice to use Uniswap as an oracle is a mistake as the price can be manipulated_ _- The choice to depend on Protocol X for admin calls is a mistake as it will cause any call to revert_

## Internal Pre-conditions

A numbered list of conditions to allow the attack path or vulnerability path to happen:

1. [{Role} needs to {action} to set] {variable} to be [at least / at most / exactly / other than] {value}
2. [{Role} needs to {action} to set] {variable} to go from {value} to {value} [within {time}]

_Example:_ _- Admin needs to call `setFee()` to set `fee` to be exactly `1 ETH`_ _- Number of ETH in the `stake.sol` contract to be at least `500 ETH`_

## External Pre-conditions

> Similar to internal pre-conditions but it describes changes in the external protocols

_Example:_ _- ETH oracle needs to go from `4000` to `5000` within 2 minutes_ _- Gas price needs to be exactly `100 wei`_

## Attack Path

A numbered list of steps, talking through the attack path:

1. **{Role} calls {function} {extra context}**
2. ..

## Impact

In case it's an attack path: **The {affected party} suffers an approximate loss of {value}. [The attacker gains {gain} or loses {loss}].**

_Example:_ _- The stakers suffer a 50% loss during staking. The attacker gains this 50% from stakers._ _- The protocol suffers a `0.0006` ETH minting fee. The attacker loses their portion of the fee and doesn't gain anything (griefing)._

In case it's a vulnerability path: **The {affected party} [suffers an approximate loss of {value} OR cannot {execute action}].**

_Example:_ _- The users suffer an approximate loss of 0.01% due to precision loss._ _- The user cannot mint tokens._

## PoC

Illustrate the concept by ways of the simplest scenario leading to the highest impact. If possible, outline the scenario in a step-by-step, Alice and Bob type sequence of events. If there is only one actor, simply use "user" or "attacker". Provide references to relevant code in each of the steps.

## Mitigation

Recommendation on how to mitigate the issue.
```

Reply in a code block.