# Lido - 致质押用户

## 申明

本文旨在为准备使用 Lido 进行收益创造的 Web3 用户提供指导，尤其是质押参与者。文章将快速回顾 Lido 的基本概念，并重点讨论作为质押参与者可能面临的风险及其可控性。



## Lido 介绍

Lido 是一个去中心化的质押协议，旨在为用户提供流动性和便利性，使用户能够在参与质押的同时，仍然能够使用其资产。作为一项创新的解决方案，Lido 允许用户在质押以获取收益的同时，还能获得一种称为 `st[xxx]` 的代币，这个代币代表着用户在质押过程中所获得的权益。



### 核心概念

1. 流动质押池：管理存款、质押奖励和提款的协议。
2. `st[token]`[^1]：质押凭证，可与其他 Defi 项目交互，产生二次收益。
3. `DAO`[^2]：Lido Liquid 协议管理实体，负责选择节点运营商、配置协议参数等等。
4. 节点运营商：管理安全稳定的基础设施以运行验证器客户端以实现协议的实体。



### 主要解决的问题

1. 降低质押门槛。
2. 提升质押流动性。



### 收益

> 用户年化利率 = 协议年化利率 * (1 - 协议手续费）

+ 协议年化利率：动态变化的，为最近7天总收益与总池的比值。

+ 协议手续费：固定10%，由 Dao 组织和节点运营商平分。



## 风险分析

作为质押参与者，以下几点是用户需要了解并关注的风险：

### 质押过程的注意事项

1. **代码安全性**：虽然官方会进行多轮代码审计并提供 Bug 赏金，但仍存在潜在的代码风险。
2. **市场风险**：质押资产的市场波动可能影响投资收益，务必关注资产价格的变化。

### 提现过程的注意事项

1. **提现时间**：一般为1到5天，具体取决于请求金额、队列中 `stETH` 的总量以及[其他因素](https://stake.lido.fi/withdrawals/request#withdrawalsPeriod)。
2. **削减风险**：由于协议产生的削减[^3]或处罚[^4]，最终赎回的以太币可能少于最初提交请求时的预期。
3. **不可撤回性**：一旦发起提现请求，无法撤回，且在此期间不产生收益。



## 应对措施

虽然面对合约代码安全漏洞或节点运营商的不当行为，普通用户通常无能为力，但可以采取以下措施：

1. **关注社区动态**：定期查看 Lido 的社区更新和开发者讨论。
2. **参与治理**：参与 Lido DAO 的治理，关注重要参数的投票和讨论。
3. **监测指标**：定期查看 Lido 在线指标和自我评分，掌握协议的运行状态。



## 其它链接

+ Lido 的自我评分：https://lido.fi/scorecard
+ Lido 在线指标查看：https://dune.com/lido/lido-node-operator-withdrawals

+ Lido 提款流程介绍：https://hackmd.io/@lido/SyaJQsZoj

+ Lido 提现指标统计：https://dune.com/lido/lido-v2

+ ETH2 Staking 指标：https://dune.com/hildobby/eth2-staking





[^1]: 在 Lido 上质押可以获得 Lido Tokens，各类 Token 区别介绍[见此](https://docs.lido.fi/guides/lido-tokens-integration-guide#lido-tokens ↩)。
[^2]: Lido DAO 是一个去中心化自治组织，通过治理代币（ `LDO` ）持有者的投票权决定关键参数（例如，设置费用、分配节点运营商和预言机等）来管理流动性质押协议。此外，DAO 将积累服务费并将其用于研究、开发、流动性挖矿激励和协议升级。职责详情[链接](https://docs.lido.fi/lido-dao#functions)，不同分类的委员会[介绍
[^3]: Slashing [削减](https://ethereum.org/en/developers/docs/consensus-mechanisms/pos/rewards-and-penalties/#slashing)，意味着作为质押者触犯了 ETH 的底线，将被清理出局，并惩罚质押金。
[^ 4]: Penalties [处罚](https://ethereum.org/en/developers/docs/consensus-mechanisms/pos/rewards-and-penalties/#penalties)，如针对错过目标和源头投票的惩罚，将扣除对应原应得的奖励，惩罚力度较轻。

