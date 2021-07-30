The first step after creating a directory was to install Go Etherum tools into the directory 
After that I needed to create the Nodes, for that I used the commands :
    ./geth account new --datadir node1
    ./geth account new --datadir node2
To Make a network I ran puppeth, named my network "hwnet"
Went through the process of Proof of Authority consensus algorithm.
Initialized each node with the new networkname.json with:
    ./geth init hwnet.json --datadir node1
    ./geth init hwnet.json --datadir node2
Then I ran the first node with:
    ./geth --datadir node1 --mine --minerthreads 1, the --mine; tells it to mine new blocks, the --minerthreads; tells how many CPU threads to use during the mining process 
Then in MyCrypto app, I used a custom node I have previously created with ChainID and ETH as a currency
I then used the keystore file from my directory to open Mycrypto wallet and send ETH from Node 1 into Node 2. for some reason I got pending in the transcation. 
I went back and sent ETH from Node 2 into 1 to see and I also got pending





