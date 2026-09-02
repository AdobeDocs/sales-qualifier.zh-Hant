---
title: 管理員設定
description: 瞭解如何管理CRM欄位、活動同步、電子郵件選擇退出和其他Sales Qualifier管理設定。
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
TQID: 'https://experienceleague.adobe.com/vbtO6I67ZEaZz3oio9InNErvq5D0wjbRxyDZpTq8Lzo'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
internal-label: Administration
source-git-commit: f1202dc6d5657875b6cdc35a0116e31cabebf9be
workflow-type: tm+mt
source-wordcount: 845
ht-degree: 0%

---


# 管理員設定

使用&#x200B;**[!UICONTROL 管理員設定]**&#x200B;來設定CRM整合、管理知識中心，以及設定電子郵件選擇退出。

Sales Qualifier會連線至Salesforce或Microsoft Dynamics 365。 此連線可讓Account Qualification Agent (AQA)以一致的方式檢視潛在客戶、帳戶、聯絡人、活動和擁有者。 Sales Qualifier也可以將外聯活動和選擇退出狀態寫回CRM，並將外聯活動與Marketo同步。

若要設定CRM連線、欄位對應和活動同步處理，請移至&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 管理員設定]** > **[!UICONTROL CRM連線]**。 標準使用者可使用已設定的CRM資料和篩選器，但無法變更這些設定。 若要第一次連線CRM，請參閱[開始使用](getting-started.md#connect-your-crm)。

>[!IMPORTANT]
>
>存取&#x200B;**[!UICONTROL 管理員設定]**&#x200B;需要`Sales Qualifier`和`Sales Qualifier Admins`使用者群組的成員資格。

## CRM MCP與內嵌外掛程式

Sales Qualifier會透過下列方式與CRM搭配使用：

* **CRM MCP查詢**—Account Qualification Agent會查詢即時CRM資料，以便回答和深入分析能反映您記錄的目前狀態。
* **內嵌外掛程式**—CRM外掛程式會在您的CRM中顯示[!DNL Marketo Sales Insights] (MSI)深入分析和代理程式資料。 使用此外掛程式將潛在客戶新增至Sales Qualifier。
* **活動同步** — 管理員開啟&#x200B;**[!UICONTROL 活動同步]**&#x200B;時，外聯活動會同步至CRM和Marketo。

## CRM存取範圍

Sales Qualifier會從CRM讀取使用者、聯絡人、擁有者對應、銷售機會、帳戶、商機和活動。 它會只將記錄的外聯活動和選擇退出狀態寫入到CRM，並將外聯活動同步到Marketo。 您的CRM管理員已在Salesforce或Dynamics中準備API存取。 Sales Qualifier管理員接著會連線CRM、對應傳入欄位，並選擇是否同步活動。

>[!NOTE]
>
>[開始使用](getting-started.md#connect-your-crm)中的認證步驟說明對CRM物件的讀取存取權。 如果您開啟活動同步或選擇退出回寫，請和您的CRM管理員合作，授予CRM設定所需的對應寫入許可權。

## 對應CRM欄位（傳入對應）

CRM連線之後，請針對連線選取&#x200B;**[!UICONTROL 管理]**，並開啟&#x200B;**[!UICONTROL 輸入對應]**。 傳入對應可控制Sales Qualifier將哪些CRM欄位提取至應用程式。

1. 選取&#x200B;**[!UICONTROL 新增節]**。
1. 輸入區段名稱和說明。
1. 選取實體型別。 預設會選取&#x200B;**[!UICONTROL 潛在客戶]**。 **[!UICONTROL 連絡人]**、**[!UICONTROL 帳戶]**&#x200B;和&#x200B;**[!UICONTROL 商機]**&#x200B;也可供使用。
1. 選取要匯入的CRM欄位。

   每個欄位列會顯示其&#x200B;**[!UICONTROL 顯示名稱]**、**[!UICONTROL 欄位名稱]**&#x200B;和&#x200B;**[!UICONTROL 資料型別]**。

1. 針對您想要在&#x200B;**[!UICONTROL 潛在客戶]**&#x200B;清單中作為篩選器提供的每個潛在客戶、連絡人或機會欄位，開啟&#x200B;**[!UICONTROL 可篩選]**。
1. 預覽區段並選取&#x200B;**[!UICONTROL 新增]**。

對應的欄位會顯示在Sales Qualifier的對應區域中：

* 潛在客戶欄位會顯示在&#x200B;**[!UICONTROL 人員]**&#x200B;索引標籤上。
* 帳戶欄位出現在&#x200B;**[!UICONTROL 帳戶]**&#x200B;索引標籤上。
* 機會欄位出現在&#x200B;**[!UICONTROL 帳戶機會]**&#x200B;區段中。 可篩選的商機欄位也會在&#x200B;**[!UICONTROL 我的商機聯絡人]**&#x200B;中顯示為自己的欄，並加上標籤，例如&#x200B;**[!UICONTROL 階段（商機）]**，以便與聯絡人欄位區分開來。

## 設定活動同步（傳出對應）

1. 從&#x200B;**[!UICONTROL CRM連線]**，為連線的CRM選取&#x200B;**[!UICONTROL 管理]**。
1. 開啟&#x200B;**[!UICONTROL 輸出對應]**。
1. 開啟&#x200B;**[!UICONTROL 活動同步]**，將Sales Qualifier外聯活動同步回CRM和Marketo。

當活動同步關閉時，Sales Qualifier會繼續使用傳入CRM資料，但不會將外聯活動同步至您的CRM或Marketo。

## 建立知識中心行動手冊 {#knowledge-center}

**[!UICONTROL 知識中心]**&#x200B;可讓Account Qualification Agent (AQA)存取您的銷售資料。 Sales Qualifier使用這些資料來產生研究、資格深入分析和外展活動，以反映貴組織的銷售方式。 只有管理員可以建置和管理行動手冊。

![知識中心](assets/knowledge-center.png){width="800" zoomable="yes"}

1. 在左側導覽列中，展開&#x200B;**[!UICONTROL 管理]**，選取&#x200B;**[!UICONTROL 管理設定]**，然後選取&#x200B;**[!UICONTROL 知識中心]**
1. u
1. 設定Sales Qualifier用來研究您的公司及草擬電子郵件的&#x200B;**[!UICONTROL 公司名稱]**&#x200B;和&#x200B;**[!UICONTROL 公司URL]**。
1. 以PDF、PPTX或DOCX格式上傳銷售重頭戲、理想客戶設定檔(ICP)、定位指南和其他銷售宣傳品。
1. 選取&#x200B;**[!UICONTROL 建置行動手冊]**。

每個上傳的檔案會顯示其處理狀態（例如&#x200B;**[!UICONTROL 就緒]**）以及上次更新時間。

>[!NOTE]
>
>行動手冊最多可能需要24小時的時間處理。

當教戰手冊準備就緒時，代表可以在兩個地方使用它：

* **傳出電子郵件提示** — 在接觸點提示中，命名檔案並描述要使用的內容。 例如，輸入`Use the ABC positioning guide from the Knowledge Center and focus on the security value proposition`。 請參閱[產生並檢閱接觸點](outbound-workflows.md#step-3-generate-and-review-touchpoints)。
* **AI聊天**：請參考您問題中的知識中心。 例如，輸入`From the Knowledge Center, help me position our security solution for ABC Corp before tomorrow's call`。 檢視[AI聊天](ai-assistant.md)。

在這兩種情況下，產生的內容都會反映行動手冊中的訊息，而非一般研究。

## 設定全域電子郵件選擇退出

1. 在左側導覽列中，展開&#x200B;**[!UICONTROL 管理]**&#x200B;並選取&#x200B;**[!UICONTROL 管理設定]**。
1. 選取&#x200B;**[!UICONTROL 合規性]**&#x200B;下的&#x200B;**[!UICONTROL 電子郵件設定]**。
1. 開啟每封電子郵件中的&#x200B;**[!UICONTROL 包含選擇退出連結]**，以將取消訂閱頁尾附加至傳出電子郵件。
1. 在&#x200B;**[!UICONTROL 選擇退出訊息範本]**&#x200B;中輸入頁尾文字。 納入應顯示取消訂閱連結的`{opt_out_link}`權杖。

設定會自動儲存。

當潛在客戶選取連結時，Sales Qualifier會停止向該潛在客戶傳送電子郵件，並將選擇退出狀態同步到連線的CRM。

## 參考資料：範例API引數

您的CRM團隊可以使用這些範例，確認會傳回預期的潛在客戶欄位的讀取存取權。

### Dynamics OData範例

```text
$select=fullname,_ownerid_value,leadid,emailaddress1,jobtitle,statuscode,createdon,modifiedon,statecode
$filter=_ownerid_value eq '<crmUserId>' [AND additional filters]
$expand=Lead_ActivityPointers(...),parentaccountid(...)
$orderby=modifiedon desc
```

### Salesforce SOQL範例

```sql
SELECT Id, Salutation, FirstName, LastName, Name, Title, Company, Email,
  LeadSource, Status, OwnerId, LastModifiedDate, LastActivityDate, CreatedDate,
  (SELECT Id, Subject, ActivityDate, Status FROM Tasks ORDER BY ActivityDate DESC LIMIT 1),
  (SELECT Id, Subject, ActivityDateTime FROM Events ORDER BY ActivityDateTime DESC LIMIT 1)
FROM Lead
WHERE OwnerId = '<crmUserId>' AND IsDeleted = false
ORDER BY LastModifiedDate DESC
```

>[!MORELIKETHIS]
>
>* [開始使用](getting-started.md)
>* [潛在客戶](prospects.md)
