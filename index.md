## Flotorizer

Flotorizer is a web app that was already built. The goal was to make a transaction using [OIP HD-MultiWallet](https://github.com/oipwg/oip-hdmw) so that a full node is not required. So the existing code needed to be changed.

**FLO blockchain** has the ability to permanently store 1040 bytes of data per transaction. More information can be found [here](https://flo.cash/).

Upon selection of a file, the software on the client side calculates a **sha-512 hash** of the document and sends it to the server. The server then executes a transaction using **OIP HD-MultiWallet** and stores the hash in the **blockchain**. If everything is successful, then finally a pdf with the information about the transaction where the hash can be found is given as output.


**Demo** :  [Flotorizer web app](http://www.flotorizer.net/)


<img src="screenshots/flotorizer.png" width="1000">
