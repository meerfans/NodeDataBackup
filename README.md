# qngNodeDataBackup

data backup for qng node


Here is a backup for qng node data, which is the data before block 1100000. This will help you quickly sync to the latest status.(这里有一个 110万高度之前的 qng 节点数据备份，它可以帮助你快速同步到最新状态。)

- qitmeer.io source

  https://www.qitmeer.io/resource/download/NodeDataBackup/data110.zip

- github source

  https://github.com/meerfans/NodeDataBackup/releases/download/data.110/data110.zip

- pan.baidu.com

  链接（link）: https://pan.baidu.com/s/1t_CM9NVgT6Nl7DWBeho_iQ  密码（key）: 4cv1
  

## qng config

copy the config bellow to `qng.conf`.

```bash
#testnet=1
datadir=./data
logdir=./data
notls=false
printorigin=false
debuglevel=debug

## for rpc 
rpclisten=0.0.0.0:18131
rpcuser=meer
rpcpass=meer123

## P2P port,default 8130
port=18130

## cache set, which can increase synchronization rate, default is 2000, for 8G memory,the recommended value 20000.
bdcachesize=20000
dagcachesize=20000

#evmenv="--http --http.port=18545 --ws --ws.port=18546"
evmenv="--http --http.port=1234 --http.api=personal,net,web3,eth,qng,txpool"

#evmenv="--allow-insecure-unlock --http --http.port=1234 --http.api=personal,net,web3,eth,qng,txpool --ws --ws.port=18546 --ws.addr=0.0.0.0 --ws.api=eth,web3,net,debug,txpool"

#addpeer=/ip4/18.167.121.52/tcp/28130/p2p/16Uiu2HAmEUYzcShySWjU4ELYMqvWjH1Z3uL6iG4vaeZwAuHidquR
```
