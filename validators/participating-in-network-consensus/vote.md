# Vote

Mix chain functionality can be changed by voting on the contracts implementations. New implementations can be deployed and opened to vote by validators for others to decide on whether to accept/reject the changes.

## Open a new ballot

To open a new vote, a validator needs to call the \`newBallot\` function on the [voting contract](https://miexs.com/address/0x81368e7C4f2968A1C773CC427d61f0Af3d912bb3) with the following params:

* startAfterNumberOfCycles - number of cycles (minimum 1) after which the ballot is open for voting
* cyclesDuration - number of cycles (minimum 2) for the ballot to remain open for voting
* contractType
  * 1 - Consensus
  * 2 - BlockReward
  * 3 - ProxyStorage
  * 4 - Voting
* proposedValue - address of the new implementation deployed for the relevant contract type
* description - text description which should contain the reason/change introduced in the ballot

![new ballot](<../../.gitbook/assets/image (25).png>)

## Check ballot info

Everyone can check all the ballots created using the \`getBallotInfo\` function. This function receives two params:

* id - the ballot id
* key - account address

![getBallotInfo](<../../.gitbook/assets/image (20).png>)

## Vote

Everyone can vote on open ballots after the start block has passed until the end block hasn't yet.

It's important to note that at the end of a vote, only validators count toward the final result.

Voting is done by calling the \`vote\` function, which receives two params:

* id - the ballot id
* choice - 1 is accept, 2 is reject

![vote](<../../.gitbook/assets/image (3).png>)

Some other useful functions of the [voting contract](https://miexs.com/address/0x81368e7C4f2968A1C773CC427d61f0Af3d912bb3) are:

## getQuorumState

Returns the state of a specific ballot id: 1 - in progress, 2 - accepted, 3 - rejected

## getAccepted/getRejected

Returns the number of accepts/rejects of a specific ballot id.

## activeBallots

Returns an array of active ballot ids.
