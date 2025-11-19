Updating and Verifying Pool Server | RISEWiki

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

Updating and Verifying Pool Server
==================================

* TODO: how will node owners be notified of upgrades.

Copy

```
docker compose pull # only if you need a new version
docker compose up -d # only if there is a new version or configuration change
```

![](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2Flh7-rt.googleusercontent.com%2Fdocsz%2FAD_4nXewTPZZBwrCM5khxzWspoziHKFz9sUjMM01n3lH8H4dvk2YibAL_GuF_zvw-7mB0DaJifjT822oMRl8KBWU5dAryZ_8LIePzFSbQYXPdCuiW4n_HQsKsfVBOyMY1XizrKDTkHNPDYBhh3qZ4IbY0H_jqjcV%3Fkey%3D7pNPNUdijy-V80BvXQjgPQ&width=768&dpr=4&quality=100&sign=e5427543&sv=2)

### Verify Functionality

There is a URL in the pool server that will allow the testing of the application and port forwarding. Testing from the same network may not provide correct results but it is valuable.. If it fails on the same network, it will also fail on remote networks.

1. Open this URL in web browser: `http://{PUBLIC_IP}:{PUBLIC_PORT}/health`. Be sure to replace the `{PUBLIC\_IP}` and `{PUBLIC\_PORT}` with the real values that are being tested.
2. When viewing in a browser, the result should be a simple “Ok”.
3. If the health check succeeds on the same network, pass the health URL to a friend for them to test.
4. What else would you like to see in the health check?

There should be some reports on the Pool server page that will show some recent performance numbers. This will include last checkin and number of errors in the current checking period.

Watch the logs!

[PreviousPool Server Setup](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/pool-server-setup)[NextManaging Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/managing-pool-server)

Last updated 11 months ago

This site uses cookies to deliver its service and to analyze traffic. By browsing this site, you accept the [privacy policy](https://infinityrising.com/legal/privacy-policy).

AcceptReject