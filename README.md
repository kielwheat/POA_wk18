# POA zbanktest

This repo contains instructions for launching the zbanktest blockchain network.  There is a screenshot folder that will help guide users in the setup.

Instructions:
1. Run geth to creat two account nodes.  
    ./geth --datadir node1 account new  (and then substitute node2)
    This will create the public and private keys.  These and their passwords can be found in the chain config file.  If you would like to make another account, simply create a new node (node3 for example)
2. Run puppeth to create the zbanktest block.  Copy the inputs from puppeth_config screenshot or the chain config file.  This will create a new genesis block with the Clique (Proof of Authroity) consensus algorithm.
3. Begin mining blocks by following the Mining block instructions in the chain config.  This will allow transactions between node1 and node2 to occur by using the MyCrypto wallet.
4. Connect to the zbanktest network in MyCrypto by following the instructions in the MyCrypto_network picture tutorial
5. Send a test transaction in MyCrypto:
    a. Open MyCrypto 
    b. Follow the instructions in the MyCrypto_transaction picture tutorial to send a transaction between nodes.
    C. A successful transaction should look like the tx_success picture, however there may be a network lag that doesn't update the pending message so make sure to confirm balances!
