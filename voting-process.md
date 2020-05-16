# Voting process

When a proposal is submitted to the consortium, the members of the consortium must *vote* before the proposal passes. All members of the consortium must be notified of the proposal for it to be a **valid proposal**. Invalid proposal can still be discussed on, but cannot be approved officially. Each member picks one of the four possible options:

- `y`: means "Yes", agrees to the proposal and wants to see it taken into effect
- `w`: means "Whatever", does not have an opinion about the proposal and does not want their voice to be counted
- `?`: means "Question", when the member needs clarification about the proposal before voting on it
- `!`: means "Alternative suggestion", when the member has a counter-proposal to the current proposal

As soon as there is any `!` vote, the current proposal is put on hold, and the counter-proposal in the `!` vote should be listened to, and voted on like any other proposal. All proposals have the same voting process, so that it's possible to have a chain of `!`, and along this chain, the original proposal is refined until everyone is satisfied. Or, a discussion takes place until there is no resolution (none of the proposals along the chain pass), indicating an impasse. If there are multiple `!` votes for the same decision, the first `!` counter-proposal should be listened to and the other counter-proposals are disregarded, but can be resubmitted as `!` on the subsequent proposal.

Votes of type `?` don't cancel the current proposal, they just ask for clarification from the member who proposed it. After the clarification is given, **all** members vote again for the same proposal.

The proposal **passes** if and only if all members have voted **within the deadline** AND there are **at least one `y` vote**, zero `?` votes, zero `!` votes, and any number of `w` votes. Deadlines are explained below.

## Deadlines

The default deadline for all proposals is 21 days (exactly `21 * 24 hours`), after that, members that have not given a vote are considered to **have given the `w` vote**. In this way, no proposal would have absentees.
