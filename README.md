### bitcoin-ruby-node
---
https://github.com/mhanne/bitcoin-ruby-node

```json
{"id": 0, "method": <command>, "params": <params>}
{"id": <id>, "method": <method>, "result": <result>}
```

```sh
gem install bitcoin-ruby-node
bitcoin_node --help
bitcoin_node --import ~/.bitcoin/blocks --skip-validation
bitcoin_node_cli info
bitcoin_node_cli -c config.yml info
bitcoin_node_cli monitor "block tx"

echo -e '{"id": 1, "method": "tslb", "params"}' | nc 127.0.0.1 9999
rake doc
rake
rspec spec/node/command_api_spec.rb
```

```yml
all:
  network: bitcoin
  storage: sequel::postgres:/bitcoin
  command: 127.0.0.1:1234
blockchain:
  max:
    connect: 30
wallet:
  keystore: "simple::file=keys.json" 
```


