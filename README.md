# ZKX challenges for the StarkNet Hackathon - Autumn 2022

v.0.1

## [HARD] Challenge:  Write a Cairo smart contract for the creation of working groups 

### Working Group
Each working group is led by a Coordinator (one or more users), who is/are responsible for organising the collective group and final decision-making.
A Coordinator can be a working group with its own voting power and Treasury.
A Coordinator can coordinate other Working Groups at the same hierarchy level and other subsidiaries with the same parents.
Each Working Group can have subsidiaries as a sub-DAO with underlying Working Group(s). From the structural and organisational standpoint, it’s a tree with unlimited depth.
Every DAO has a first Working Group for the governance of the DAO itself, called a Coordinator. The setup of the First Working Group is a part of the initial Setup.
Working Groups initiated at the same level as the Originating Working Group are proposed by its Coordinator.
Working Group Coordinator is in charge of the relevant Treasury attributed to the Working Group.
Treasury can be either shared with other Working Groups that are linked to the same parent (are located in the same level) and also to its subsidiaries.

### Create Proposal
A proposal can have a part (volume, percentage) of the parenting treasury to assign funds for the Proposal to be executed.
Assigned funds can be released using different scenarios (execution on approval, time-locked, staged releases)
A proposal can include the assignment of the user(s) to the Committee – in this scenario assigned user (if the Proposal is approved) is elected as part of the Committee
Proposal approval/decline strategy (one vote – one token, quadruple voting, grouped voting, transfer of rights);

### The committee fundamentals and configuration
Approval rules: A proposal needs to be approved by an X number of members (where X can be defined as a static value or a percentage of registered or staking users). X is configurable at the time when a new entity is configured and deployed.
Veto rules: A Committee has a right to veto an approved Proposal within X seconds (where X is defined at the initiation/configuration stage and has a default value of 86400) if the Proposal has a veto actioned by Y members of the Committee (where Y can be defined as a static value or a percentage of committee members)
The committee member can have funding paid from the Treasury in the amount of X every Y seconds (where X is defined as a number of tokens, Y as a number of seconds)
