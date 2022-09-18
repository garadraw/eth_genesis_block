**Research**

1.  genesis.json File Documentation
https://gist.github.com/0mkara/b953cc2585b18ee098cd

2. Linux Ssh Connections
https://tutonics.com/2012/06/allow-multiple-ssh-sessions-over.html

3. Tmux Documentation
https://askubuntu.com/questions/8653/how-to-keep-processes-running-after-ending-ssh-session

4. Create your Own Private Eth Network
https://gist.github.com/0mkara/b953cc2585b18ee098cd

5. Geth Documentation
https://geth.ethereum.org/docs/interface/command-line-options




**Geth Commands**

Initialising a Blockchain in the Current Folder
- geth --datadir . init genesis-block.json
Mining on Blockchain and Sending the Minted Tokens to an Account
- geth --allow-insecure-unlock --datadir . --keystore ~/Library/ethereum/keystore --networkid 4568 --http --http.addr '0.0.0.0'
--http.corsdomain "*" --http.port 8502 --http.api 'personal,eth,net,web3,txpool,miner' --mine --miner.etherbase=<Publick Key Account Here>
To Enter the Java Console
- geth attach geth.ipc



**To Use Geth Functions**

To Check Balance of Account
- web3.eth.getBalance()
To Check if Address
- web3.isAddress()



**Linux Commands**

Create a Secondary Shh Connection to the Same Server(Use Tmux to Keep it Open After you End the Ssh Connection)
- ssh -S none v@192.168.1.56
