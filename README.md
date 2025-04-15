

![主界面](https://github.com/user-attachments/assets/0dabde5c-630e-47a5-8d04-f5927bc755be)


##   🌵Brief introduction
PanguSync has developed a new database incremental synchronization technology that addresses the drawbacks of high latency and energy consumption in full volume comparison software, as well as the complex configuration of log software. This technology has the advantages of easy configuration, low latency, low energy consumption, and high error tolerance. Once the source changes, it can be synchronized to the target in near real time, suitable for applications with daily increments of around tens of millions. Once Mysql/SQL Server database synchronization enthusiasts use this software, they will feel like they have found a treasure, just like a cultivator obtaining an extremely low threshold advanced cultivation technique.

##  ☀️Buy
- Purchase method: WeChat【vicecity2】, [Paypal](https://www.paypal.com/paypalme/hotstandby?country.x=C2)
- One machine, one code
- Send the hardware id and payment record via email【435031783@qq.com】 to receive the registration code

|  |Trial|Play|Professional | Enterprise  | Supreme|
|---|---|---|---|---|---|
|  Price of $\color{red}{1}$ registration code| Free  | **$150** |  **$300**|   **$450**|   **$500**  |
| Number of tasks |  5   |50   |500   |  2000  |   no limit  |
|Authorization period| 2 hours per session (unlimited number of times) | no limit  | no limit   |  no limit |  no limit  | 

### Cloud film hot backup case in a tertiary hospital ($\color{red}{one}$ $\color{red}{hundred}$ $\color{red}{million}$  $\color{red}{level}$) https://www.bilibili.com/video/BV14x4y167A2/?spm_id_from=333.999.0.0&vd_source=8db0f4c511ee648e595718cb636c8df7


### 🔰How to register (without internet connection)
**When purchasing, send me the hardware id via email【435031783@qq.com】. After receiving the registration code, fill it in the text box and click register** 
<br><img src="https://github.com/user-attachments/assets/004de983-6ffe-4397-9d0c-22c5ada45e73" width="400px"> 
<img src="https://github.com/user-attachments/assets/84f9a2b3-2bec-43ec-a35a-8ebda68872e6" width="400px"> 



### 💪Core advantages
- ♋️Diverse synchronized postures
- 💦Rookie 3 seconds to get started
- 👢Automatically handle the misalignment of self increasing primary keys on the target end
- 🔒Automatically handle foreign key constraint conflicts (both parent and child tables require configuration tasks)
- 🔑Automatically handle unique key or unique index conflicts (for databases of the same type)
- 📈Support breakpoint continuation


### 🔯Synchronous mode

| Mode| Example |Support| Applicable scenarios| Precautions|
|---|---|---|---|---|
| one-way| A➔B |✔️  |A Write B Read|/|
| two-way|A⇆B|✔️  |Data dual machine hot backup [non dual write scenario]| Please uncheck 'Special Mode' in the editing interface|
|  broadcast|A➔B，A➔C，...，A➔Z|✔️  |A write N read|/|
| Chain type| A➔B➔C➔......➔Z |✔️  |A write N read|Please check 'Special Mode' in the editing interface|
| Chain extension| ![输入图片说明](%E5%8D%95%E5%90%91%E6%A0%91%E5%BD%A2.png) |✔️  |A write N read|Please check 'Special Mode' in the editing interface|



### 🔧配置项说明 Configuration item description
|  配置项 | 说明  |
|---|---|
|  筛选条件<br>Condition | 设置where条件后，源端新增、更新变化会先根据where条件进行筛选，符合条件的会同步到目标端，删除变化不进行where筛选<br>After setting the 'where' condition, new and updated changes on the source end will be filtered based on the 'where' condition first. Those that meet the condition will be synchronized to the target end, and changes that are deleted will not be filtered by the 'where' condition  |
|  特殊模式 <br>Special Mode|勾选特殊模式后，可支持链式同步，比如A➔B➔C，需要部署两个任务A➔B、B➔C，然后在A➔B任务中勾选特殊模式，即可实现A➔B➔C，即A的变化可以传递到B的下游，若后续有A➔B➔C➔D的规划，则B➔C任务中也可以提前勾选特殊模式，即B的变化可以传递到C的下游<br>After selecting the special mode, chain synchronization can be supported, such as A ➔ B ➔ C, where two tasks A ➔ B and B ➔ C need to be deployed. Then, selecting the special mode in the A ➔ B task can achieve A ➔ B ➔ C, where changes in A can be transmitted downstream of B. If there are plans for A ➔ B ➔ C ➔ D in the future, special mode can also be selected in advance in the B ➔ C task, where changes in B can be transmitted downstream of C|
|  字段检测 <br>Check columns|勾选字段检测后，源【新增字段】【修改字段】【删除有映射关系的字段】后，同步任务会自动停止，需要人工再次确认编辑，这样做是为了安全考量，防止新字段数据同步丢失。如果不考虑新字段的同步，即只需按初次配置的映射关系进行同步，则可以不勾选此项，后续源【新增字段】【删除无映射关系的字段】都不会导致任务的停止，但是源【复合主键变化】、【删除有映射关系的字段】依然会停止同步，需要人工再次确认编辑，这是处于安全的考量<br>After selecting 'check columns', the synchronization task will automatically stop when the source 'Add Columns'、'Modify Columns'、'Delete Columns with Mapping Relationship'. It is necessary to manually confirm the editing again for security reasons and to prevent the loss of data synchronization for new columns. If the synchronization of new fields is not considered, that is, only the mapping relationship configured for the first time needs to be synchronized, then this option can be left unchecked. Subsequent source 'adding columns' and 'deleting columns without mapping relationships' will not cause the task to stop, but source 'compound primary key changes' and 'deleting columns with mapping relationships' will still stop synchronizing and require manual confirmation and editing. This is for security reasons  |
|  字段映射<br> field mapping| 该选项仅在源和目标是同类型数据库的情况下生效。勾选该选项后，可以实现字段自动映射功能而无需重新编辑任务，比如同步任务A➔B，A中添加一个新字段Column1后，只需要在B中也添加相同名称的字段Column1，即可实现新字段的同步。如果源和目标字段完全一样，则建议勾选此项。如果源和目标字段名称大多数不一样，则不建议勾选此项，避免源新增字段名称刚好和目标的某个字段名称一样，就自动映射了，但也许这个字段你并不想映射到目标的同名字段<br>This option only takes effect when the source and target are databases of the same type. After selecting this option, the automatic field mapping function can be achieved without the need for re editing tasks, such as synchronizing tasks A to B. After adding a new field Column1 in A, only the same named field Column1 needs to be added in B to achieve synchronization of the new field. If the source and target fields are exactly the same, it is recommended to check this option. If the source and target field names are mostly different, it is not recommended to check this option to avoid the automatic mapping of newly added field names in the source that happen to be the same as a field name in the target. However, you may not want to map this field to a field with the same name in the target |


### 🌎全局参数 Global parameters
|  参数| 说明  |
|---|---|
|  增量获取行数 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>Incremental get rows| 每个周期内获取的最大源变化行数，默认2000<br>The maximum number of source change rows obtained in each cycle, default to 2000 |

### 📢注意事项 Precautions
- 👿不建议开杀毒实时防控，可能会影响性能 It is not recommended to enable real-time antivirus prevention and control, as it may affect performance
- ⚡️选库不选表可批量生成任务 Batch generation tasks can be generated by selecting only the database and not the table
- 🔄【A⇆B】模式部署步骤：假设A为主节点，B为备节点，先truncate清空B节点(不要使用delete)，新建B➔A的任务，待运行成功后，再新建A➔B的任务运行，等待A➔B全量同步完成，后续进行增量同步。另外一种方法就是通过备份还原使两边初始数据完全一致，也是先部署B➔A，再部署A➔B，然后参考【[**如何跳过初始数据直接进行增量同步**](https://blog.csdn.net/sss899000/article/details/146609891)】【 A ⇆ B 】 Mode deployment steps: Assuming A is the primary node and B is the backup node, first truncate and clear B node (do not use delete), create a new task for B ➔ A, wait for it to run successfully, then create a new task for A ➔ B to run, wait for A ➔ B to complete full synchronization, and then perform incremental synchronization. Another method is to make the initial data on both sides completely consistent through backup and restoration. This involves deploying B ➔ A first, then A ➔ B, and referring to article 【[**How to skip initial data and perform incremental synchronization directly**](https://blog.csdn.net/sss899000/article/details/146609891)】
- 🍨初次部署会进行全量同步，如果表多以及数据量大会占用一定资源，可通过【同步周期】和【睡眠时间】来调节，等全量同步完再恢复原来的参数，或者参考【[**如何跳过初始数据直接进行增量同步**](https://blog.csdn.net/sss899000/article/details/146609891)】  The initial deployment will perform full synchronization. If there are too many tables and the amount of data will occupy a certain amount of resources, it can be adjusted through the synchronization period and sleep time. After the full synchronization is completed, the original parameters can be restored, or refer to Article 【[**How to skip initial data and perform incremental synchronization directly**](https://blog.csdn.net/sss899000/article/details/146609891)】





### ㊙️关于开机自启动 Regarding the self startup upon startup
- 将软件设置为快捷方式，然后Win+R输入shell:startup，将快捷方式拖入该目录 Set the software as a shortcut, then [Win+R] enter [shell: startup] and drag the shortcut into the directory
- Win+R输入control userpasswords2，取消【要使用本计算机，用户必须输入用户名和密码】Win+R input control 'userpasswords2', cancel 'To use this computer, the user must enter a username and password'
- 付费版可以自动运行任务，在Config文件夹下面添加一个AutoStart.txt文件即可 The paid version can automatically run tasks. Simply add an AutoStart.txt file to the 'Config' folder
















