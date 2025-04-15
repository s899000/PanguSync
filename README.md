

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



### 🔧Configuration item description
|  configuration items | describe  |
|---|---|
|  Condition |After setting the 'where' condition, new and updated changes on the source end will be filtered based on the 'where' condition first. Those that meet the condition will be synchronized to the target end, and changes that are deleted will not be filtered by the 'where' condition  |
|  Special Mode|After selecting the special mode, chain synchronization can be supported, such as A ➔ B ➔ C, where two tasks A ➔ B and B ➔ C need to be deployed. Then, selecting the special mode in the A ➔ B task can achieve A ➔ B ➔ C, where changes in A can be transmitted downstream of B. If there are plans for A ➔ B ➔ C ➔ D in the future, special mode can also be selected in advance in the B ➔ C task, where changes in B can be transmitted downstream of C|
|  Check columns|After selecting 'check columns', the synchronization task will automatically stop when the source 'Add Columns'、'Modify Columns'、'Delete Columns with Mapping Relationship'. It is necessary to manually confirm the editing again for security reasons and to prevent the loss of data synchronization for new columns. If the synchronization of new fields is not considered, that is, only the mapping relationship configured for the first time needs to be synchronized, then this option can be left unchecked. Subsequent source 'adding columns' and 'deleting columns without mapping relationships' will not cause the task to stop, but source 'compound primary key changes' and 'deleting columns with mapping relationships' will still stop synchronizing and require manual confirmation and editing. This is for security reasons  |
|   field mapping| This option only takes effect when the source and target are databases of the same type. After selecting this option, the automatic field mapping function can be achieved without the need for re editing tasks, such as synchronizing tasks A to B. After adding a new field Column1 in A, only the same named field Column1 needs to be added in B to achieve synchronization of the new field. If the source and target fields are exactly the same, it is recommended to check this option. If the source and target field names are mostly different, it is not recommended to check this option to avoid the automatic mapping of newly added field names in the source that happen to be the same as a field name in the target. However, you may not want to map this field to a field with the same name in the target |


### 🌎Global parameters
|  parameters| describe  |
|---|---|
| Incremental get rows| The maximum number of source change rows obtained in each cycle, default to 2000 |

### 📢Precautions
- 👿It is not recommended to enable real-time antivirus prevention and control, as it may affect performance
- ⚡️Batch generation tasks can be generated by selecting only the database and not the table
- 🔄【 A ⇆ B 】 Mode deployment steps: Assuming A is the primary node and B is the backup node, first truncate and clear B node (do not use delete), create a new task for B ➔ A, wait for it to run successfully, then create a new task for A ➔ B to run, wait for A ➔ B to complete full synchronization, and then perform incremental synchronization. 
- 🍨The initial deployment will perform full synchronization. If there are too many tables and the amount of data will occupy a certain amount of resources, it can be adjusted through the synchronization period and sleep time. After the full synchronization is completed, the original parameters can be restored





### ㊙️Regarding the self startup upon startup
- Set the software as a shortcut, then [Win+R] enter [shell: startup] and drag the shortcut into the directory
- Win+R input 'control userpasswords2', cancel 'To use this computer, the user must enter a username and password'
- The paid version can automatically run tasks. Simply add an AutoStart.txt file to the 'Config' folder
















