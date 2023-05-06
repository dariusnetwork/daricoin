# daricoin-genesis
 Daricoin Genesis data 7 May 2023!

 This is a genesis data for Darius Network that powered Daricoin $DARI

 # Joining the Network

 ## Step 1: Download geth
 Use geth version is Azimir (v1.11.6)

 For linux

 ```
wget https://gethstore.blob.core.windows.net/builds/geth-linux-amd64-1.11.6-ea9e62ca.tar.gz
tar -xvf geth-linux-amd64-1.11.6-ea9e62ca.tar.gz
 ```

For Mac OS

```
wget https://gethstore.blob.core.windows.net/builds/geth-darwin-amd64-1.11.6-ea9e62ca.tar.gz
tar -xvf geth-darwin-amd64-1.11.6-ea9e62ca.tar.gz
```

For Windows

```
curl https://gethstore.blob.core.windows.net/builds/geth-windows-amd64-1.11.6-ea9e62ca.exe -o geth-windows-amd64-1.11.6-ea9e62ca.exe
```

# Join the consensus 

```
./geth --identity "DariusCoin-linux-dl-node-1" --authrpc.port "3550" --syncmode full --http.addr 0.0.0.0 --http --http.port "1237" --http.corsdomain "*" --http.api "eth,net,web3,txpool,admin,miner,debug" --datadir "DARICOIN/genesis/data" --port "3001" --networkid 789 console --nodiscover --http.vhosts "*" --syncmode=full --gcmode=archive  --mine --miner.threads=1 --miner.etherbase=0x248b714C06Dd454A1Fc7072626a062cC578EC96F
```
Change the miner address with your own address that you are having private key. `0x248b714C06Dd454A1Fc7072626a062cC578EC96F` this should be changed so that mined coin is deposited to your address. Each successfull miner will get 2 DARI Coin in every 12 seconds.

Add the following in console
```
admin.addPeer("enode://0d792fda911f12434c507ec3a539cf9b5c9c912c01c7b445870599b7d881906c3648b3e375a434430672b8c036a22fca42077b1738718d2f3a90c67a19f4ce92@159.89.163.141:3001")
```

 
