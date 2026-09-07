# vps hosting coupon: BandwagonHost 现役优惠码、套餐价格与 CN2 GIA 选购全解

如果你正在搜 `vps hosting coupon`,大概率你不想按列表价原价下单。这篇文章把 BandwagonHost(搬瓦工)目前公开的循环优惠码、所有在售套餐的真实价格和配置,以及 CN2 GIA / E-Commerce SLA / Ultra 几条线路之间的差异一次说清楚——读完你能直接选到合适的方案,而不是再翻五篇文章凑齐信息。

## 一、为什么是 BandwagonHost

`bwh81.net` 是 BandwagonHost 的官方镜像域名,`aff.php?aff=...` 是它的联盟追踪入口。BandwagonHost 是一家以 KVM 虚拟化、自研 KiwiVM 控制面板和 CN2 GIA 中国三网优化线路著称的 VPS 服务商,机房覆盖洛杉矶、圣何塞、纽约、温哥华、阿姆斯特丹、迪拜、东京、大阪、香港、新加坡等十几个数据中心。它的特点是**自管型(self-managed)**——没有 cPanel、没有电话客服、没有托管,但价格因此压得很低,20G KVM PROMO 起价 $49.99/年,折合每月约 $4.17。

下面所有价格、配置都来自 BandwagonHost 官方 `/order/get-data` 接口在抓取时返回的实时数据,优惠码部分交叉了多个第三方优惠站和搬瓦工中文社区的更新记录。

## 二、当前可用的循环优惠码

BandwagonHost 的优惠码是**循环折扣(recurring)**,意思是续费时同样打折,不是只便宜一次。这一点比很多"首年 7 折、续费原价"的套路实在得多。

根据多个第三方优惠站(hostingcouponspot.com、techjury.net、valuecom.com)以及搬瓦工中文社区(bwgyhw.cn)在 2026 年的更新记录,目前公开可查到的循环优惠码如下:

| 优惠码 | 折扣力度 | 适用范围 | 状态 |
| --- | --- | --- | --- |
| `BWHCGLUKKB` | 6.78% 循环 | 全场 VPS | 多源交叉确认,2026 年仍被列为最大力度 |
| `ireallyreadtheterms8` | 5.5% 循环 | 全场 VPS | 长期稳定 |
| `ireadtheterms8` | 4.4% 循环 | 全场 VPS | 长期稳定 |
| `BWHWYWWYVY` | 5.96% 循环 | 全场 VPS | 第三方列表中可见 |

需要说明的是,优惠码的有效性会随时间波动。搬瓦工中文社区在 2026 年 3 月曾发过"所有公开优惠码失效"的更新,2 月又放出过 `NODESEEK2026`(6.77% 循环)这样的限时码。**最稳妥的做法**:在结账页面的 "Promotional Code" 输入框里逐个试,哪个能 Validate 通过就用哪个,优先试 `BWHCGLUKKB`。

> 提示:优惠码在结账时手动输入并点击 "Validate Code",页面会刷新显示折后价。续费时系统会自动套用你购买时用过的码,不用每次重输。

以 $49.99/年的 20G KVM PROMO 为例,套 `BWHCGLUKKB` 后实付约 $46.60/年,省下的钱够再买一个月流量包。

## 三、四条产品线,先搞清楚再选

BandwagonHost 把套餐分成四个 tier,差别主要在网络线路和机房等级,而不是 CPU/内存:

**1. Basic VPS(基础版)**
最便宜的一档,机房走普通国际线路 + 本地 peering,适合不在意中国方向延迟的用户——做海外跳板、跑脚本、放静态资源、做 CI runner 都没问题。机房包括纽约 USNY_6、洛杉矶 USCA_2、Fremont USCA_FMT、阿姆斯特丹 EUNL_2、温哥华 CABC_1。

