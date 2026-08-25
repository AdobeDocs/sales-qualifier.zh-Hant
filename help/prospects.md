---
title: Sales Qualifier中的潛在客戶
description: 瞭解如何在Sales Qualifier中建立、篩選及檢閱潛在客戶清單，以排定外展活動的優先順序。
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/zf2H5rq1JlIT26LqLPMrm2Mq3tSIrLOiTEw6BXb1w2U'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 08dd05e1d13b501d43d457e6217a43aaabdb1d0d
workflow-type: tm+mt
source-wordcount: 535
ht-degree: 2%

---


# 潛在客戶

在左側導覽中選取&#x200B;**[!UICONTROL 潛在客戶]**，以檢視您可以存取的潛在客戶與連絡人。 使用清單來檢閱每個潛在客戶的狀態和最新活動。

![潛在客戶表格顯示潛在客戶管理的潛在客戶狀態和最後一個活動](./assets/prospects.png){width="800" zoomable="yes"}

* **[!UICONTROL 銷售機會]** — 在連線的CRM中指派給您的銷售機會。
* **[!UICONTROL 連絡人]** — 在連線的CRM中指派給您的連絡人。
* **[!UICONTROL 人員清單]** — 您手動匯入或新增的潛在客戶。

## 建立您的潛在客戶清單

潛在客戶清單結合來自多個來源的人員：

* **CRM潛在客戶**—Sales Qualifier會自動匯入指派給已連線使用者的潛在客戶與聯絡人。 請參閱[整合](integrations.md)。
* **匯入的潛在客戶** — 從CSV檔案匯入的潛在客戶。
* **手動新增潛在客戶** — 在Sales Qualifier中新增個別潛在客戶。

若要新增非來自您CRM的潛在客戶：

1. 在&#x200B;**[!UICONTROL 潛在客戶]**&#x200B;頁面上，選取&#x200B;**[!UICONTROL 人員清單]**。
1. 選取&#x200B;**[!UICONTROL +新增人員]**，然後選取&#x200B;**[!UICONTROL 匯入CSV]**&#x200B;或&#x200B;**[!UICONTROL 新增人員]**。

   * 若要匯入CSV，請上傳`firstname,email`格式的CSV。
     名字和電子郵件為必填。 姓氏為選用。 CSV範本不包含CRM銷售機會ID欄，但您可以在匯入之前將該欄及其值新增到檔案中。 如果匯入失敗，請檢閱錯誤訊息以尋找要更正的欄位或值，然後再次上傳檔案。
   * 若要手動新增人員，請在表單中輸入其詳細資料。

1. 選取「**[!UICONTROL 儲存]**」。

## 篩選和尋找潛在客戶

選取&#x200B;**[!UICONTROL 篩選器]**&#x200B;以縮小清單。 您可以依下列條件篩選：

* 參與計畫狀態
* 建立者
* 職稱
* 帳戶
* 來源
* 上次更新時間

管理員也可以將對應的CRM欄位設為篩選條件。 在&#x200B;**[!UICONTROL 管理員設定]**&#x200B;中，針對代表用來尋找潛在客戶的每個欄位開啟&#x200B;**[!UICONTROL 可篩選]**。 檢視[對應CRM欄位](integrations.md#map-crm-fields-inbound-mapping)。

在&#x200B;**[!UICONTROL 我的商機聯絡人]**&#x200B;中，您也可以依相關商機的欄位來篩選聯絡人，例如階段、型別和結束日期。 商機欄位有標籤，例如&#x200B;**[!UICONTROL 階段（商機）]**，這會將商機欄位與聯絡人欄位區分開來。 您的管理員可控制哪些機會欄位可做為篩選器。

### 依Marketo參與度篩選

透過潛在客戶的即時[!DNL Marketo]參與（例如電子郵件開啟和點按、網頁造訪、表單填寫和有趣的時刻）來尋找並排定其優先順序。 參與幾乎會即時出現。

若要依Marketo參與度篩選潛在客戶：

1. 選取&#x200B;**[!UICONTROL 篩選器]**。
1. 新增[!DNL Marketo]參與篩選器，並設定活動型別、行銷活動或其他屬性，以聚焦於重要的參與。

每個潛在客戶都會顯示其最新的[!DNL Marketo]活動以及最近的歷史記錄。

Marketo參與篩選功能適用於所有生產區域。 您的管理員會為您的組織和沙箱開啟此功能，而行銷人員會在[!DNL Marketo]中完成一次性設定。 請參閱[開啟Marketo參與篩選](integrations.md#turn-on-marketo-engagement-filtering)。

## 檢閱潛在客戶詳細資訊

選取潛在客戶以開啟其設定檔。 在聯絡之前，請先檢閱重要的訊號：

* **AI人員摘要** — 潛在客戶或連絡人及其最近參與的AI寫入快照。 在檢閱個別活動之前，使用摘要來瞭解人員的一目瞭然。 執行Adobe Journey Optimizer B2B edition Prime或Ultimate的執行個體上提供AI人員摘要。
* **活動清單** — 按時間順序排列的活動和最近行為清單。
* **時間表檢視** — 跨管道互動的視覺時間表。
* **已檢視內容** — 潛在客戶已檢視的網頁和資產。 選取要開啟的專案。

>[!MORELIKETHIS]
>
>* [帳戶](accounts.md)
>* [傳出工作流程](outbound-workflows.md)
>* [AI聊天](ai-assistant.md)
