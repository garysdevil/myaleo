# myaleo.aleo
- 教程
    - https://www.entropy1729.com/aleo-development-starter-pack/
    - https://www.entropy1729.com/getting-started-aleo-instructions/

## Build Guide


```bash
# Compile this Aleo program
aleo build

# Run
# aleo run 函数名 输入参数 输入参数
aleo run hello 2u32 3u32
```


```bash
# 创建A账户
aleo account new

# 创建B账户
aleo account new

# A账户部署mint 100个token
aleo run mint_token A账户私钥 100u64 3634422524977942384127113436866104517282080062207687912678345956934082270693field

# A账户部署mint 100个token
aleo run transfer "mint_token时的输出" B账户地址 10u64
# aleo run transfer_token "{
#   owner: aleo1ehzqv5492sa5n57nfjwfj3xfgdws9wakalgh3hswepwngw0huvxs4ch0wl.private,
#   gates: 0u64.private,
#   amount: 100u64.private,
#   _nonce: 7700575229588452849874644034163475795874053434716094434797350333297207342206group.public
# }" aleo1ck8n80597cfhx6yq4sq40xvghkxn30qnljlqdm3z4mjcm42ajyyqjqelrn 10u64
```

```conf
Private Key  APrivateKey1zkpFCE8GgNZWLQpwm3fsr5XNpPR8dHD3QsuPCMHUb7mHaVA
    View Key  AViewKey1hU73JxupzRh7uEnynsXgUQL3neSJcJZ2dMBkCPh97zoZ
    Address  aleo1ehzqv5492sa5n57nfjwfj3xfgdws9wakalgh3hswepwngw0huvxs4ch0wl


Private Key  APrivateKey1zkpJdfVa4iFAZjdWM94vB3F8ERonpXqmc8M24hGv2Twg2GF
    View Key  AViewKey1eZqsm6igutMTUbnwWw8vPQG5ceJruyYQs8XwTmNQdMJf
    Address  aleo1ck8n80597cfhx6yq4sq40xvghkxn30qnljlqdm3z4mjcm42ajyyqjqelrn
```

```bash
# 运行本地开发者节点
aleo node start

# 查看本地开发者节点块高
curl http://localhost:4180/testnet3/latest/block/height

curl http://localhost:4180/testnet3/latest/block/hash

```