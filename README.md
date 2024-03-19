## Module Overview

This repository implements a simple `dao` module aimed at creating a decentralized autonomous organization (DAO) for managing shared funds, community tasks, proposals, and voting functionalities.

### `dao` Token
**`dao` Token**
The `dao` utilizes a community token called `dao` for governing the community and incentivizing participation. Community members need to use `dao` tokens to create proposals, participate in voting, and engage in community governance. The total supply of `dao` tokens is fixed when the `dao` is established, and initially, all `dao` tokens will be locked in the treasury.
**How to Obtain `dao` Tokens?**
The `dao` organization will publish community tasks with corresponding `dao` token rewards. Completing these tasks earns participants credentials that can be redeemed for `dao` tokens. Additionally, proposals submitted by community members may receive `dao` token rewards upon acceptance, depending on the proposal's level.

### Member Roles
**There are three types of member roles in the community:**

#### 1. InitCoreMember
Initial core members of the `dao` organization.
Authorized Roles: InitCoreMember, CoreMember.

#### 2. CoreMember
Core members of the `dao` organization:
Authorized Roles: Member.
Rights:
1. Publish community tasks.
2. Distribute task rewards.
3. Authorize regular community members.
4. Close proposals.
5. Modify proposal levels.

#### 3. Member
Regular members of the `dao` organization (need to hold `dao` tokens and apply for authorization from CoreMembers).
Rights:
1. Submit proposals.
2. Claim proposal rewards.
3. Participate in voting.

### How to Run
1. Initial members of the DAO publish community tasks.
2. By participating in community tasks and holding `dao` tokens, one can apply to join the DAO organization.
3. After joining the DAO organization, members can submit community proposals. If accepted, they can receive certain token rewards and participate in proposal voting.

## Object

### `Dao`

Contains information about the DAO, such as the number of members and the total supply.

### `Treasury`

The treasury of the DAO, used to store funds.

### `Proposal`

Represents a proposal, including its title, description, initiator, and voting status.

### `VoteCap`

Records voting information, including the voter, number of votes, and whether they support the proposal.

### `CommunityTask`

A community task describing a task that needs to be completed and the corresponding reward.

### `TaskRewardCap`

Records task rewards, including the reward amount and recipient.

### `InitCoreCap`

Authorization credential for initial core members.

### `CoreCap`

Authorization credential for core members.

### `MemberCap`

Authorization credential for members.
