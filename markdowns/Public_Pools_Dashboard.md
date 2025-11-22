Public Pools Dashboard | RISEWiki

[![Logo](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2F1762761122-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Forganizations%252FVpfHHIHQI6ROs7kspCfa%252Fsites%252Fsite_dzbNR%252Flogo%252F90i8Iwb0LXw9xIroe9wy%252FInfinity%2520Rising_logo2.png%3Falt%3Dmedia%26token%3Dde7ab13b-7593-4583-83e6-7ed79d87ed26&width=260&dpr=4&quality=100&sign=8e852af&sv=2)![Logo](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2F1762761122-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Forganizations%252FVpfHHIHQI6ROs7kspCfa%252Fsites%252Fsite_dzbNR%252Flogo%252FbwYsgKrrCmFJzlM7KKwZ%252FInfinity%2520Rising_logo2.png%3Falt%3Dmedia%26token%3Dc62ee205-acdf-47b2-9313-ca755597bd96&width=260&dpr=4&quality=100&sign=c99ea5b2&sv=2)](/)

`Ctrl``k`

* [📋INFINITY RISING](/)
* 🎮GAMEPLAY

  + [About the game](/gameplay/about-the-game)
  + [Gameplay - PC](/gameplay/gameplay-pc)
  + [Themed Zones](/gameplay/themed-zones)
  + [Mega Dome - Calido Valley](/gameplay/mega-dome-calido-valley)
  + [Gameplay - eSports Racing League](/gameplay/gameplay-esports-racing-league)
  + [Game Launcher](/gameplay/game-launcher)
  + [Community](/gameplay/community)
* 🌐ON CHAIN

  + [Blockchain Wallets](/on-chain/blockchain-wallets)
  + [COPI Stake Pool](/on-chain/copi-stake-pool)
  + [COPIC Stake Pool](/on-chain/copic-stake-pool)
  + [Marketplace](/on-chain/marketplace)
  + [Player Owned Assets](/on-chain/player-owned-assets)
* 🧑‍🤝‍🧑THE COMPANY

  + [COMPLIANCE](/the-company/compliance)
  + [Governance](/the-company/governance)
  + [Partners](/the-company/partners)
  + [Technology](/the-company/technology)
  + [Visions and Values](/the-company/visions-and-values)
* 📖Documentation

  + [Game](/documentation/game)
  + [Nodes](/documentation/nodes)

    - [Guide: How to Set Up a File Node Pool](/documentation/nodes/guide-how-to-set-up-a-file-node-pool)
    - [Public Pools Dashboard](/documentation/nodes/public-pools-dashboard)
    - [Node Delegation](/documentation/nodes/node-delegation)
