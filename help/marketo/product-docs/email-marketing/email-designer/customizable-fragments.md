---
solution: Marketo Engage
product: marketo
title: カスタマイズ可能なフラグメント
description: 一部のフィールドを編集可能にしてフラグメントをカスタマイズする方法について説明します。
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 64%

---

# カスタマイズ可能なフラグメント {#customizable-fragments}

フラグメントをメールまたはメールテンプレートで使用すると、継承が原因で、デフォルトでロックされます。 つまり、フラグメントに対して行われた変更は、フラグメントが使用されているすべてのアセットに自動的に反映されます。 カスタマイズ可能なフラグメントを使用すれば、フラグメントがメールまたはメールテンプレートに追加されたときに、フラグメント内の特定のフィールドを編集可能として定義できます。 例えば、バナー、テキスト、ボタンを含むフラグメントがあるとします。画像やボタンのターゲット URL など、特定のフィールドを編集可能として指定できます。これにより、ユーザーはフラグメントをメールやメールテンプレートに組み込む際にこれらの要素を変更でき、元のフラグメントに影響を与えることなくカスタマイズされたエクスペリエンスを提供できます。

カスタマイズ可能なフラグメントを活用することで、まったく新しいコンテンツブロックを作成したり、元のフラグメントからの継承を中断したりすることなく、コンテンツを効率的に管理およびパーソナライズできます。これにより、フラグメントレベルで行われた変更が引き続き反映されますが、メール/メールテンプレートレベルで必要なカスタマイズが可能になります。

ビジュアルフラグメントと式フラグメントの両方をカスタマイズ可能としてマークできます。各タイプのフラグメントの処理方法について詳しくは、以下の節を参照してください。

## ビジュアルフラグメントへの編集可能なフィールドの追加 {#visual}

ビジュアルフラグメントの一部を編集可能にするには、次の手順に従います。

>[!NOTE]
>
>編集可能なフィールドは、**画像**、**テキスト**、**ボタン**&#x200B;コンポーネントに追加できます。**HTML** コンポーネントの場合、式フラグメントと同様に、パーソナライゼーションエディターを使用すると、編集可能なフィールドが追加されます。[詳しくは、HTML コンポーネントと式フラグメントに編集可能フィールドを追加する方法を参照してください](#expression)

1. フラグメントコンテンツ編集画面を開きます。

1. 編集可能なフィールドを設定するフラグメント内のコンポーネントを選択します。

1. コンポーネントのプロパティパネルが右側に開きます。「**[!UICONTROL 編集可能なフィールド]**」タブを選択し、「**[!UICONTROL 編集を有効にする]**」オプションを切り替えます。

1. 選択したコンポーネントの編集可能なすべてのフィールドがパネルにリストされます。編集可能なフィールドは、選択したコンポーネントタイプによって異なります。

   以下の例では、「ここをクリック」ボタンの URL の編集を許可します。

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. **[!UICONTROL 概要]** をクリックして、編集可能なすべてのフィールドとそのデフォルト値を確認します。

   この例では、ボタンの URL フィールドに、コンポーネントで定義したデフォルト値が表示されます。この値は、ユーザーがコンテンツにフラグメントを追加した後にカスタマイズできます。

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. 完了したら、変更を保存します。

フラグメントをメールに追加すると、フラグメントで設定されたすべての編集可能フィールドをユーザーがカスタマイズできるようになります。
<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->
>[!MORELIKETHIS]
>
>[フラグメント](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
