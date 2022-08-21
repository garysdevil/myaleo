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

# 创建一个token
# aleo run mint_token token的地址 数量 密码
aleo run mint_token aleo1nmjzszxsejh0ec6s9tgdx03g24l8e3ev0jy6fx2ckz7s4vt7hgxqu8hz04 100u64 3634422524977942384127113436866104517282080062207687912678345956934082270693field

# token转账
# aleo run transfer_token record记录  token的地址 数量
aleo run transfer_token "{
  owner: aleo1nmjzszxsejh0ec6s9tgdx03g24l8e3ev0jy6fx2ckz7s4vt7hgxqu8hz04.private,
  gates: 0u64.private,
  amount: 100u64.private,
  _nonce: 3024738992072387217402876176731225730589877991873828351104009809002984426287group.public
}" aleo1nmjzszxsejh0ec6s9tgdx03g24l8e3ev0jy6fx2ckz7s4vt7hgxqu8hz04 10u64

# 在本地部署aleo应用
aleo node start
```