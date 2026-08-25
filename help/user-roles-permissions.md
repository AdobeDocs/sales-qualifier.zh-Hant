---
title: 使用者角色和許可權
description: 瞭解Sales Qualifier使用者群組如何控制應用程式和管理存取許可權。
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
TQID: 'https://experienceleague.adobe.com/9X9DYGMvLGcPG--G6rHcDEk91hdT9-XYc9wbiL2Qoww'
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4bid: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: d6a8091bd893ea80a26edfc1526646aec037223f
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 4%

---


# 使用者角色和許可權

Sales Qualifier使用兩個必要的使用者群組，將銷售工作與整個組織的設定分開。

## 必要的使用者群組

| 群組 | 屬於誰 | 授予內容 |
| --- | --- | --- |
| `Sales Qualifier` | 每個使用者，包括管理員 | 存取應用程式：潛在客戶、帳戶、參與計畫、工作、績效和設定檔設定。 |
| `Sales Qualifier Admins` | 除了`Sales Qualifier`群組之外，僅限管理員 | 存取&#x200B;**[!UICONTROL 管理設定]**，其管理整個組織的CRM連線、知識中心及規範設定。 |

標準使用者只需要`Sales Qualifier`群組。 管理員需要兩個群組的成員資格。 請參閱[開始使用](getting-started.md)以建立這些群組。

組織也可以建立選用的`Sales Qualifier BDR managers`群組。 成員可以存取電子郵件效能報表。

## 管理員存取權

**[!UICONTROL 管理設定]**&#x200B;僅會顯示在&#x200B;**[!UICONTROL 管理]**&#x200B;之下，供同時屬於兩個必要群組的使用者使用。 這些設定的變更會套用至整個組織。

## 管理員可控制哪些專案

| 設定 | 在何處進行設定 | 效果 |
| --- | --- | --- |
| CRM連線和欄位對應 | [整合](integrations.md#map-crm-fields-inbound-mapping) | 決定潛在客戶或帳戶顯示的CRM欄位，以及篩選可用的欄位。 |
| 全域電子郵件選擇退出 | [整合](integrations.md#configure-global-email-opt-out) | 在每一封傳出電子郵件中新增取消訂閱頁尾。 |
| 知識中心與Playbook | [知識中心](knowledge-center.md) | 使公司行動手冊可用於傳出提示和[AI聊天](ai-assistant.md)。 |
| 活動同步 | [整合](integrations.md#configure-activity-sync-outbound-mapping) | 決定Sales Qualifier外聯活動是否出現在CRM中。 |

標準使用者可以使用這些設定，但無法變更它們。 如果缺少預期的篩選器、教戰手冊參考或CRM欄位，請聯絡管理員。

>[!MORELIKETHIS]
>
>* [開始使用](getting-started.md)
>* [整合](integrations.md)
>* [知識中心](knowledge-center.md)
