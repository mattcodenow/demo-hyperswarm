# Demo Hyperswarm
Demonstration of connecting with many peers by topic.  
Duplicated from the documentation found at [https://docs.holepunch.to/quick-start](https://docs.holepunch.to/quick-start).

## Clone
To clone the project enter the following in your terminal:
```
git clone https://github.com/mattcodenow/demo-hyperswarm.git
```
Change into the project directory:
```
cd demo-hyperswarm
```

## Install
From inside the project directory:
```
npm install
```

## Start

### Peer A
From a terminal window inside the project directory:
```
node peer.mjs
```
This first peer instance on this first terminal window should print out the topic:
```
joined topic: 2415d390a0a970ec66a6d45fcc4dd3482fd6fc13978329f834fe32ee709afba7
```

### Peer B
From a second terminal window inside the project directory:
```
node peer.mjs 2415d390a0a970ec66a6d45fcc4dd3482fd6fc13978329f834fe32ee709afba7
```

### A & B Peer Connection
Each peer terminal window should print out a connection event with a long id or key for the peer:
```
* got a connection from: 4ca7050e486d75e7abdfb6ce5b59e367691e490b63bbbf2367356b0055664284 *
```

### A & B Peer Chat
Try entering text in each terminal window, hitting the enter key, and watching how hyperswarm connects and mirrors the data to the other peer.  
