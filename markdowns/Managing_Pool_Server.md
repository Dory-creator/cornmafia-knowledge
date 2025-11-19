Managing Pool Server | RISEWiki

[![Logo](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2F1762761122-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Forganizations%252FVpfHHIHQI6ROs7kspCfa%252Fsites%252Fsite_dzbNR%252Flogo%252F90i8Iwb0LXw9xIroe9wy%252FInfinity%2520Rising_logo2.png%3Falt%3Dmedia%26token%3Dde7ab13b-7593-4583-83e6-7ed79d87ed26&width=260&dpr=4&quality=100&sign=8e852af&sv=2)![Logo](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2F1762761122-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Forganizations%252FVpfHHIHQI6ROs7kspCfa%252Fsites%252Fsite_dzbNR%252Flogo%252FbwYsgKrrCmFJzlM7KKwZ%252FInfinity%2520Rising_logo2.png%3Falt%3Dmedia%26token%3Dc62ee205-acdf-47b2-9313-ca755597bd96&width=260&dpr=4&quality=100&sign=c99ea5b2&sv=2)](/)

`Ctrl``k`

* [📋INFINITY RISING](/)
* 🎮GAMEPLAY

  + [About the game](/gameplay/about-the-game)
  + [Gameplay - PC](/gameplay/gameplay-pc)
  + [Non-Player Characters](/gameplay/non-player-characters)
  + [Themed Zones](/gameplay/themed-zones)
  + [Mega Dome - Calido Valley](/gameplay/mega-dome-calido-valley)
  + [Gameplay - eSports Racing League](/gameplay/gameplay-esports-racing-league)
  + [Gameplay - Mobile](/gameplay/gameplay-mobile)
  + [Game Launcher](/gameplay/game-launcher)
  + [City - Life](/gameplay/city-life)
  + [Community](/gameplay/community)
* 🌐BLOCKCHAIN

  + [Blockchain Wallets](/blockchain/blockchain-wallets)
  + [Cardano World](/blockchain/cardano-world)
  + [COPI Stake Pool](/blockchain/copi-stake-pool)
  + [COPIC Stake Pool](/blockchain/copic-stake-pool)
  + [$COPI Token](/blockchain/usdcopi-token)
  + [Marketplace](/blockchain/marketplace)
  + [PLAYER OWNED ASSETS](/blockchain/player-owned-assets)
* 🧑‍🤝‍🧑THE COMPANY

  + [COMPLIANCE](/the-company/compliance)
  + [Founders](/the-company/founders)
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

  + [Link Tree](https://linktr.ee/cornucopias.game)
  + [Official Website](https://www.infinityrising.com/)

[Powered by GitBook](https://www.gitbook.com/?utm_source=content&utm_medium=trademark&utm_campaign=PQmCVki2WHg9QcW9pdrX)

On this page

Copy

1. [📖Documentation](/documentation)
2. [Nodes](/documentation/nodes)
3. [Guide: How to Set Up a File Node Pool](/documentation/nodes/guide-how-to-set-up-a-file-node-pool)

Managing Pool Server
====================

From time to time, pool servers are going to need to be upgraded or restarted. The following are a few commands that can be used to hopefully get your pool back to earning rewards.

This kind of maintenance is using the command line, but don’t worry, it is not that hard. Similarly to the example in [Change to working folder: “cd d:\CornPoolServer](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/pool-server-setup#starting-docker), go to that same path.

If the pool server needs to be stopped, then the following command can be used. This function can also be achieved using the docker desktop. Find the container named “pool-server-1” and click the stop button.

Copy

```
docker compose stop
```

If the pool server needs to be restarted, click the stop and start buttons in docker desktop or execute this command in the same folder as the docker-compose.yml file.

Copy

```
docker compose restart
```

This is the maintenance that must be done on the command line. Docker desktop is improving, and it may provide deeper integration with docker compose in the future, but until then, these commands will help to recreate the pool server container.

Copy

```
docker compose stop
docker compose rm
Docker compose up -d
```

[PreviousUpdating and Verifying Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/updating-and-verifying-pool-server)[NextNode Rewards](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/node-rewards)

Last updated 11 months ago

This site uses cookies to deliver its service and to analyze traffic. By browsing this site, you accept the [privacy policy](https://infinityrising.com/legal/privacy-policy).

AcceptReject