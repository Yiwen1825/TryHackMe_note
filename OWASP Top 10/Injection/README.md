# Injection
* SQL Injection: 通過注入惡意 SQL 查詢來操縱查詢結果
* Command Injection: 輸入系統命令使應用程式伺服器執行系統命令
## Command Injection Practical
### Q1.站根目錄下有什麼奇怪的文字檔案？
1. 先看看目錄底下有什麼文字檔: ```ls```
![image](https://github.com/user-attachments/assets/36375288-f2eb-450b-bde3-33a14c9eebc9)
* Answer: drpepper.txt
### Q2. 有幾個 non-root/non-service/non-daemon users ?
* Non-root/non-service/non-daemon users 是指在 Linux 系統中，不屬於 root 使用者、系統服務帳號或守護進程帳號的普通使用者
1. 顯示系統中的所有使用者資訊```cat /etc/passwd```

![image](https://github.com/user-attachments/assets/b2d37242-2380-4b0d-a7de-54757865cf4f)
* 輸出那些東西的意義:
```
使用者名稱:x:UID:GID:說明字段:主目錄:Shell
```
* UID
  * 0: 系統管理員
  * 1~999: 系統帳號
  * **1000~60000: 可登入帳號**
* 因為沒有UID>1000的用戶所以數量為0
* Answer: 0
### Q3. 該應用程式以什麼用戶身份運行？
1. 顯示目前登入使用者的名稱: ```whoami```

![image](https://github.com/user-attachments/assets/79d02e53-9351-4032-a332-bcb2fb485f60)
* Answer: www-data
### Q4. 使用者的shell設定為什麼？
### Q5. 正在運行什麼版本的 Ubuntu？
### Q6. 輸出 MOTD。顯示了最喜歡的飲料是什麼？

