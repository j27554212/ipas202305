# 資訊安全管理 == > ISO 27001:2022  +  CISSP ==> CSSLP
- 1. 資訊安全管理 
  - 1-1.資訊安全管理基本概念
  - 1-2.資訊安全管理系統  == > ISO 27001:2022
  - 1-3.相關法規概論與遵循
  - 1-4.隱私權保護與智慧財產權
- 2. 資產與風險管理
  - 2-1.資產分類分級與盤點
  - 2-2.風險評鑑與風險處理
    - 資通系統風險評鑑參考指引(修訂)v4.1_1101231 
- 3. 存取控制、加解密與金鑰管理
  - 3-1.存取控制與身份認證
    - 身分鑑別與存取控制參考指引v2.0_1111231 
  - 3-2.加解密與金鑰生命週期
- 4. 事故管理與營運持續
  - 4-1.事件與事故管理
  - 4-2.備援
  - 4-3.營運持續
    - 營運持續管理參考指引v2.0_1111231 

## 資訊安全技術概論 == > CEH + Security+ (Network+)  == > OSCP | CHFI
- 1.網路與通訊安全
  - 1-1.網路安全
  - 1-2.通訊安全 
- 2.作業系統與應用程式安全
  - 2-1.作業系統安全(作業系統內建的安全性機制) ==> Windows Security | Linux Security
  - 2-2.作業系統與應用程式 (含資料庫與網頁)攻擊手法 
  - 2-3.程式與開發安全
    - 2-3-1.程式安全
    - 2-3-2.開發安全  SSDLC ==> CSSLP
- 3.資安維運技術
  - 3-1.惡意程式防護與弱點管理
  - 3-2.資料安全及備份管理
  - 3-3.日誌管理
  - 3.4.資安防護技術
- 4.新興科技安全
  - 4-1.雲端安全概論
  - 4-2.行動裝置安全概論
  - 4-3.物聯網安全概論
  
