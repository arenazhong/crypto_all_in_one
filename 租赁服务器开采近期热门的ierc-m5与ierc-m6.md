### ierc-m6 挖矿指南（当前进度 0.319%）

> **进度查询**（需科学上网）：[https://www.ierc20.com/tick/ierc-m6](https://www.ierc20.com/tick/ierc-m6)

---

#### 重要安全提示
1. **禁用网页版挖矿**：网页版需导入私钥，已发生多起盗币事件，建议使用命令行版本
2. **设备要求**：家用电脑性能不足，国内云服务器（阿里/腾讯云）无法下载挖矿程序
3. **推荐方案**：使用支持加密货币充值的海外GPU服务器平台

---

### 操作流程

#### 1. 服务器租用
- **注册平台**：[vast.ai 新用户注册](https://cloud.vast.ai/?ref_id=88254)
- **机型选择**：RTX3080/3090（时租约$0.15），无需RTX4090
- **配置指南**：[GPU服务器租用教程](https://heiyetouzi.xyz/minequainetwork/#toc-heading-15)（直接查看第三章节）

![](https://ac63e02.webp.li/ierc20m6-001.png)
![](https://ac63e02.webp.li/ierc20m6-002.png)

---

#### 2. 环境配置
通过控制台执行以下命令：
```bash
apt update && apt install nodejs npm vim -y
npm install n -g
n stable
hash -r
node -v 
git clone https://github.com/IErcOrg/ierc-miner-js
cd ierc-miner-js
npm i -g yarn
yarn install
```

---

#### 3. 配置文件修改
```bash
vim tokens.json
```
替换为以下内容（`:wq`保存）：
```json
{
  "ierc-m4": { "workc": "0x0000", "amt": "1000" },
  "ierc-m5": { "workc": "0x00000", "amt": "1000" },
  "ierc-m6": { "workc": "0x000000", "amt": "1000" }
}
```

---

#### 4. 启动挖矿
```bash
yarn cli wallet --set [你的ETH私钥]
yarn cli mine ierc-m6 --account [你的ETH地址]
```
![](https://gcore.jsdelivr.net/gh/btcltceth/blogassets@v0.2.26/b/img/ierc20m6-003.png)

---

### 收益管理
- **实时查询**：[https://www.ierc20.com/tick/ierc-m6](https://www.ierc20.com/tick/ierc-m6)（需科学上网）
- **交易价格**：当前单价约10U/枚
- **扩容建议**：支持多机并行挖矿

![](https://ac63e02.webp.li/ierc20m6-004.png)
![](https://ac63e02.webp.li/ierc20m6-005.png)

---

### 延伸阅读
[2025中国十大虚拟币交易平台排名🔥](https://btc8848.com/top-10-exchanges/)  
[币圈暴富故事：从1100万到负债10万](https://heiyetouzi.xyz/biquanstory001/)

---

#### 热门搜索
比特币购买 | POW挖矿 | ierc挖矿 | 交易所注册 | OKX下载 | 币安App | 合约交易 | Web3空投 | NFT钱包 | 质押挖矿 | 铭文铸造 | 节点运营 | 杠杆策略 | btc8848.com | heiyetouzi.xyz