# SQL_Injection_Scan_by_Python
## 專案名稱: Cyber Security Tool SQL Injection Scan by Python

### 參考檔案:**[CyberSecurityTool_SQLinjectionScan.pdf](https://github.com/jerry7776112/SQL_Injection_Scan_by_Python/blob/main/CyberSecurityTool_SQLinjectionScan.pdf)**

### What is SQL Injection:
是發生在網站、應用程式與資料庫之間的安全漏洞，駭客會在設計不良的程式中夾帶惡意指令，讓資料庫伺服器誤以為該指令是正常的SQL指令而執行，因此遭到破壞或入侵。透過利用 SQL 注入，攻擊者可繞過身份驗證，訪問、修改和刪除資料庫中的數據。
##### Type:
*	**In-band SQLi (Classic SQLi):**
最常見且最容易利用的 SQL Injection攻擊。 當攻擊者能夠使用相同的通訊通道發起攻擊並收集結果時，就會發生In-band SQL Injection。
*	**Error-based SQLi:**
透過資料庫服務器顯示的錯誤消息來獲取有關資料庫結構的相關資訊。在某些情況下，僅透過Error-based SQL injection就足以讓攻擊者enumerate整個資料庫。 通常發生在Web開發階段。
*	**Union-based SQLi:**
利用 UNION SQL 運算符將兩個或多個 SELECT 語句的結果組合成一個結果，作為 HTTP 響應其中一部份的回傳。
*	**Inferential SQLi (Blind SQLi):**
Inferential SQL Injection需要更長時間才能被攻擊者利用，但它與任何其他形式的 SQL 注入一樣危險。 在Inferential SQL Injection中，實際上沒有數據通過 Web 應用程序傳輸，攻擊者無法看到攻擊的結果。 攻擊者可透過發送payloads、觀察 Web 應用程序的回應及資料庫服務器的最終行為來重建資料庫結構。
*	**Boolean-based (content-based) Blind SQLi:**
依據向資料庫所發送的 SQL 查詢，強制應用程序根據查詢結果返回 TRUE 和 FALSE 來判斷資料庫結構。 此種攻擊效率緩慢，需逐個字符嘗試。
*	**Time-based Blind SQLi:**
依據向資料庫所發送的 SQL 查詢，強制資料庫在回應之前等待指定的時間（以秒為單位）。 回應時間將向攻擊者顯示查詢結果是 TRUE 還是 FALSE。此種攻擊效率緩慢，需逐個字符嘗試。
*	**Out-of-band SQLi:**
不常見，用於替代time-based 的另外一種方式。根據資料庫服務器發出 DNS 或 HTTP 請求以將數據傳遞給攻擊者的能力。主要取決於 Web 應用程序使用的資料庫服務器上啟用的功能。 當攻擊者無法使用同一通道發起攻擊並收集結果時，就會發生。

#### 實作
* SQL Injection Scan by Python
* Network Concept
* Python-requests
* Python-BeautifulSoup
* Python-sys

#### Usage
1.  ```pip install -r requirements.txt```
2.  ```python scan.py [anyURL]```
      ``` ex: python scan.py https://cnn.com ```
