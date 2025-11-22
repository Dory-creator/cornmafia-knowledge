Guide: How to Set Up a File Node Pool | RISEWiki

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

      * [Introduction](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/introduction)
      * [Pool Server Setup](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/pool-server-setup)
      * [Updating and Verifying Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/updating-and-verifying-pool-server)
      * [Managing Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/managing-pool-server)
      * [Node Rewards](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/node-rewards)
      * [Public Pools](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/public-pools)
    - [Public Pools Dashboard](/documentation/nodes/public-pools-dashboard)
    - [Node Delegation](/documentation/nodes/node-delegation)
* 🔗LINKS

  + [Official Website](https://www.infinityrising.com/)

[Powered by GitBook](https://www.gitbook.com/?utm_source=content&utm_medium=trademark&utm_campaign=PQmCVki2WHg9QcW9pdrX)

On this page

Copy

1. [📖Documentation](/documentation)
2. [Nodes](/documentation/nodes)

Guide: How to Set Up a File Node Pool
=====================================

[File Nodes are introduced here](/the-company/technology/nodes/file-nodes) in the copiwiki, what follows is instructions on how to setup and host one.

* [Introduction](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/introduction)
* [Pool Server Setup](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/pool-server-setup)
* [Updating and VerifyingPool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/updating-and-verifying-pool-server)
* [Managing Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/managing-pool-server)
* [Node Rewards](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/node-rewards)
* [Public Pools](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/public-pools)

**If you plan on setting up your node pool locally you might want to check to make sure your network supports port forwarding (required for nodes) natively.**

On the local machine you plan to run the node pool on, open a command prompt (cmd on Windows) and type

Copy

```
tracert [your_ip_address]
```

, replacing "[your\_ip\_address]" with your actual IP address which can be found by searching "what is my ip" online. You should only see one "hop" or line. If you see multiple, your network does not support port forwarding natively.

**Example:**

Copy

```
tracert 64.233.176.138 Expected Result: 1 <1 ms <1 ms <1 ms 199-119-153-199-119-153-27.cpe.sparklight.net [199.118.152.28]
```

(the numbers don't matter, but you should only have 1 line)

[PreviousNodes](/documentation/nodes)[NextIntroduction](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/introduction)

Last updated 8 months ago

This site uses cookies to deliver its service and to analyze traffic. By browsing this site, you accept the [privacy policy](https://infinityrising.com/legal/privacy-policy).

AcceptReject