# VFF Platform (Vote For Fact) Proposal

## 1. Executive Summary

VFF (Vote For Fact) is a decentralized fact-checking platform built on the Kaia blockchain. It aims to combat misinformation by leveraging collective intelligence, blockchain technology, and economic incentives. The platform introduces a unique dual-token system and a reputation-based voting mechanism to ensure accurate and reliable fact-checking.

## Table of Contents

1. [Executive Summary](#1-executive-summary)
2. [Product Overview](#2-product-overview)
3. [Detailed Product Flow](#3-detailed-product-flow)
- 3.1. [Content Discovery and Submission](#31-content-discovery-and-submission)
- 3.2. [Voting Process](#32-voting-process)
- 3.3. [Verification Process](#33-verification-process)
- 3.4. [Result Determination and Reward Distribution](#34-result-determination-and-reward-distribution)
- 3.5. [Reputation System](#35-reputation-system)
- 3.6. [Oracle Integration](#36-oracle-integration)
- 3.7. [Community Contribution](#37-community-contribution)
4. [Economic Model](#4-economic-model)
- 4.1. [Dual-Token System](#41-dual-token-system)
- - 4.1.1. [TruthCoin (TC)](#411-truthcoin-tc)
- - 4.1.2. [VerifyPoint (VP)](#412-verifypoint-vp)
- 4.2. [Token Interaction](#42-token-interaction)
- 4.3. [Economic Sustainability](#43-economic-sustainability)
- 4.4. [Incentive Alignment](#44-incentive-alignment)
5. [Use Cases](#5-use-cases)
- 5.1. [Individual User: Maria, Student](#51-individual-user-maria-student)
- 5.2. [News Organization: TruthSeeker News](#52-news-organization-truthseeker-news)



## 2. Product Overview

VFF consists of the following key components:

1. **Decentralized Fact-Checking System**: Allows users to submit and verify news articles or claims.
2. **Dual-Token Economy**: Utilizes TruthCoin (TC) and VerifyPoint (VP) for different platform activities.
3. **Reputation System**: Tracks user reliability and influences voting power.
4. **Educational Module**: Improves media literacy among users.
5. **Community Governance**: Enables token holders to participate in platform decisions.

```mermaid
graph TD
    A[User finds controversial content] -->|Uses VFF| B[Content submitted to VFF]
    B --> C[Set verification conditions]
    C --> D[Users vote and stake tokens]
    D --> E[AI-assisted verification]
    E --> F{Clear consensus?}
    F -->|Yes| G[Final verdict determined]
    F -->|No| H[Expert review]
    H --> G
    G --> I[Reward distribution]
    I --> J[Update user reputations]
    J --> K[Post result to social media]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style G fill:#bbf,stroke:#333,stroke-width:2px
    style K fill:#bfb,stroke:#333,stroke-width:2px
    style I fill:#90EE90,stroke:#333,stroke-width:2px

```


## 3. Detailed Product Flow

### 3.1 Content Discovery and Submission

1. **Browser Extension and Mobile App**:
   - Users install the VFF browser extension or mobile app.
   - These tools integrate with major social media platforms (SNS) like Facebook, X, Thread, Instagram, etc.

2. **Content Flagging**:
   - When a user encounters a controversial news article or claim on SNS, they can easily flag it using the VFF extension/app.
   - The user sets verification conditions (e.g., time limit, minimum number of votes) or opts for decentralized verification.

3. **Content Submission to VFF Platform**:
   - Flagged content is automatically submitted to the VFF platform.
   - A smart contract is created to manage the verification process based on the set conditions.

4. **SNS Interaction**:
   - Upon submission, a VFF bot posts a comment on the original SNS post.
   - The comment informs others that a fact-check has been initiated and invites them to participate on the VFF platform.

### 3.2 Voting Process

1. **Voter Participation**:
   - Users can access the voting page through the SNS bot comment or directly on the VFF platform.

2. **Staking Mechanism**:
   - To vote, users must stake 10 VFF tokens (fixed price per vote).
   - A token locking mechanism prevents users from transferring or selling staked tokens during the voting period.

3. **Voting Options**:
   - Users can vote "True," "False," or "Need Expert Review."

4. **Time-Weighted Voting**:
   - Early voters may receive higher rewards, incentivizing quick responses to misinformation.

### 3.3 Verification Process

1. **AI-Assisted Verification**:
   - An open-source AI model, running on Kaia's service chain, processes the content and votes.
   - The AI considers factors like vote distribution, user reputations, and content analysis.

2. **Expert Review** (if necessary):
   - For complex or contentious cases, or if "Need Expert Review" receives significant votes, human experts are engaged.
   - Experts are randomly selected based on their credentials and reputation.

3. **Verification Completion**:
   - The verification process concludes when preset conditions are met (e.g., time limit reached, sufficient votes collected).

### 3.4 Result Determination and Reward Distribution

1. **Final Verdict**:
   - The system combines AI analysis, community votes, and expert opinions (if applicable) to reach a final verdict.

2. **Smart Contract Execution**:
   - A Kaia-based smart contract automatically processes the results.

3. **Reward Distribution**:
   - Correct voters receive their staked tokens back plus a share of the reward pool.
   - Incorrect voters forfeit their staked tokens, which are added to the reward pool.

4. **Dynamic Reward Pool**:
   - The reward amount is adjusted based on factors like participation level and verification difficulty.

### 3.5 Reputation System

1. **Reputation Scoring**:
   - Users earn reputation points based on their voting accuracy and participation frequency.

2. **Reputation Benefits**:
   - Higher reputation users may receive additional rewards or have more weight in future votes.

### 3.6 Oracle Integration

1. **Cross-Platform Data Flow**:
   - Kaia's Oracle services facilitate secure data exchange between SNS platforms and the VFF system.

2. **Real-time Updates**:
   - Verification results are posted back to the original SNS content, providing real-time fact-checking information to the wider audience.

### 3.7 Community Contribution

1. **AI Model Improvement**:
   - The community can contribute to improving the open-source AI verification models.

2. **Governance Participation**:
   - Token holders can propose and vote on system improvements and parameter adjustments.

This detailed flow encompasses the entire process from content discovery on social media to the final reward distribution, incorporating both the initial concept and the technical implementation suggestions. It leverages Kaia blockchain's features like smart contracts, oracles, and service chains to create a robust, transparent, and efficient fact-checking ecosystem.


## 4. Economic Model

### 4.1 Dual-Token System

## 4.1.1 TruthCoin (TC)

- **Purpose**: Governance, high-stakes voting, value storage
- **Total Supply**: 1,000,000,000 TC
- **Distribution**:
    - 40% Public Sale
    - 25% Team and Advisors (4-year vesting)
    - 20% Community Rewards
    - 10% Foundation Reserve
    - 5% Early Investors (1-year lock-up)
- **Utility**:
    - Governance voting
    - High-stakes fact-checking
    - Staking for passive income
    - Accessing premium features

## 4.1.2 VerifyPoint (VP)

- **Purpose**: Daily platform activities, learning rewards
- **Supply**: Dynamic, algorithmically adjusted
- **Utility**:
    - Low-stakes fact-checking
    - Earning from educational activities
    - Micro-tasks and content submission

### 4.2 Token Interaction

- TC can be converted to VP at any time (dynamic rate)
- VP to TC conversion is restricted (minimum reputation required, conversion limits)

```mermaid
graph TD
    A[User Activity] --> B{Activity Type}
    B -->|Voting| C[Stake TC]
    B -->|Content Submission| D[Earn VP]
    B -->|Educational Tasks| E[Earn VP]

    C --> F{Voting Outcome}
    F -->|Correct| G[Return TC + Bonus]
    F -->|Incorrect| H[Lose Staked TC]

    G --> I[Option to Convert]
    D --> I
    E --> I

    I -->|Convert| J[VP to TC Conversion]
    I -->|Hold| K[Keep as VP]

    H --> L[TC Added to Reward Pool]
    G --> L

    M[Platform Fees] --> L
    
    L --> N[Distribute Rewards]
    N --> O[To Correct Voters]
    N --> P[To Content Submitters]
    N --> Q[To Verifiers/Experts]

    R[TC Staking for Governance] --> S[Earn Passive Income]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style C fill:#FFA07A,stroke:#333,stroke-width:2px
    style D fill:#90EE90,stroke:#333,stroke-width:2px
    style E fill:#90EE90,stroke:#333,stroke-width:2px
    style L fill:#FFD700,stroke:#333,stroke-width:2px
    style R fill:#FFA07A,stroke:#333,stroke-width:2px
```

### 4.3 Economic Sustainability

- TC has a 2% annual inflation rate for the first 5 years
- VP supply is dynamically adjusted based on platform activity
- Transaction fees and incorrect vote penalties are used for token burns and reward pools

### 4.4 Incentive Alignment

- Staking mechanism ensures users have skin in the game
- Reputation system rewards consistent, accurate participation
- Long-term TC holding is incentivized through governance rights and fee sharing

## 5. Use Cases

### 5.1 Individual User: Maria, Student

Maria is a college student interested in current events but often unsure about the reliability of news she reads online.

1. Maria signs up for VFF and completes the onboarding process, receiving a small amount of VP.
2. She takes several media literacy courses on VFF, earning more VP and increasing her reputation.
3. Maria starts participating in low-stakes fact-checking using her VP.
4. As her accuracy and reputation grow, she earns more VP and converts some to TC.
5. With her TC, Maria now participates in high-stakes fact-checking of major news stories.
6. She also uses her TC to vote on platform governance issues, feeling more engaged with the community.

Outcome: Maria becomes a more discerning news consumer, earns crypto while learning, and actively contributes to combating misinformation.

### 5.2 News Organization: TruthSeeker News

TruthSeeker News is a digital news outlet looking to increase reader trust and engagement.

1. TruthSeeker integrates VFF's API into their website.
2. They submit all their published articles to VFF for community fact-checking.
3. Articles display a VFF verification badge, showing real-time community trust scores.
4. TruthSeeker encourages readers to participate in VFF verification, increasing engagement.
5. They use VFF analytics to identify trending topics and potential misinformation in their industry.
6. TruthSeeker's reputation for accuracy grows, attracting more readers and advertisers.

Outcome: TruthSeeker News enhances its credibility, engages readers in the fact-checking process, and gains valuable insights into news trends and reader concerns.

These use cases demonstrate how VFF can benefit both individual users and organizations, creating a more informed and engaged community while combating the spread of misinformation.
