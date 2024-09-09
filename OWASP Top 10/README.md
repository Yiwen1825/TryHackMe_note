# OWASP Top 10
Learn about and exploit each of the OWASP Top 10 vulnerabilities; the 10 most critical web security risks.
## Introduction
* Injection 注入攻擊
* Broken Authentication 身份驗證機制缺陷
* Sensitive Data Exposure 敏感數據暴露
* XML External Entity XML 外部實體注入
* Broken Access Control 存取控制機制缺陷
* Security Misconfiguration 存取控制機制缺陷
* Cross-site Scripting 跨站腳本攻擊
* Insecure Deserialization 不安全的反序列化
* Components with Known Vulnerabilities 使用含已知漏洞的元件
* Insufficent Logging & Monitoring 日誌與監控不足
## Injection
* SQL Injection: 通過注入惡意 SQL 查詢來操縱查詢結果
* Command Injection: 輸入系統命令使應用程式伺服器執行系統命令
### Command Injection Practical
#### Q1.站根目錄下有什麼奇怪的文字檔案？
![image](https://github.com/user-attachments/assets/36375288-f2eb-450b-bde3-33a14c9eebc9)
1. 先看看目錄底下有什麼文字檔: ```ls```
* Answer: drpepper.txt
#### Q2. 有幾個 non-root/non-service/non-daemon users ?
![image](https://github.com/user-attachments/assets/b2d37242-2380-4b0d-a7de-54757865cf4f)
1. 顯示系統中的所有使用者資訊```cat /etc/passwd```
#### Q3. 該應用程式以什麼用戶身份運行？
![image](https://github.com/user-attachments/assets/79d02e53-9351-4032-a332-bcb2fb485f60)
1. 顯示目前登入使用者的名稱: ```whoami```
* Answer: www-data
### Q4. 使用者的shell設定為什麼？
### Q5. 正在運行什麼版本的 Ubuntu？
### Q6. 輸出 MOTD。顯示了最喜歡的飲料是什麼？