## 1.網路與通訊安全
  - 1-1.網路安全
    - 網路基本知識 ==> OSI vs TCP/IP vs IEEE 802
    - 網路攻擊模式分析
      - 網路協定的攻擊模式分析
        - DNS 的攻擊模式分析
          - [DNS 快取記憶體DNS Poisoning (DNS Spoofing)](https://www.cloudflare.com/zh-tw/learning/dns/dns-cache-poisoning/)
          - [DNS Amplification Attack](https://www.cc.ntu.edu.tw/chinese/epaper/0028/20140320_2808.html) 
        - NTP 的攻擊模式分析
          - [NTP 放大DDoS 攻擊](https://www.cloudflare.com/zh-tw/learning/ddos/ntp-amplification-ddos-attack/)
          - 有關XXXX攻擊的敘述,下列何者正確/錯誤? 
      - 著名的網路攻擊模式分析
        - DDOS
          - 2000年初的DDOS: ping of death, TCP syn flood, smurf attack (icmp flood attack) 
          - HTTP DDOS
        - 社交工程
          - 網路釣魚 (phishing）   
          - 魚叉式網路釣魚（Spear phishing）
          - 變臉詐騙/BEC(Business Email Compromise) 商務電子郵件詐騙
    - 安全的網路技術與協定
      - 應用層
        - https ==> SSL/TLS
        - sftp ftps
        - telnet ==> ssh
        - DNSsec
        - email 安全
      - 網路層
        - IPsec
      - 安全連線
        - ssh
        - VPN     


  - 1-2.通訊安全
    - 無線區域網路(WLAN)
      - [ap(access point)](https://zh.wikipedia.org/wiki/%E7%84%A1%E7%B7%9A%E6%8E%A5%E5%85%A5%E9%BB%9E) 
      - ad hoc mode(Ad-Hoc模式、無線隨意網路) vs infrastrcuture mode(基礎架構模式) 
      - 服務集識別碼(Service Set Identifier，SSID)
      - 獨立基本服務集（IBSS）、基本服務集（BSS）和擴充服務集（ESS）
    - 無線區域網路安全
      - Fake AP
      - 攻擊WEP
         - 有關WEP的敘述下列何者為非?
         - (A)有線等效加密(Wired Equivalent Privacy，WEP）是個保護無線網路資料安全的體制
         - (B)使用RC4串流加密技術達到機密性 ==>(B)使用RC4區塊加密技術達到機密性
         - (c)使用CRC-32 驗和達到資料正確性
         - (D)RC4是流加密的一種，同一個鑰匙絕不能使用二次，所以使用（雖然是用明文傳送的）IV的目的就是要避免重複；然而24位元的IV並沒有長到足以擔保在忙碌的網路上不會重複，而且IV的使用方式也使其可能遭受到關連式鑰匙攻擊
      - 攻擊WPA
      - 攻擊WPA2
      - 攻擊WPA3 

- 2.作業系統與應用程式安全
  - 2-1.作業系統安全
    - windows 作業系統
      - [Windows Authentication](https://docs.microsoft.com/en-us/windows-server/security/windows-authentication/windows-authentication-overview)
      - [Windows 驗證](https://docs.microsoft.com/zh-tw/windows-server/security/windows-authentication/windows-authentication-overview)
      - [NTLM 使用者驗證](https://docs.microsoft.com/zh-tw/troubleshoot/windows-server/windows-security/ntlm-user-authentication)
      - [Kerberos 認證](https://zh.wikipedia.org/wiki/Kerberos)
      - [Security and Protection(舊版)](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831778(v=ws.11)) 
      - 使用者帳戶控制(User Account Control，UAC)
    - windows 作業系統常用指令 [Windows commands](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands)
    - windows 作業系統管理與安全工具
      - task manager
      - event viewer
      - systeminternals 
    - windows server技術:[官方網站](https://docs.microsoft.com/en-us/windows-server/)
      - Active Directory(AD) ==> LDAP
      - Group Policy(GP) ==>  gpedit.msc [Local Group Policy Editor](https://www.isunshare.com/windows-10/5-ways-to-access-local-group-policy-editor-on-windows-10.html)
      - Windows Server Update Services (WSUS)
    - [Windows security眾多文件] (https://docs.microsoft.com/en-us/windows/security/)
      - [Security and Protection(舊版)](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831778(v=ws.11)) 
    - windows 攻擊手法: 
      - Windows binary exploitation 
      - Windows Kernel exploitation
      - 傳遞雜湊(Pass-the-Hash)
      - wannacry 攻擊(2017)
      - 
    - LINUX 作業系統
    - LINUX 作業系統常用指令
    - LINUX 作業系統管理與安全工具
    - LINUX 攻擊手法: 
      - Linux binary exploitation 
      - Linux Kernel exploitation
      - 'root'kit
        - [nurupo/rootkit](https://github.com/nurupo/rootkit)
        - [惡意程式潛伏Linux主機　揪出系統遭植入Rootkit](https://www.netadmin.com.tw/netadmin/zh-tw/technology/F632D1F9D2B34E8B9FCC725B45509BB5) 
        - [f0rb1dd3n/Reptile](https://github.com/f0rb1dd3n/Reptile)
        - [后渗透之Rootkit及入门](https://zhuanlan.zhihu.com/p/132519704)
      - [髒牛漏洞(Dirty Cow)](https://ppfocus.com/0/scbf79101.html)
      - [LES: Linux privilege escalation auditing tool](https://github.com/mzet-/linux-exploit-suggester)
      - [入侵 Linux 系統的慣用姿勢：11 種提權方式揭祕 - 知乎](https://www.gushiciku.cn/pl/p96O/zh-tw)
      
      - [HackerCat](https://www.youtube.com/channel/UCkZAkJWOAExMfVp1XHt1VOA)
      
  - 2-2.作業系統與應用程式 (含資料庫與網頁)攻擊手法
    - 網站安全
    - OWASP TOP 10
      - sqli
        - SQL == Structured Query Language == 結構化查詢語言
      - XSS
        - [XSS DVWA 12 - XSS (Stored) (low/med/high) - Damn Vulnerable Web Application (DVWA)] (https://www.youtube.com/watch?v=P1I9UGpGdrU)
        - [11 - XSS (Reflected) (low/med/high) - Damn Vulnerable Web Application (DVWA)](https://www.youtube.com/watch?v=P1I9UGpGdrU)
    - OWASP API TOP 10
    - 網站安全測試 
    - 資料庫
      - SQL資料庫
      - NOSQL資料庫  
    - 資料庫的攻擊事件
    - 資料庫的攻擊手法
    - 資料庫的安全防護
  - 2-3.程式與開發安全
    - 應用程式(application) secure coding
      - desktop application
      - web application 網站應用程式 客戶端  vs 伺服器端(asp.net)
      - mobile application:  andriod(java  kotlin) ios 
      - [EC-Council CASE .NET應用程式安全工程師認證課程](https://www.uuu.com.tw/Course/Show/1501/EC-Council-CASE-NET%E6%87%89%E7%94%A8%E7%A8%8B%E5%BC%8F%E5%AE%89%E5%85%A8%E5%B7%A5%E7%A8%8B%E5%B8%AB%E8%AA%8D%E8%AD%89%E8%AA%B2%E7%A8%8B)
    - 應用程式的安全威脅
      - 逆向工程
    - 安全程式開發(secure code standard)
    - 程式的安全防護
      - 代碼渾淆
      - 加核與加密 
    - 開發安全與SSDLC

        - SQL == Structured Query Language == 結構化查詢語言
```
SELECT first_name, last_name 
FROM users 
WHERE user_id = '$id'
```

- [Mitre Att&CK](https://attack.mitre.org/)
- [Common Attack Pattern Enumeration and Classification (CAPEC™)](https://capec.mitre.org/about/index.html)

## 3.資安維運技術
  - 3-1.惡意程式防護與弱點管理
    -  各種惡意程式(malware)
       - 勒索軟體
       - 網站木馬
       - 蠕蟲(worm) 
    - 惡意程式分析(malware analysis)
       - 靜態分析
       - 動態分析
    -  惡意程式防護
    -  弱點與弱點資料庫
    -  弱點嚴重性 CVSS
    -  弱點管理
       - 弱點掃描(Vulnerability Assessment)
       - 網站弱點掃描
       - 系統弱點掃描
  - 3-2.資料安全及備份管理
    - 資料安全(data security)
      - 資料外洩
    - 備份管理
      - 資料備份方式:
        - 完全備份(Full Backup) 
        - 差異備份(Differential Backup)  
        - 增量備份(Incremental Backup)
      - 儲存媒體
      - RAID 
      - 備份管理作業
  - 3-3.日誌管理
    - 日誌管理基本觀念
    - 日誌類型==> (A)系統日誌檔 (B) 應用程式日誌檔 (C) 安全性日誌檔
    - Windows 作業系統日誌檔
    - 日誌分析
    - 日誌管理

  - 3.4.資安防護技術
    - [Mitre D3FEND™ - A knowledge graph of cybersecurity countermeasures](https://d3fend.mitre.org/) 
    - 防火牆(Firewall)
      - 防火牆類型
        - 封包過濾防火牆(Packet-Filtering Firewall)
        - 狀態檢視防火牆(Stateful Inspection Firewall)
        - 代理伺服器(Proxy Server)
    - 網站應用程式防火牆(Web Application Firewall, WAF)
    - 蜜罐（Honeypot）
    - 滲透測試(Penetration Testing)  vs 紅隊演練 (Red Team Assessment) 


  
## 4.新興科技安全
  - 4-1.雲端安全概論
    - 雲端運算定義
    - 雲端安全
  - 4-2.行動裝置安全概論
    - OWASP MOBILE TOP 10 
  - 4-3.物聯網安全概論
    - 物聯網(IOT)
    - OWASP IOT TOP 10  


