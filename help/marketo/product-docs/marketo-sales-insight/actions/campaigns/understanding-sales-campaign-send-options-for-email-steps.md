---
description: セールスキャンペーンのメールステップの送信オプションについて説明します。 送信するタイミング、送信時間をスケジュールするタイミング、または最初と次のステップに向けて送信するタスクを作成するタイミングを選択できます。
title: メールステップにおけるセールスキャンペーンの送信オプションについて
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
TQID: 'https://experienceleague.adobe.com/dd4l3DH5i6E-zpjJk-cpQTMgZy-3a90JcrkeAFGl4PM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 93%
---
# メールステップのセールスキャンペーン送信オプションについて {#understanding-sales-campaign-send-options-for-email-steps}

セールスキャンペーンを作成する場合、[!DNL Sales Insight Actions] でのメール手順の作成方法に関して、いくつかのオプションがあります。 また、セールスキャンペーン内のどのステップのメールかによって、利用できるオプションも異なります。

## 最初のステップの送信オプション {#first-step-send-options}

セールスキャンペーンの最初のステップと初日の場合は、次のオプションがあります。

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### このメールを送信するタイミングを自分で選択する {#first-step-i-will-choose}

* このオプションを使用すると、人物を追加してセールスキャンペーンを開始する際に、そのセールスキャンペーン内で最初に送信するメールの「送信時刻」を選択できます。

### 以下の時刻にこのメールを送信する {#first-step-following-time}

* リードを追加してセールスキャンペーンを開始する際に、今回のメールのスケジュールが設定されます。
* セールスキャンペーンを開始する際に、常に新しい「送信時刻」を選択するオプションがあります。

### タスクを作成（このメールは自分で送信） {#first-step-create-a-task}

* このオプションでは、都合のよいときに送信できるメールタスク（および [!DNL Salesforce] と同期）が作成されます。
* これを選択すると、セールスキャンペーンを開始する際に、コマンドセンターとライブフィードでこれらのタスクがキューに入れられます。 その後、送信前に、各メールをパーソナライズして送信（またはスケジュール）できます。

  * このタスクを web アプリケーションで開くと、作成ウィンドウが開き、取引先責任者のメールアドレス、メールの件名、選択したテンプレートが表示されます。
  * このタスクを Gmail または [!DNL Outlook] で開くと、ネイティブの作成ウィンドウが開き、取引先責任者のメールアドレス、メールの件名、選択したテンプレートが動的に入力されます。

## 後続のステップの送信オプション {#subsequent-step-send-options}

セールスキャンペーンの後続の日／ステップでは、以下のオプションを使用できます。

### このセールスキャンペーンの前のメールと同じ時刻にこのメールを送信 {#subsequent-send-at-same-time}

* このオプションを選択すると、直近のメールと同じ時刻にメールが送信されます。
* 関連付けられた日に送信されます。

>[!IMPORTANT]
>
>同じ日に送信したメールの場合、前のメールと同じ時刻にメールを送信することはサポートされていません。 代わりに、前日にメールを送信した時刻にメールが送信されます。 キャンペーンの初日にメールに対してこのオプションを選択した場合（非推奨）、そのメールはキャンペーンの開始時に即座に送信されます。

### 以下の時刻にこのメールを送信 {#subsequent-send-at-following-time}

* リードを追加してセールスキャンペーンを開始する際に、今回のメールのスケジュールが設定されます。
* セールスキャンペーンを開始する際に、常に新しい「送信時刻」を選択するオプションがあります。

### タスクを作成（このメールは自分で送信） {#subsequent-create-a-task}

* このオプションでは、都合のよいときに送信できるメールタスク（および [!DNL Salesforce] と同期）が作成されます。
* この選択を行った後、セールスキャンペーンを開始すると、[!DNL Sales Insight Actions] はこれらのタスクをコマンドセンターとライブフィードでキューに入れます。 その後、送信前に、各メールをパーソナライズして送信（またはスケジュール）できます。

  * このタスクを web アプリケーションで開くと、作成ウィンドウが開き、取引先責任者のメールアドレス、メールの件名、選択したテンプレートが表示されます。
  * このタスクを Gmail または [!DNL Outlook] で開くと、ネイティブの作成ウィンドウが開き、取引先責任者のメールアドレス、メールの件名、選択したテンプレートが動的に入力されます。

### このキャンペーンの前のメールのフォローアップとしてこのメールを作成 {#subsequent-create-this-email}

* セールスキャンペーンの前のメールを、セールスキャンペーンで送信される次のメールに追加したい場合は、このチェックボックスを有効にします。
* 追加されたメールのコピーの場合、セールスキャンペーンのメールテンプレートが常に送信されます。 送信される前にユーザーが行った編集は、送信には含まれません。

>[!NOTE]
>
>メールをフォローアップとして作成するこのオプションは、前のステップもメールの場合に、メールステップでのみ使用できます。 前のステップが電話、InMail、またはカスタムの場合、フォローアップを作成するオプションは表示されません。

>[!MORELIKETHIS]
>
>[ セールスキャンペーンの作成](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[セールスキャンペーンのステップのタイプとリマインダータスク](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[セールスキャンペーンの設定](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}