**2. E-Commerce VPS(CN2 GIA-E)**
搬瓦工最有代表性的产品线。中国方向走电信 CN2 GIA(AS4809)/CTGNet(AS23764)、联通 Premium(AS10099)、移动 CMIN2(AS58807)三网优化,2.5Gbps 起步带宽。可选机房最多,包括洛杉矶 USCA_6/USCA_9、圣何塞 SJC5、纽约 USNY_8、温哥华 CABC_6、阿姆斯特丹 EUNL_1/EUNL_9、迪拜 AEDXB_1、东京 JPTY_1、大阪 JPOS_1 等。**面向中国访客的建站、跨境业务、远程办公首选这一档。**

**3. E-Commerce+SLA(LA USCA_5 专属)**
和 E-Commerce 同样的中国优化线路,但机房在洛杉矶 Coresite LA2(USCA_5),配备双路冗余电源、双 NIC、Tier III 设施,提供 **99.99% SLA** 保证(普通档是 99.95%)。适合不能停机的生产业务。目前只有 USCA_5 一个机房,套餐从 20G 到 1280G HIBW 20T 全覆盖。

**4. Ultra VPS(香港 / 东京 / 大阪 / 新加坡 CN2 GIA)**
物理上离中国最近、延迟最低的一档,但价格也最高。香港 HK_8(Equinix HK2)、东京 JPTY_8、大阪 JPOS_6、新加坡 SG_8。带宽 1–2.5Gbps。适合对延迟极度敏感的场景——游戏服、实时音视频、金融类业务。如果延迟不是硬指标,洛杉矶 E-Commerce 的性价比明显更高。

## 四、全套餐对比表

下面两张表覆盖 BandwagonHost 官方接口在抓取时返回的**全部在售套餐**。价格均为 USD,优惠前列表价;实际支付可叠加第三节中的循环优惠码。

### Basic VPS(基础版,1Gbps 带宽)

