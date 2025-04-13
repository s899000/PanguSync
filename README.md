

![主界面](https://github.com/user-attachments/assets/0dabde5c-630e-47a5-8d04-f5927bc755be)


##   🌵简介 Brief introduction
针对全量比对型软件的高延迟高能耗、日志型软件的配置复杂等缺点，PanguSync独创了一种新型数据库增量同步技术，具备易配置、低延迟、低能耗、高容错等优点。源一旦发生变化，可准实时同步到目标，适合日增量在千万级左右的应用。Mysql/Sqlserver数据库同步爱好者一旦使用该软件，将如获至宝，就如修行者获得了一本门槛极低的高等修行功法。

PanguSync has developed a new database incremental synchronization technology that addresses the drawbacks of high latency and energy consumption in full volume comparison software, as well as the complex configuration of log software. This technology has the advantages of easy configuration, low latency, low energy consumption, and high error tolerance. Once the source changes, it can be synchronized to the target in near real time, suitable for applications with daily increments of around tens of millions. Once Mysql/SQL Server database synchronization enthusiasts use this software, they will feel like they have found a treasure, just like a cultivator obtaining an extremely low threshold advanced cultivation technique.

##  ☀️爽快人购买 Buy
1. 购买方式：微信【vicecity2】、支付宝、银行卡、淘宝 
2. 可签[**合同**](https://pan.baidu.com/s/1U7jMJv-76q36T6diGwAVug?pwd=abcd#list/path=%2F)，可开[**发票**](https://pan.baidu.com/s/1U7jMJv-76q36T6diGwAVug?pwd=abcd#list/path=%2F)
3. 一机一码


|  |试用版|体验版|专业版 | 企业版  | 至尊版 |
|---|---|---|---|---|---|
| **$\color{red}{1}$个注册码售价**  |免费 | **￥499**<br> $\color{blue}{联系微信购买 }$   |  **￥1000** <br>[**[购买]**](https://item.taobao.com/item.htm?ft=t&id=754824495442)|   **￥1500** <br>[**[购买]**](https://item.taobao.com/item.htm?id=761877111372)|   **￥1600** <br> [**[购买]**](https://item.taobao.com/item.htm?ft=t&id=767418824294) |
| 任务数量 |  5   |50   |500   |  2000  | 不限|
|授权期限|   2h/次（次数不限） |  终生 &nbsp;&nbsp;&nbsp;&nbsp;  | 终生  &nbsp;&nbsp;&nbsp;&nbsp;  |  终生  &nbsp;&nbsp;&nbsp;&nbsp; |  终生  &nbsp;&nbsp;&nbsp;&nbsp; | 
 

- Purchase method: WeChat【vicecity2】, [Paypal](https://www.paypal.com/paypalme/hotstandby?country.x=C2)
- One machine, one code
- Send the hardware id and payment record via email【435031783@qq.com】 to receive the registration code

|  |Trial|Play|Professional | Enterprise  | Supreme|
|---|---|---|---|---|---|
|  Price of $\color{red}{1}$ registration code| Free  | **$150** |  **$300**|   **$450**|   **$500**  |
| Number of tasks |  5   |50   |500   |  2000  |   no limit  |
|Authorization period| 2 hours per session (unlimited number of times) | no limit  &nbsp;&nbsp;&nbsp;&nbsp;  | no limit  &nbsp;&nbsp;&nbsp;&nbsp;  |  no limit  &nbsp;&nbsp;&nbsp;&nbsp; |  no limit  &nbsp;&nbsp;&nbsp;&nbsp; | 


### 🔥某三甲医院云胶片热备案例($\color{red}{亿级}$)https://www.bilibili.com/video/BV14x4y167A2/?spm_id_from=333.999.0.0&vd_source=8db0f4c511ee648e595718cb636c8df7





### 🔰如何注册(无需联网) How to register (without internet connection)
 **购买时提供硬件序列号，收到注册码后，在文本框内填入，点击注册** 
<br><img src="序列号.png" width="400px"/> <img src="注册码.png" width="400px"  />








### 💪核心优势 Core advantages
- ♋️同步姿势多样
- 💦小白3秒上手
- 👢自动处理目标端自增主键错位
- 🔒自动处理外键约束冲突(父子表都需要配置任务)
- 🔑自动处理唯一键或唯一索引冲突(同类型数据库)
- 📈支持断点续传





 ### 📜教程 Tutorial
- 🔥[**_PanguSync,一款windows数据库同步软件_**](https://zhuanlan.zhihu.com/p/680995986)
- 🔥[**_一款超好用的增量数据准实时同步工具PanguSync_**](https://zhuanlan.zhihu.com/p/686039921)
- 👪[**_一主多从同步教程_**](https://blog.csdn.net/sss899000/article/details/146512375)
- 🌈[**_PanguSync常见错误解决方法_**](https://blog.csdn.net/sss899000/article/details/139549129)
- 🚴[**_如何跳过初始数据直接进行增量同步_**](https://blog.csdn.net/sss899000/article/details/146609891)
- 👫[**_关于字段自动映射功能的说明_**](https://blog.csdn.net/sss899000/article/details/146909189)









### 🔯同步模式 Synchronous mode

| 模式| 示例 |支持|适用场景| 注意事项 |
|---|---|---|---|---|
| 单向| A➔B |✔️  |A写B读|/|
| 双向|A⇆B|✔️  |数据双机热备【非双写场景】|编辑界面请❌【特殊模式】|
| 广播|A➔B，A➔C，...，A➔Z|✔️  |A写N读|/|
| 链式| A➔B➔C➔......➔Z |✔️  |A写N读|编辑界面请✔️【特殊模式】|
| 链式扩展| ![输入图片说明](%E5%8D%95%E5%90%91%E6%A0%91%E5%BD%A2.png) |✔️  |A写N读|编辑界面请✔️【特殊模式】|



### 🔧配置项说明 Configuration item description
|  配置项 | 说明  |
|---|---|
|  where条件 | 设置where条件后，源端新增、更新变化会先根据where条件进行筛选，符合条件的会同步到目标端，删除变化不进行where筛选  |
|  特殊模式  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|勾选特殊模式后，可支持链式同步，比如A➔B➔C，需要部署两个任务A➔B、B➔C，然后在A➔B任务中勾选特殊模式，即可实现A➔B➔C，即A的变化可以传递到B的下游，若后续有A➔B➔C➔D的规划，则B➔C任务中也可以提前勾选特殊模式，即B的变化可以传递到C的下游|
|  字段检测|勾选字段检测后，源【新增字段】【修改字段】【删除有映射关系的字段】后，同步任务会自动停止，需要人工再次确认编辑，这样做是为了安全考量，防止新字段数据同步丢失。如果不考虑新字段的同步，即只需按初次配置的映射关系进行同步，则可以不勾选此项，后续源【新增字段】【删除无映射关系的字段】都不会导致任务的停止，但是源【复合主键变化】、【删除有映射关系的字段】依然会停止同步，需要人工再次确认编辑，这是处于安全的考量  |
|  字段映射| 该选项仅在源和目标是同类型数据库的情况下生效。勾选该选项后，可以实现字段自动映射功能而无需重新编辑任务，比如同步任务A➔B，A中添加一个新字段Column1后，只需要在B中也添加相同名称的字段Column1，即可实现新字段的同步。如果源和目标字段完全一样，则建议勾选此项。如果源和目标字段名称大多数不一样，则不建议勾选此项，避免源新增字段名称刚好和目标的某个字段名称一样，就自动映射了，但也许这个字段你并不想映射到目标的同名字段 |


### 🌎全局参数 Global parameters
|  参数| 说明  |
|---|---|
|  增量获取行数 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 每个周期内获取的最大源变化行数，默认2000 |

### 📢注意事项 Precautions
- 👿不建议开杀毒实时防控，可能会影响性能
- ⚡️选库不选表可批量生成任务
- 🔄【A⇆B】模式部署步骤：假设A为主节点，B为备节点，先truncate清空B节点(不要使用delete)，新建B➔A的任务，待运行成功后，再新建A➔B的任务运行，等待A➔B全量同步完成，后续进行增量同步。另外一种方法就是通过备份还原使两边初始数据完全一致，也是先部署B➔A，再部署A➔B，然后参考【[**如何跳过初始数据直接进行增量同步**](https://blog.csdn.net/sss899000/article/details/146609891)】
- 🍨初次部署会进行全量同步，如果表多以及数据量大会占用一定资源，可通过【同步周期】和【睡眠时间】来调节，等全量同步完再恢复原来的参数，或者参考【[**如何跳过初始数据直接进行增量同步**](https://blog.csdn.net/sss899000/article/details/146609891)】





### ㊙️关于开机自启动 Regarding the self startup upon startup
- 将软件设置为快捷方式，然后Win+R输入shell:startup，将快捷方式拖入该目录
- Win+R输入control userpasswords2，取消【要使用本计算机，用户必须输入用户名和密码】
- 付费版可以自动运行任务，在Config文件夹下面添加一个AutoStart.txt文件即可
















