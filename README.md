






##   🌵Brief introduction
PanguSync is a cross platform database synchronization software that can run on Windows/Linux. It has created a database incremental synchronization technology that not only solves the high energy consumption and high latency of full comparison software, but also avoids the complex configuration of logging software. It does not require CDC/Binlog to obtain SQL server/MySQL incremental changes (insert, update, delete) in milliseconds. On this basis, multiple synchronization modes are adapted, supporting bidirectional [A ⇆ B], broadcast [A → B, A → C], and chain [A → B → C]. In order to ensure supreme stability, functions such as self increasing primary key error correction, bidirectional reflux blocking, unique constraint error correction, foreign key constraint error correction, and segment detection mapping are built-in.



### 🔥Incremental synchronization case
https://www.bilibili.com/video/BV1TmvPz8EhF/?vd_source=8db0f4c511ee648e595718cb636c8df7


### 📟Interface
#### PanguSync 10.0 for Windows
<img src="主界面.png">

#### PanguSync 1.3 for Linux(Ubuntu)
<img src="Ubuntu运行效果.png">

#### PanguSync 1.3 for Linux(CentOS)
<img src="CentOS运行效果.png">

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


### 🔰How to register
After making payment through [PayPal](https://paypal.me/hotstandby), send the payment record and Hardware ID  to the email 435031783@qq.com, After receiving the registration code, you can register on your own<br>
<img width="400" height="320" alt="5a7518ea-094a-4f1e-92bb-61ecfa3c8ec5" src="https://github.com/user-attachments/assets/0755f569-65f5-439f-ba5e-7c922acb05f1" />
<img width="400" height="320" alt="03bc9da8-42c9-43b2-8279-8dfb9ef1a640" src="https://github.com/user-attachments/assets/4ec7614e-721a-4719-a3fe-e05825f722b0" />


### ☀️Purchase

|   | Trial |v1| v2| v3  | v4 | Professional| Supreme | 
|---|---|---|---|---|---|---|---|
|  **Price** |  **free**   | **$49**| **$82**| **$96** |**$126** | **$155** |  **$184**  | 
| **Task Num**|  2 | 10|50| 100 | 300| 500 |  Unlimited |
| **Authorization Period**|  1 hour each time<br>(Unlimited trial) |  forever |  forever | forever |forever |forever |forever |















