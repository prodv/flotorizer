## Flotorizer

Flotorizer is a web app that calculates the **sha-512 hash** of a file and stores it into the FLO blockchain. This blockchain has the ability to permanently store 1040 bytes of data per transaction (https://flo.cash/).

It was built using **NodeJS**.

Upon selection of a file, the software on the client side calculates a sha-512 hash of the document and sends it to the server. The server then executes a transaction using **OIP HD-MultiWallet** and stores the hash in the blockchain. If everything is successful, then finally a pdf with the information about the transaction where the hash can be found is given as output.

Hence existence of a file can be proved this way i.e the file was present atleast at the time of transaction.

If any one contested that the file actually existed, then all we have to do is to calculate it's signature with any independent sha-512 calculator and compare the result with the record in the Blockchain. No one can delete the record and the record is public.

Demo :  http://www.flotorizer.net/


<img src="screenshots/flotorizer.png" width="1000">
