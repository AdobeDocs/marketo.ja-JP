---
description: メールテンプレートのフィールドプロンプトについて説明します。 送信者が送信時にカスタムコンテンツに入力するように促すプレースホルダーを追加します。
title: フィールドプロンプト
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
TQID: https://experienceleague.adobe.com/ahVbX8SGxaVUjSPsU-1uVc36ecIW60lwYXxDZSxC0kU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 79%

---

# フィールドプロンプト {#field-prompts}

フィールドプロンプトを使用すると、メールが送信できるようになる前に、削除または置換される必要があるテキストの文字列をメールに追加できます。 これは、ユーザーに追加のパーソナライゼーションを追加することを思い出させるのに最適な方法です。

フィールドプロンプトを追加するには、目的のテキストを入力します。 感嘆符で開始して、中括弧で囲みます（以下を参照）。

**例：**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>ユーザーは、メールが送信できるようになる前に、このテキストを独自のパーソナライゼーションに置き換える必要があります。

![](assets/field-prompts-1.png)

>[!NOTE]
>
>セールスキャンペーンでプロンプトを使用する場合は、手作業のメール手順でプロンプトを使用することをお勧めします。 これらのステップは、メールを送信するためのリマインダータスクにユーザーを割り当てるので、プロンプトをカスタムテキストに置き換えるチャンスがあります。 セールスキャンペーンの自動メールステップは、ユーザーにプロンプトの置き換えを許可することなく、自動的に送信しようとします。 置き換えられていないプロンプトは、メール送信失敗の原因となります。
