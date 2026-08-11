- 安裝工具 (C# form)
```
1. DB(確認DB連線正常、更新產品版本資訊等)
2. Client安裝(包含撰寫帶參數給bat執行安裝後續檔案或新增windows服務等)
3. 授權序號驗證
4. 安裝流程頁面設計
```
---
- .msi安裝工具 (WiX v4)
```
1. 安裝頁面設計
2. 安裝流程設計
3. 檢察系統安裝元件(Visual C++ Redistributable...)
4. 安裝系統服務
```
---
- 產品平台 (C# .framework、JavaScript、Html、CSS)
```
1. C# .framework
2. JavaScript
3. Html
4. MVC+ViewModel架構

Model處理後端DB取資料等方法
View處理前端頁面呈現
Controller處理已設計的Request API並接到對應的Model方法
ViewModel儲存前端頁面需要的變數類別(TB、TVCBL等)。

產品我理解的流程是，tracker(或Server)會去收各設備的資訊(IP、MAC、ChassisType、有哪些軟體、登入資訊等)，
收回伺服器寫進DB，可以透過產品網站提供的很多報表進行管理，甚至也可以透過ADServer做到管理等事情。
```
---
- 富文字編輯器 Rich Text Editor (Tiptap)
```
CKEditor LTS版本以前有CPE、CVE弱點問題，更改使用 Tiptap。
1. 文字編輯器頁面設計(純JS)
2. 文字編輯器功能撰寫
3. 向下相容(相容原 CKEditor 產生的 Html 文字)
```
---
- 軟體物料清單 Software Bill of Materials，SBOM (Syft、Trivy、Grype、OSV-Scanner、Batch File)
```
經研究若有較多的自行開發 .dll 套件等，使用Syft進行掃描較全面。
匯出 SBOM 檔案：Syft
比對弱點資料：Trivy、Grype、OSV-Scanner
自動化流程執行：.bat
```
