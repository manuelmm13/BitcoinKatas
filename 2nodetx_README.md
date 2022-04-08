2 node exercise through CLI 

>bitcoin-cli addnode “Node1Address" "add"
>bitcoin-cli addnode “Node2Address" "add"
>bitcoin-cli generateblock "Node1Address" '["tx1"]'
>bitcoin-cli createrawtransaction "[{\"tx1\" : \"mytxid\",\"vout\":0}]" "{\"Node2Address\":amount}"
>bitcoin-cli signrawtransactionwithwallet "myhex"
>bitcoin-cli sendrawtransaction "signedhex"
>bitcoin-cli getaddednodeinfo "Node2Address"