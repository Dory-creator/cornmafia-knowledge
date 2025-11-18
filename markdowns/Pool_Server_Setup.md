Pool Server Setup | RISEWiki

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

* [Pool Server Setup](#pool-server-setup)
* [Helpful Skills](#helpful-skills)
* [Before Starting](#before-starting)
* [Create Pool Server Config](#create-pool-server-config)
* [Refreshing Pool Server Access Key](#refreshing-pool-server-access-key)
* [Delegate File Node](#delegate-file-node)
* [Installing Docker](#installing-docker)
* [Creating Public Access](#creating-public-access)
* [Choosing Cache Storage](#choosing-cache-storage)
* [Starting the Container](#starting-the-container)

Copy

1. [📖Documentation](/documentation)
2. [Nodes](/documentation/nodes)
3. [Guide: How to Set Up a File Node Pool](/documentation/nodes/guide-how-to-set-up-a-file-node-pool)

Pool Server Setup
=================

Pool Server Setup
-----------------

### Helpful Skills

Running a pool server will require some advanced technical knowledge. The following are some of the skills that may be required in running a successful pool server:

* General docker understanding. (<https://docker.com>)
* Running commands on the command line. This could be windows or linux.
* Understanding of general networking, firewalls, and internet router configurations.
* Looking at logs of data events to help with troubleshooting.

### Before Starting

Before starting the setup process you might want to check to make sure your network supports port forwarding natively. To do this, start by finding your public IP address. Most search engines like Google will provide this information if you search "What is my IP?". Next, open your command prompt (`cmd` on Windows). Type the command `tracert X.X.X.X` replacing the X's with your public IP address. Trace route (or `tracert)`will show the "hops" from your location to another IP address. If there is only one "hop" or line then your should be able to use port forwarding. If you see more than one "hop", then you should contact your ISP before proceeding.

Example:

`tracert [your_ip_address]`

Expected Result:

`1 <1 ms <1 ms <1 ms 199-119-153-199-119-153-27.cpe.sparklight.net [199.118.152.28]`

(the numbers don't matter, but you should only have 1 line)

### Create Pool Server Config

If the player is a node owner, then they should be able to see a section in the UI for managing their pool servers. Click on the link to manage pool servers, and click “Create Pool Server”.

Enter the name of the pool. The name of the pool should be a concise description of the pool. This is especially important if the player will likely be running multiple pool servers and even running one or more public servers.

Once the pool server is created, a secret access key will be presented. This key will be used in running the pool server. This is how the pool server software will know its configurations and provide performance information for its nodes that will yield rewards. Store this key in a safe place.

### Refreshing Pool Server Access Key

The pool access key does need to be kept secret, but if there is any reason that a node owner suspects that the key has been compromised, go to the pool management section of the player account. Click to see the details of the pool server in question. Click on the button to refresh the access key. The access key will be shown one time only. It is recommended that the access key be replaced in the `docker-compose.yml` configuration immediately since the old access key will no longer work. Once the configuration is updated, restart the docker container with the command `docker compose up -d` .

### Delegate File Node

The last step in creating a new pool server is to delegate a node. It is possible to run a pool server without a node. However, no work will be allocated to the pool unless at least one node is delegated to the pool.

In order to delegate a node, go to the Node section of the player account, and choose a node that has not been delegated. Click the button that says delegate node. When a dialog box appears, it should allow the selection of available pools. Choose a pool and click ok.

### Installing Docker

Docker is the chosen technology to roll out the pool server technology. This was chosen for several reasons:

1. Isolation: docker runs containers that will not allow host applications to affect the container and the container cannot negatively affect the host applications.
2. Ease of configuration: Most of the setup and configuration is done when the image is created. To containerize the image, only a few variables need to be set to get the docker to work as expected.
3. Platform choice: Docker can run on Windows, Linux, and Mac. It can also run on many NAS devices and on many cloud servers. Note: Cornucopias will not test every platform. Stick with Windows and Linux for the best support. We will not prevent the images to be run in other configurations. However, watch your performance metrics!

#### Windows

Running docker on windows is best facilitated using docker desktop. Use the following URL to download and install the tool. If you are new to docker, there should be a lot of information available to give you confidence that it is a safe and useful tool.

<https://www.docker.com/products/docker-desktop/>

Docker desktop will run on Linux and Mac. Follow these instructions for Mac and Desktop Linux.

#### Linux

Running docker on Linux might be a little more complicated. It is possible to run Docker Desktop on desktop Linux. However, these instructions will focus on a command line installation of docker engine. Think of this as the “server” approach. These instructions will help to deploy to home linux servers and cloud servers. Obviously, there are many distributions and versions of Linux, and this document is not meant to be exhaustive. Instead, refer to the docker documentation for latest information on installing docker engine.

<https://docs.docker.com/engine/install/>

Once the installation is complete, running the command docker ps should return an empty set of running containers.

### Creating Public Access

Creating public access to a pool server might be the trickiest part of this setup. It is important to make this right because it might open up your private network to the public Internet. Do this at your own risk. Also, please only forward necessary ports to your internal host. Redirecting all Internet traffic to an internal host is NOT recommended. (Some routers may have this option)

First, determine the public port number. If running behind a NAT (like at home), configure port forwarding for port 8001/tcp on the router. The port should be forwarded to the internal ip address that the pool server is running on and port 8001/tcp. For example, configure 8001/tcp on the router to forward to 192.168.1.22 port 8001/tcp. Note that some networks may change the internal IP address unexpectedly, so it is best practice to configure the internal host to have a static IP address.

The IP address and ports may differ in various configurations, and the pool server configuration should be able to accommodate many different configurations.

If running in the AWS cloud, configure the security group to allow tcp access to port 8001/tcp.

The following are some videos that might help setting up a port forward.

* <https://www.youtube.com/watch?v=jfSLxs40sIw>

### Choosing Cache Storage

Choose a location on the computer that can hold all of the cache files. Here are some of the considerations:

1. Which drive contains enough free space? There could be 100G of cache files as the project starts getting up to speed.
2. Drive speed can be important. NVMe drives are much faster thanIt would be nice if the storage was on a fast drive such as an NVME. However, using a spinning drive might make the most sense. Note that the validation of cache files will take long on these drives. This will not be a long term issue because it is on the roadmap to fix.

Now that the cache folder is chosen, the container can be started.

### Starting the Container

There are various ways that the container can be managed. A long command on the terminal or creating the container in the desktop application are both options that have been considered. The long command is too error prone, and believe it or not, the desktop creation of the container is cumbersome and error prone as well. Docker compose is the strategy that is the best solution for giving and receiving instructions for how to run this container. How about some terminology?

Docker Image: An image is the template for which a container will run. All of the software and dependencies have been packaged up and downloaded as an image.

Docker Container: A container is an image that has been run. Once an image has been run, it creates a state, and that state is stored as a container. If a new image is available, a container needs to be recreated in order to take advantage of the updated image.

Yaml: Docker compose uses a file called docker-compose.yml. Call this the docker compose file or the yaml file. This is just the phonetic way to refer to the file type.

Before starting the container, take a look at the variables that need to be updated. These variables will be in the docker compose configuration file, and can be changed easily.

#### Environmental Variables

Variable

Value

Description

`FILENODES_POOL_API_URL`

`https://filenodes.api.conucopiasweb.io`

Not Recommended: This is the hostname that will be used to receive instructions. The hostname will change when moving from staging to production, for example.

`FILENODES_POOL_ACCESS_KEY`

Unique key from pool server creation. Example:

gvgA??????????????????????????????????????yJY

Each pool server will have its own unique key that authenticates and authorizes it for participation in the file nodes network.

`FILENODES_POOL_PUBLIC_PORT`

`8001`

Each pool server will tell the API server how the client should access the files it is caching. This would be a public IP and port.

`FILENODES_POOL_PUBLIC_HOST`

`None`

Not Recommended: Use this environmental variable if the IP is not determined correctly by the filenodes service.

`FILENODES_POOL_PUBLIC_PATH`

`cache`

Not Recommended: Use this environmental variable to change the base URL path to access cached files.

#### Docker Compose Configuration

The following is an example docker compose configuration. Please create a folder on your computer that will have plenty of free disk space (100G-250G), and create the file “docker-compose.yml”. Copy and paste the template below, and carefully update the access key, public url, and cache path. Save the file and move to starting the container.

#### Step by Step Docker Configuration

Each will be discussed in the step by step approach for deploying a pool server.

1. Create a working folder. For example: “D:\CornPoolServer”.

   1. Open up explorer to where you would like to create your working folder.
   2. Right click in the open space and select new, then folder.
   3. Name your folder then hit enter.
   4. Double click on the folder to go into that newly created folder.
2. Create a folder inside that folder for the pool server cache. For example: “D:\CornPoolServer\cache”

   1. Right click in the open space and select new, then folder.
   2. Name your folder(cache) then hit enter.
   3. Do not double click on this folder for the next step. In the future, you may navigate to the folder to watch all of the cache files being created.
3. Use a text editor or notepad to create a docker-compose.yml file inside the working folder. For example: “D:\CornPoolServer\docker-compose.yml” Note: If using notepad you will need to “save as”, then select “all files” and make sure the file name ends in .yml
4. Copy and paste the docker compose template below into the docker-compose.yml file. Note: indentation and spacing matter.
5. Should the container always restart? For testing or manual management, change the restart value to “no”.
6. Update the access key. Copy and paste the access key that was provided.
7. Ensure that the public port matches port forward port.
8. Configure the cache folder. Update the path of the mapping to the internal docker path with a filesystem path. For example: “D:\CornPoolServer\Cache:/cache”.

#### Sample docker-compose.yml with cache configured to path

Copy

```
name: cornucopias
services:
    pool-server:
        image: public.ecr.aws/cornucopias/nodes/pool-server:latest
        ports:
          - "8001:8001"
        restart: unless-stopped # if you want to manually start the pool server replace “unless-stopped” with “no”
        environment:
            FILENODES_POOL_ACCESS_KEY: <PASTE ACCESS KEY HERE>
            FILENODES_POOL_PUBLIC_PORT: 8001
        volumes:
          - D:\CornPoolServer\Cache:/cache
```

#### Starting Docker

Starting docker is pretty easy. Do not get intimidated by using the command line. Ask for help.

**Open powershell or cmd.**

![](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2Flh7-rt.googleusercontent.com%2Fdocsz%2FAD_4nXcxFBtxubSkkw1C2LcxSBq1xZ4mwKdfYYrj0es_qFXiS08c95fOz7NQaxpX7ooi3QPFb25Soyr5ILkwUP749naVBXu1M3ynQtHAlecMpHddEG2zIj0D-Qy5Uvqgj15MghCaflSA5yUGSqXKxbpRsfUZlhU%3Fkey%3D7pNPNUdijy-V80BvXQjgPQ&width=768&dpr=4&quality=100&sign=58fa482d&sv=2)

**Change to working folder:**

![](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2Flh7-rt.googleusercontent.com%2Fdocsz%2FAD_4nXeA7OP_oFUaBSWYFxf58UYUGSR7ZJsuShR3kiqe7AZxkCqGqdbHimxzU7hB2AOb6GXLvMfhX-0GF45bcj1y4qhei4sfM-FuU2s0urH6swWK9gFBWiUn5WrjzBH7Unn3DeZZdnAi5w%3Fkey%3D7pNPNUdijy-V80BvXQjgPQ&width=768&dpr=4&quality=100&sign=3861f861&sv=2)

**Start pool server using the command “docker compose up -d”**

![](https://copiwiki.cornucopias.io/~gitbook/image?url=https%3A%2F%2Flh7-rt.googleusercontent.com%2Fdocsz%2FAD_4nXe-OcYDw6njyyN9T2sr2MzHvBShHLoXj-j7YldHJGdtAPNfwvjjaGPqObl9FkptrJsWRmX29xgKp8bbnJf3SCKtekRNKQPywJjWI_7BPZk0P1s0lh6WryvMHFtb8OjDH8VMIrTQpYDGoDU0VpDhIOzeAj8%3Fkey%3D7pNPNUdijy-V80BvXQjgPQ&width=768&dpr=4&quality=100&sign=2ff8a69e&sv=2)

[PreviousIntroduction](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/introduction)[NextUpdating and Verifying Pool Server](/documentation/nodes/guide-how-to-set-up-a-file-node-pool/updating-and-verifying-pool-server)

Last updated 6 months ago