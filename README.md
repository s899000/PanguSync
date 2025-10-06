


<img src="主界面.png">



##   🌵Brief introduction
PanguSync has created a database incremental synchronization technology that not only solves the high energy consumption and high latency of full comparison software, but also avoids the complex configuration of logging software. It does not require CDC/Binlog to obtain SQL server/MySQL incremental changes (insert, update, delete) in milliseconds. On this basis, multiple synchronization modes are adapted, supporting bidirectional [A ⇆ B], broadcast [A → B, A → C], and chain [A → B → C]. In order to ensure supreme stability, functions such as self increasing primary key error correction, bidirectional reflux blocking, unique constraint error correction, foreign key constraint error correction, and segment detection mapping are built-in.



### 🔥Incremental synchronization case
https://www.bilibili.com/video/BV1TmvPz8EhF/?vd_source=8db0f4c511ee648e595718cb636c8df7




### 🔯Synchronous mode

| Mode| Example |Support| Applicable scenarios| Precautions|
|---|---|---|---|---|
| one-way| A➔B |✔️  |A Write B Read|/|
| two-way|A⇆B|✔️  |Data dual machine hot backup [non dual write scenario]| Please uncheck 'Special Mode' in the editing interface|
|  broadcast|A➔B，A➔C，...，A➔Z|✔️  |A write N read|/|
| Chain type| A➔B➔C➔......➔Z |✔️  |A write N read|Please check 'Special Mode' in the editing interface|
| Chain extension| <img src="单向树形.png"> |✔️  |A write N read|Please check 'Special Mode' in the editing interface|





### ㊙️Regarding the self startup upon startup
- Set the software as a shortcut, then [Win+R] enter [shell: startup] and drag the shortcut into the directory
- Win+R input 'control userpasswords2', cancel 'To use this computer, the user must enter a username and password'
- The paid version can automatically run tasks. Simply add an AutoStart.txt file to the 'Config' folder



### 🔰License Purchase

|   | Trial |v1| v2| v3  | v4 | Professional| Supreme | 
|---|---|---|---|---|---|---|---|
|  **Price** |  **free**   | **$49**| **$82**| **$96** |**$126** | **$155** |  **$184**  | 
| **Task Num**|  2 | 10|50| 100 | 300| 500 |  Unlimited |
| **Authorization Period**|  1 hour each time<br>(Unlimited trial) |  forever |  forever | forever |forever |forever |forever |

### Paypal
https://paypal.me/hotstandby

### Email
435031783@qq.com











