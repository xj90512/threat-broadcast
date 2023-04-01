## 运行环境

![](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) 


## 项目介绍

从以下公开的威胁情报来源爬取并整合最新信息：

- 360：https://cert.360.cn/warning
- 奇安信：https://ti.qianxin.com/advisory/
- 红后：https://redqueen.tj-un.com/IntelHome.html
- 绿盟：http://www.nsfocus.net/index.php
- 斗象：https://vas.riskivy.com/vuln
- NVD：https://nvd.nist.gov/feeds/xml/cve/misc/nvd-rss-analyzed.xml
- CNNVD：http://www.cnnvd.org.cn/web/vulnerability/querylist.tag
- Tenable (Nessus)：https://www.tenable.com/cve/feeds?sort=newest
- ~~安全客：https://www.anquanke.com/vul~~ （该平台已经不做 CVE 分析了）
- ~~CNVD：https://www.cnvd.org.cn/flaw/list~~ （该平台不断升级反爬机制，表示尊重）

<details>
<summary><b>关于 CVE 收录的完整性问题说明</b></summary>
<br/>


本程序只收录国内外安全厂商已收录并分析的 CVE，并不收录所有 CVE，需要全量 CVE 的同学可自行去以下站点下载：

- CVEs 官网： https://cve.mitre.org/
- GitHub（CVEs 实时同步）： https://github.com/CVEProject/cvelist
- CIRCL（CVEs 实时同步）： https://cve.circl.lu/ 或 https://cve.circl.lu/api/browse
- 每日 CVE： https://cassandra.cerias.purdue.edu/CVE_changes/today.html

## 目录说明

```
threat-broadcast
├── README.md ............................... [项目说明]
├── main.py ................................. [程序运行入口]
├── cache ................................... [威胁情报缓存]
├── data
│   └── cves.db ............................. [sqlite: 威胁情报归档]
├── docs .................................... [Github Page 威胁情报总览]
├── recv
│   ├── mail_*.dat .......................... [接收威胁情报的邮箱]
│   └── qq_group.dat ........................ [接收威胁情报的 QQ 群]
├── src ..................................... [项目源码]
├── script .................................. [数据库脚本]
├── tpl ..................................... [模板文件]
├── imgs .................................... [项目图片]
└── logs .................................... [项目日志]
```