* 🔗LINKS

  + [Official Website](https://www.infinityrising.com/)

[Powered by GitBook](https://www.gitbook.com/?utm_source=content&utm_medium=trademark&utm_campaign=PQmCVki2WHg9QcW9pdrX)

On this page

* [Public Pools Dashboard](#public-pools-dashboard)
* [Configuring a Public Pool](#configuring-a-public-pool)
* [Understanding the Public Pools Dashboard](#understanding-the-public-pools-dashboard)
* [Understanding the Public Pool Detail](#understanding-the-public-pool-detail)

Copy

1. [📖Documentation](/documentation)
2. [Nodes](/documentation/nodes)

Public Pools Dashboard
======================

Overview and descriptions of the information represented in the public pools dashboard.

Scruffy breaks down the public pools dashboard

Public Pools Dashboard
----------------------

The public pools dashboard can be found at this URL:

<https://cornucopias.io/nodes/pools>

The public pools dashboard will be the focal point for delegation. Today, the dashboard will simply show performance information, but in the future, it will be the best location to decide where to delegate file nodes. The landing page is a listing of public pool servers that are willing to receive delegations. The list by default is sorted by how strong the pool is performing.

### Configuring a Public Pool

Once a pool server has been created, configured and validated, the pool needs a few additional steps to be listed on the public dashboard:

1. Edit the pool and change the pool type to public.
2. Ensure that at least 8 nodes have been delegated to the pool.

At this point, the pool will be listed on the public dashboard. If the pool is not listed, it may be because a full reward cycle must pass before the changes create performance data for the dashboard. Please allow for 24-48 hours for the public dashboard to update with the new pool information.

Updating the pool with a new picture and description may help to attract more delegations by making the pool's mission or purpose clearer. The pool picture must be appropriate for all ages. The Cornucopias team has final say on what is appropriate and not appropriate. If a pool picture or description is found to be inappropriate, it will be removed from the public dashboard without warning.

### Understanding the Public Pools Dashboard

#### **Columns**

* **Picture**: A picture that represents the pool.
* **Name**: The name of the pool. This might be a concise description. This field is globally unique.
* **Ticker**: This is a 3-5 character code that represents the pool. It should be unique and is often used as a shorthand for the pool's name. It is globally unique.
* **Region**: The geographical location that the pool server is closest to. This is measured by network latency and is not necessarily the physical location of the server. The regions are:

  + North America
  + Europe
  + Asia Pacific
  + South America
* **15 Day**: The total number of bytes served in the last 15 days.
* **Last Cycle**: The total number of bytes served in the last reward cycle.
* **Saturation**: Represents the availability of the pool for more delegations.

  + If the pool owner has delegated 8 of their own nodes to the pool, the pool can hold 40 delegations including your own.
  + If the pool owner has delegated 9 of their own nodes to the pool, the pool can hold 45 delegations including your own.
  + If the pool owner has delegated 10 of their own nodes to the pool, the pool can hold 50 delegations including your own.
  + If the pool is full, it will show "FULL" in this column.
* **Active Cycles** - The number of consecutive days that the pool server has been active. If a pool is down for a complete reward cycle (24 hours), it will reset this number to zero.
* **Age** - The age of the pool since it was created. This is calculated from the creation date of the pool server.
* **Strength** - The strength of the pool is determined by a simple algorithm that helps the fastest and most reliable pool servers to be ranked at the top. This value is ranked and distributed evenly between 5 buckets. This distribution includes private pools, so the even distribution may not be visible on the public dashboard. A sixth bucket is reserved for the pools that are not functioning. These will appear to have 0 bars.

  + **Formula**: `Strength = (Byte Rate) * (Success Rate) * (Percentage of Cycles with at least one registration)`
  + **Byte Rate**: The average bytes per second over the last 15 days.
  + **Success Rate**: The percentage of successful requests over the last 15 days.
  + **Percentage of Cycles with at least one registration**: The percentage of reward cycles in the last 15 days where the pool had at least one registration.

#### **Sorting**

The pool dashboard table can be sorted by name, ticker, and strength.

#### **Filtering**

The pool dashboard table can be filtered by region, availability, and strength.

### Understanding the Public Pool Detail

The public pool detail page provides more in-depth information about a specific pool. It includes description, graphs and delegations.

#### Description

The description section provides a more detailed overview of the pool's purpose, mission, and any other relevant information that the pool owner wants to share. This is an opportunity for the pool owner to explain why someone should delegate to their pool. It can include links to social media, websites, or other resources.

#### Graphs

Check-In Counts

The pool server will check in several times a day. This is how the availability of a pool server is determined. The most reliable pools will have consistent check-in counts, indicating that they are online and serving requests. The graph shows the number of successful check-ins over the last 15 days.

Request Success Rate

A successful request is a successful download of a chunk from a pool server to a launcher client. Failed requests occur if there's a server or network issue. The success rate is the percentage of successful requests in the last 15 days, shown in a graph to track reliability trends.

Delegations Count

The node's state is constantly evolving, and the delegation can change daily. The delegation count graph displays the number of delegations per day over the past 15 days, providing insights into the pool's popularity.

Speed

The average bytes per second over the last 15 days. This is the foundational metric for the pool strength. Fast pools really help the network to be responsive and efficient.

#### Delegators

A list of all of the nodes that are currently delegated to the pool.

[PreviousPublic Pools](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/public-pools)[NextNode Delegation](/documentation/nodes/node-delegation)

Last updated 5 months ago

This site uses cookies to deliver its service and to analyze traffic. By browsing this site, you accept the [privacy policy](https://infinityrising.com/legal/privacy-policy).

AcceptReject