| 套餐 | CPU | RAM | SSD | 月流量 | 起价(计费周期) | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 20G KVM PROMO (pid=44) | 2 核 | 1 GB | 20 GB | 1 TB | $49.99/年 | [购买 20G Basic](https://bwh81.net/aff.php?aff=77528&pid=44) |
| 40G KVM PROMO (pid=45) | 3 核 | 2 GB | 40 GB | 2 TB | $52.99/半年 · $99.99/年 | [购买 40G Basic](https://bwh81.net/aff=77528&pid=45) |
| 80G KVM PROMO (pid=46) | 4 核 | 4 GB | 80 GB | 3 TB | $19.99/月 · $59.99/季 · $107.99/半年 · $199.99/年 | [购买 80G Basic](https://bwh81.net/aff.php?aff=77528&pid=46) |
| 160G KVM PROMO (pid=47) | 5 核 | 8 GB | 160 GB | 4 TB | $39.99/月 · $112.99/季 · $213.99/半年 · $399.99/年 | [购买 160G Basic](https://bwh81.net/aff.php?aff=77528&pid=47) |
| 320G KVM PROMO (pid=48) | 6 核 | 16 GB | 320 GB | 5 TB | $79.99/月 · $227.99/季 · $432.99/半年 · $799.99/年 | [购买 320G Basic](https://bwh81.net/aff.php?aff=77528&pid=48) |
| 480G KVM PROMO (pid=49) | 7 核 | 24 GB | 480 GB | 6 TB | $119.99/月 · $341.99/季 · $649.49/半年 · $1199.99/年 | [购买 480G Basic](https://bwh81.net/aff.php?aff=77528&pid=49) |

### CN2 GIA-E E-Commerce VPS(2.5–10Gbps,三网优化)

| 套餐 | CPU | RAM | SSD | 月流量 | 带宽 | 起价(计费周期) | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G CN2 GIA-E (pid=87) | 2 核 | 1 GB | 20 GB | 1 TB | 2.5 Gbps | $49.99/季 · $89.99/半年 · $169.99/年 | [购买 20G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=87) |
| 40G CN2 GIA-E (pid=88) | 3 核 | 2 GB | 40 GB | 2 TB | 2.5 Gbps | $89.99/季 · $169.99/半年 · $299.99/年 | [购买 40G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=88) |
| 80G CN2 GIA-E (pid=89) | 4 核 | 4 GB | 80 GB | 3 TB | 2.5 Gbps | $56.99/月 · $149.99/季 · $289.99/半年 · $549.99/年 | [购买 80G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=89) |
| 160G CN2 GIA-E (pid=90) | 6 核 | 8 GB | 160 GB | 5 TB | 5 Gbps | $86.99/月 · $239.99/季 · $459.99/半年 · $879.99/年 | [购买 160G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=90) |
| 320G CN2 GIA-E (pid=91) | 8 核 | 16 GB | 320 GB | 8 TB | 5 Gbps | $159.99/月 · $459.99/季 · $869.99/半年 · $1599.99/年 | [购买 320G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=91) |
| 640G CN2 GIA-E (pid=92) | 10 核 | 32 GB | 640 GB | 10 TB | 10 Gbps | $289.99/月 · $799.99/季 · $1499.99/半年 · $2759.99/年 | [购买 640G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=92) |
| 1280G CN2 GIA-E (pid=93) | 12 核 | 64 GB | 1280 GB | 12 TB | 10 Gbps | $549.99/月 · $1559.99/季 · $2979.99/半年 · $5499.99/年 | [购买 1280G GIA-E](https://bwh81.net/aff.php?aff=77528&pid=93) |
| 1280G GIA-E HIBW 15T (pid=160) | 12 核 | 64 GB | 1280 GB | 15 TB | 10 Gbps | $679.00/月 · $1935.00/季 · $3670.00/半年 · $6790.00/年 | [购买 1280G HIBW 15T](https://bwh81.net/aff.php?aff=77528&pid=160) |
| 1280G GIA-E HIBW 20T (pid=161) | 12 核 | 64 GB | 1280 GB | 20 TB | 10 Gbps | $899.00/月 · $2562.00/季 · $4860.00/半年 · $8999.00/年 | [购买 1280G HIBW 20T](https://bwh81.net/aff.php?aff=77528&pid=161) |

### E-Commerce+SLA(洛杉矶 USCA_5,99.99% SLA)

| 套餐 | CPU | RAM | SSD | 月流量 | 带宽 | 起价(计费周期) | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G SLA (pid=164) | 2 核 | 1 GB | 20 GB | 1 TB | 2.5 Gbps | $65.89/季 · $125.99/半年 · $239.99/年 | [购买 20G SLA](https://bwh81.net/aff.php?aff=77528&pid=164) |
| 40G SLA (pid=165) | 3 核 | 2 GB | 40 GB | 2 TB | 2.5 Gbps | $116.99/季 · $219.99/半年 · $399.99/年 | [购买 40G SLA](https://bwh81.net/aff.php?aff=77528&pid=165) |
| 80G SLA (pid=166) | 4 核 | 4 GB | 80 GB | 3 TB | 2.5 Gbps | $69.99/月 · $199.99/季 · $379.99/半年 · $699.99/年 | [购买 80G SLA](https://bwh81.net/aff.php?aff=77528&pid=166) |
| 160G SLA (pid=167) | 6 核 | 8 GB | 160 GB | 5 TB | 5 Gbps | $109.99/月 · $299.99/季 · $569.99/半年 · $1099.99/年 | [购买 160G SLA](https://bwh81.net/aff.php?aff=77528&pid=167) |
| 320G SLA (pid=168) | 8 核 | 16 GB | 320 GB | 8 TB | 5 Gbps | $199.99/月 · $569.99/季 · $1079.99/半年 · $1999.99/年 | [购买 320G SLA](https://bwh81.net/aff.php?aff=77528&pid=168) |
| 640G SLA (pid=169) | 10 核 | 32 GB | 640 GB | 10 TB | 10 Gbps | $369.99/月 · $1055.99/季 · $1999.99/半年 · $3699.99/年 | [购买 640G SLA](https://bwh81.net/aff.php?aff=77528&pid=169) |
| 1280G SLA (pid=170) | 12 核 | 64 GB | 1280 GB | 12 TB | 10 Gbps | $699.99/月 · $1989.99/季 · $3779.99/半年 · $6999.99/年 | [购买 1280G SLA](https://bwh81.net/aff.php?aff=77528&pid=170) |
| 1280G SLA HIBW 15T (pid=171) | 12 核 | 64 GB | 1280 GB | 15 TB | 10 Gbps | $879.99/月 · $2509.99/季 · $4768.99/半年 · $8799.99/年 | [购买 1280G SLA 15T](https://bwh81.net/aff.php?aff=77528&pid=171) |
| 1280G SLA HIBW 20T (pid=172) | 12 核 | 64 GB | 1280 GB | 20 TB | 10 Gbps | $1159.99/月 · $3299.99/季 · $6269.99/半年 · $11598.99/年 | [购买 1280G SLA 20T](https://bwh81.net/aff.php?aff=77528&pid=172) |

### Ultra VPS(香港 / 东京 / 大阪 / 新加坡 CN2 GIA)

| 套餐 | CPU | RAM | SSD | 月流量 | 带宽 | 起价(月付) | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 40G 香港 CN2 GIA (pid=95) | 2 核 | 2 GB | 40 GB | 500 GB | 1 Gbps | $89.99/月 · $899.99/年 | [购买 40G 香港](https://bwh81.net/aff.php?aff=77528&pid=95) |
| 80G 香港 CN2 GIA (pid=96) | 4 核 | 4 GB | 80 GB | 1 TB | 1 Gbps | $155.99/月 · $1559.99/年 | [购买 80G 香港](https://bwh81.net/aff.php?aff=77528&pid=96) |
| 160G 香港 CN2 GIA (pid=97) | 6 核 | 8 GB | 160 GB | 2 TB | 1 Gbps | $299.99/月 · $2999.99/年 | [购买 160G 香港](https://bwh81.net/aff.php?aff=77528&pid=97) |
| 320G 香港 CN2 GIA (pid=98) | 8 核 | 16 GB | 320 GB | 4 TB | 1 Gbps | $589.99/月 · $5899.99/年 | [购买 320G 香港](https://bwh81.net/aff.php?aff=77528&pid=98) |
| 640G 香港 CN2 GIA (pid=122) | 10 核 | 32 GB | 640 GB | 6 TB | 1 Gbps | $989.99/月 · $9989.99/年 | [购买 640G 香港](https://bwh81.net/aff.php?aff=77528&pid=122) |
| 1280G 香港 CN2 GIA (pid=124) | 12 核 | 64 GB | 1280 GB | 8 TB | 1 Gbps | $1889.99/月 · $18989.99/年 | [购买 1280G 香港](https://bwh81.net/aff.php?aff=77528&pid=124) |
| 40G 东京 CN2 GIA (pid=108) | 2 核 | 2 GB | 40 GB | 500 GB | 1.2 Gbps | $89.99/月 · $899.99/年 | [购买 40G 东京](https://bwh81.net/aff.php?aff=77528&pid=108) |
| 80G 东京 CN2 GIA (pid=109) | 4 核 | 4 GB | 80 GB | 1 TB | 1.2 Gbps | $155.99/月 · $1559.99/年 | [购买 80G 东京](https://bwh81.net/aff.php?aff=77528&pid=109) |
| 160G 东京 CN2 GIA (pid=110) | 6 核 | 8 GB | 160 GB | 2 TB | 1.2 Gbps | $299.99/月 · $2999.99/年 | [购买 160G 东京](https://bwh81.net/aff.php?aff=77528&pid=110) |
| 320G 东京 CN2 GIA (pid=111) | 8 核 | 16 GB | 320 GB | 4 TB | 1.2 Gbps | $589.99/月 · $5899.99/年 | [购买 320G 东京](https://bwh81.net/aff.php?aff=77528&pid=111) |
| 640G 东京 CN2 GIA (pid=123) | 10 核 | 32 GB | 640 GB | 6 TB | 1.2 Gbps | $989.99/月 · $9989.99/年 | [购买 640G 东京](https://bwh81.net/aff.php?aff=77528&pid=123) |
| 1280G 东京 CN2 GIA (pid=125) | 12 核 | 64 GB | 1280 GB | 8 TB | 1.2 Gbps | $1889.99/月 · $18989.99/年 | [购买 1280G 东京](https://bwh81.net/aff.php?aff=77528&pid=125) |
| 40G 大阪 CN2 GIA (pid=134) | 2 核 | 2 GB | 40 GB | 500 GB | 1.5 Gbps | $49.99/月 · $499.99/年 | [购买 40G 大阪](https://bwh81.net/aff.php?aff=77528&pid=134) |
| 80G 大阪 CN2 GIA (pid=135) | 4 核 | 4 GB | 80 GB | 1 TB | 1.5 Gbps | $86.99/月 · $869.99/年 | [购买 80G 大阪](https://bwh81.net/aff.php?aff=77528&pid=135) |
| 160G 大阪 CN2 GIA (pid=136) | 6 核 | 8 GB | 160 GB | 2 TB | 1.5 Gbps | $165.99/月 · $1665.99/年 | [购买 160G 大阪](https://bwh81.net/aff.php?aff=77528&pid=136) |
| 320G 大阪 CN2 GIA (pid=137) | 8 核 | 16 GB | 320 GB | 4 TB | 1.5 Gbps | $329.99/月 · $3199.00/年 | [购买 320G 大阪](https://bwh81.net/aff.php?aff=77528&pid=137) |
| 640G 大阪 CN2 GIA (pid=138) | 10 核 | 32 GB | 640 GB | 6 TB | 1.5 Gbps | $549.99/月 · $5549.99/年 | [购买 640G 大阪](https://bwh81.net/aff.php?aff=77528&pid=138) |
| 1280G 大阪 CN2 GIA (pid=139) | 12 核 | 64 GB | 1280 GB | 8 TB | 1.5 Gbps | $1059.99/月 · $10559.99/年 | [购买 1280G 大阪](https://bwh81.net/aff.php?aff=77528&pid=139) |
| 40G 新加坡 CN2 GIA (pid=173) | 2 核 | 2 GB | 40 GB | 500 GB | 1.5 Gbps | $49.99/月 · $499.99/年 | [购买 40G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=173) |
| 80G 新加坡 CN2 GIA (pid=174) | 4 核 | 4 GB | 80 GB | 1 TB | 1.5 Gbps | $86.99/月 · $869.99/年 | [购买 80G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=174) |
| 160G 新加坡 CN2 GIA (pid=175) | 6 核 | 8 GB | 160 GB | 2 TB | 2.5 Gbps | $165.99/月 · $1665.99/年 | [购买 160G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=175) |
| 320G 新加坡 CN2 GIA (pid=176) | 8 核 | 16 GB | 320 GB | 4 TB | 2.5 Gbps | $329.99/月 · $3199.00/年 | [购买 320G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=176) |
| 640G 新加坡 CN2 GIA (pid=177) | 10 核 | 32 GB | 640 GB | 6 TB | 5 Gbps | $549.99/月 · $5549.99/年 | [购买 640G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=177) |
| 1280G 新加坡 CN2 GIA (pid=178) | 12 核 | 64 GB | 1280 GB | 8 TB | 5 Gbps | $1059.99/月 · $10559.99/年 | [购买 1280G 新加坡](https://bwh81.net/aff.php?aff=77528&pid=178) |

> 表格里所有购买链接都通过 `aff.php?aff=77528&pid=产品ID` 的形式指向对应套餐的购物车页面,联盟追踪参数已保留,点击后 cookie 会正常写入,优惠码在结账时手动叠加。

## 五、怎么选:三个典型场景

**场景 A:个人建站 / 博客 / 小项目,预算有限**
直接选 Basic 的 20G KVM PROMO(pid=44),$49.99/年 + `BWHCGLUKKB` 折后约 $46.60/年。1TB 流量对个人站绰绰有余,机房选洛杉矶 USCA_2 或纽约 USNY_6 都行。缺点是没有 CN2 GIA,中国方向访问会绕普通线路,延迟和晚高峰丢包会比较明显。

**场景 B:面向中国访客的电商 / 跨境业务 / 远程办公**
选 CN2 GIA-E 的 20G(pid=87)或 40G(pid=88)。20G 季付 $49.99 起,40G 年付 $299.99,三网 CN2 GIA + 2.5Gbps 带宽,机房选洛杉矶 USCA_9(容量最大、稳定性最好)。这是搬瓦工性价比最高的"中国优化"方案,比香港 Ultra 便宜一个量级,延迟多 50–80ms 但稳定性差距不大。👉 [查看 CN2 GIA-E 全部套餐](https://bwh81.net/aff.php?aff=77528&gid=1)

**场景 C:不能停机的生产业务 / 合规要求 SLA**
选 E-Commerce+SLA 的 80G(pid=166)或 160G(pid=167),99.99% SLA + 双路冗余,机房固定在 USCA_5。比同档普通 E-Commerce 贵约 25–30%,换来的是合同里能写进去的可用性承诺。

**场景 D:延迟敏感(游戏服 / 实时音视频 / 金融)**
香港 Ultra 的 40G(pid=95)起步 $89.99/月,东京/大阪/新加坡同档价格接近。香港延迟最低但带宽只有 1Gbps;大阪和新加坡 1.5Gbps,价格反而比香港便宜(40G 大阪 $49.99/月 vs 香港 $89.99/月)。如果业务对延迟敏感但对带宽要求不高,**大阪是 Ultra 里性价比最高的选择**。

## 六、下单流程与优惠码使用

1. 通过上面的套餐链接进入对应产品页(联盟 cookie 自动写入)。
2. 选机房和计费周期,点 "Order Now" 进购物车。
3. 在 "Promotional Code" 框输入 `BWHCGLUKKB`,点 "Validate Code"。如果显示无效,依次试 `ireallyreadtheterms8`、`BWHWYWWYVY`、`ireadtheterms8`。
4. 确认折后价,注册账号(支持支付宝、PayPal、信用卡),完成支付。
5. 开通后进 KiwiVM 面板,可随时免费迁移机房、重装系统(支持 AlmaLinux、RockyLinux、CentOS、Debian、Ubuntu、Fedora)、做快照和自动备份。

> 30 天退款政策适用于新购套餐,续费和升级不在退款范围内。优惠码是循环的,续费时自动套用,不用重输。

## 七、几个常被问到的问题

**优惠码会失效吗?** 会。搬瓦工历史上多次出现"所有公开码失效"的窗口期,通常会随后放出新的限时码(如 `NODESEEK2026`)。下单前在结账页实测是最可靠的方式。

**CN2 GIA-E 和香港 Ultra 差距大吗?** 洛杉矶 CN2 GIA-E 到中国延迟约 150–180ms,香港约 30–50ms。日常建站、跨境电商选 GIA-E 完全够用;只有实时性要求高的业务才需要为香港的延迟多付 5–10 倍价格。

**能升级套餐吗?** 可以,在 KiwiVM 面板内升级,差价按比例计算,优惠码同样适用。降级不支持。

**支持 IPv6 吗?** 全部套餐包含 1 个独立 IPv4 + 一个 /64 的 IPv6 段,rDNS 在面板里自助修改。

**有 DDoS 防护吗?** Basic 和 E-Commerce 走的是普通防护;CN2 GIA 线路本身对 DDoS 容量有限,严重攻击会被 nullroute。如果业务面临持续攻击风险,需要考虑专门的防护方案,不是搬瓦工的强项。
