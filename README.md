# nuaa-card-key
！！@请合法使用，不要违反法律与校规，本人仅为技术研究，一切由于违法使用本项目的行为造成的后果与本人无关@！！  
1.本校卡片扇区加密分析：  
（1）用MCT使用预设密码ffffffffffff读取，发现567三区未加密，尝试用知一密破解（nested），失败，此卡修复了嵌套攻击漏洞。  
（2）在尝试中我使用了hardnested，再结合之前的扇区扫描，发现0-4区A密钥是经过更改的，B密钥为默认ffffffffffff，8，9，10三区ab都加了密，11-15只加了a的密  
（3）hardnested一晚上。。。。。计算出了密钥  
（4）然后使用该密钥尝试了朋友的卡，发现四扇区的a密钥需单独计算，每个人不一样。  
# 扇区信息分布  
0区：卡号及厂商标识  
1区：？？？未知？？？（待探索）  
2区：加密扇区，但是无信息  
3区：？？？未知？？？（待探索）  
4区：在线式洗浴子钱包     
5区：未加密  
6区：未加密  
7区：未加密  
8区：饭卡金额  
9区：？？？未知？？？（待探索）   
10区：？？？未知？？？（待探索）   
11区：加密扇区，但是无信息  
12区：离线式热水饮水机（每一楼都有那个)  
13区：加密扇区，但是无信息    
14区：加密扇区，但是无信息  
15区：加密扇区，但是无信息  
...待续...
