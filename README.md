# 清大企業領航人才培育計畫-華碩 (Cloud Computing)

## 💡課前準備💡

本課程將有實作練習的部分，會以微軟的公有雲平台 Azure 為例,  
請同學們於上課前，開通帳號，並下載相關軟體至您的筆電。

### A、帳號申請 ###

同學們可以申請兩種帳號 *(二擇一)* :

- Azure **學生帳號** [申請連結](https://azure.microsoft.com/zh-tw/free/students/) :  
  - 申請**無須**信用卡  
  - 僅接受 xxx@xxx.edu 校園信箱申請  
  - 第一次申請有 US$100 額度 , 約台幣 NT$3,080
  - 能使用的雲服務較少

- Azure **一般帳號** [申請連結](https://azure.microsoft.com/zh-tw/free/) :  
  - **需要**信用卡進行身分驗證  
  - 第一次申請內建 NT $ 6,300 額度
  - 可使用所有的雲端資源
  
### B、開發環境 IDE ### 

此次 Lab 我們將使用 ( **[Visual Studio Code](https://code.visualstudio.com/)** , VS Code) 作為程式碼檢視、發佈的整合開發環境,  
VS code 可安裝在多種作業系統上 :  
- Windows 版本 (建議選擇 System Installer 確保安裝權限足夠) [下載連結](https://code.visualstudio.com/Download)
- Linux 版本 [下載連結](https://code.visualstudio.com/Download)
- Mac 版本 [下載連結](https://code.visualstudio.com/Download)


### C、輔助工具 ### 

下列為開發雲端應用程式常用到的工具,可以先下載安裝在開發環境 :  

- 遠端連線工具 : **PuTTY** [下載連結](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
- 檔案傳輸 : **WinSCP** [下載連結](https://winscp.net/eng/download.php)
- Web API 開發測試工具 : **Postman** [下載連結](https://www.getpostman.com/postman)
- 資料庫工具 : 
  - **MySQL Workbench** [下載連結](https://dev.mysql.com/downloads/workbench/)
  - **Azure Data Studio** [下載連結](https://docs.microsoft.com/zh-tw/sql/azure-data-studio/what-is?view=sql-server-ver15)


## 💡課程大綱💡
- 介紹雲端運算定義
- 部署模型與應用場景  
  - 公有雲
  - 私有雲
  - 混合雲
 
- 重要雲端服務名詞介紹
- 邊緣運算簡介
- AI as a Service
- LAB (發佈您的第一個雲端服務)


## 💡雲端服務實作與相關參考資源💡

### LAB 規劃

**A、Azure 環境介紹**

 - 首頁網址 :  https://portal.azure.com/
 - 入口網站設定 (選單 / 語言/配色)
 - 資源群組
 - 檢視我的帳單
 - 從 `建立資源` 開始

**B、雲端服務使用**

  - **IaaS**  
    - 建立 VM
    - 使用 UI
     >- Demo Scale UP 
    - 使用 Azure CLI
     >- 帳號 : asus  
     >- 密碼 : ----@-----@---

  - **PaaS**
    - 建立Web Server (App Service)
     > https://docs.microsoft.com/zh-tw/azure/app-service/
     
    - 建立 DB Server
     >- 注意防火牆規則 : `連線安全性`  \ `加入用戶端 IP`  
     >- 政府資料開放平台 : https://data.gov.tw/  
     >- [透過MyWorkbench 匯入 CSV / JSON 資料](https://www.itread01.com/content/1549318893.html)  
     >- 以休閒旅遊 展覽資訊為例  
     >- 工具參考  :  [AzureDataStudio](https://docs.microsoft.com/zh-tw/sql/azure-data-studio/what-is?view=sql-server-ver15)  
     
    - Deploy Web from VS Code to Azure
     >- 參考 : [Azure Extensions](https://code.visualstudio.com/docs/azure/extensions)  
     >- 參考 : [使用 Visual Studio Code 部署至 Azure App Service](https://docs.microsoft.com/zh-tw/azure/javascript/tutorial-vscode-azure-app-service-node-01)  
     >- 範例 : https://html5up.net/  
     >- FTP : https://docs.microsoft.com/zh-tw/azure/app-service/deploy-ftp  

  - **AIaaS (Cognitive Services)**  
    - [認知服務 API](https://azure.microsoft.com/zh-tw/services/cognitive-services/)  
    - Text Service  
     >- LUIS 服務 : https://azure.microsoft.com/zh-tw/services/cognitive-services/language-understanding-intelligent-service/  
     >- https://preview.luis.ai/applications  
    - Computer-vision Service  
     >- https://azure.microsoft.com/zh-tw/services/cognitive-services/computer-vision/  
     >- 參考文件 : https://docs.microsoft.com/zh-tw/azure/cognitive-services/computer-vision/  
     >- 語言支援 : [語言](https://docs.microsoft.com/zh-tw/azure/cognitive-services/computer-vision/language-support)  
     >- 申請試用 :  [API 資訊](https://azure.microsoft.com/zh-tw/try/cognitive-services/my-apis/?apiSlug=computer-vision)  
    - Demo : 使用 Web  
    - Demo : 使用 :PostMan
    - Bot Service  
     >- [Line Bot 設定](https://docs.microsoft.com/zh-tw/azure/bot-service/bot-service-channel-connect-line?view=azure-bot-service-4.0) 
     >- [Azure Bot Service + LUIS + Line Bot 打造你的聊天機器人](https://medium.com/@starcaspar/azure-bot-service-luis-line-bot-%E6%89%93%E9%80%A0%E4%BD%A0%E7%9A%84%E8%81%8A%E5%A4%A9%E6%A9%9F%E5%99%A8%E4%BA%BA-3bbfe9893fd0)  
     >- [Line Bot](http://studyhost.blogspot.com/2019/03/bot-frameworkline-bot.html)

