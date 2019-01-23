 
## Quick Xamarin BLE
用於xamarin 上訪問藍芽

## 使用限制

|平台  |限制  |
|--|--|
| xamarin.forms |  |
| xamarin.android   |API LEVEL>=18  |
| xamarin.ios | ios SDK>=7
  |
 

## 安裝
[**NuGet**](https://www.nuget.org/packages/Quick.Xamarin.BLE/)

	Install-Package Quick.Xamarin.BLE -Version 1.0.0
	
 

## 範例程式

 

## 刪除文件

您可以通過單擊文件資源管理器中的**刪除**按鈕來刪除當前文件。該文件將被移動到** Trash **文件夾中，並在7天不活動後自動刪除。

## 導出文件

您可以通過單擊菜單中的**導出到磁盤**來導出當前文件。您可以選擇將文件導出為純Markdown，使用Handlebars模板或PDF作為HTML導出。


＃同步

同步是StackEdit的最大特色之一。它使您可以將工作區中的任何文件與存儲在** Google Drive **，** Dropbox **和** GitHub **帳戶中的其他文件同步。這使您可以繼續在其他設備上書寫，與共享文件的人協作，輕鬆集成到您的工作流程中...同步機制在後台每分鐘進行一次，下載，合併和上傳文件修改。

有兩種類型的同步，它們可以相互補充：

- 工作區同步將自動同步所有文件，文件夾和設置。這將允許您在任何其他設備上獲取工作區。	> 要開始同步工作區，只需在菜單中使用Google登錄即可。- 文件同步將使工作區的一個文件與** Google Drive **，** Dropbox **或** GitHub **中的一個或多個文件同步。	> 在開始同步文件之前，您必須在** Synchronize **子菜單中鏈接一個帳戶。





## 打開一個文件

You can open a file from **Google Drive**, **Dropbox** or **GitHub** by opening the **Synchronize** sub-menu and clicking **Open from**. Once opened in the workspace, any modification in the file will be automatically synced.

## Save a file

You can save any file of the workspace to **Google Drive**, **Dropbox** or **GitHub** by opening the **Synchronize** sub-menu and clicking **Save on**. Even if a file in the workspace is already synced, you can save it to another location. StackEdit can sync one file with multiple locations and accounts.

## Synchronize a file

Once your file is linked to a synchronized location, StackEdit will periodically synchronize it by downloading/uploading any modification. A merge will be performed if necessary and conflicts will be resolved.

If you just have modified your file and you want to force syncing, click the **Synchronize now** button in the navigation bar.

> **Note:** The **Synchronize now** button is disabled if you have no file to synchronize.

## Manage file synchronization

Since one file can be synced with multiple locations, you can list and manage synchronized locations by clicking **File synchronization** in the **Synchronize** sub-menu. This allows you to list and remove synchronized locations that are linked to your file.


# Publication

Publishing in StackEdit makes it simple for you to publish online your files. Once you're happy with a file, you can publish it to different hosting platforms like **Blogger**, **Dropbox**, **Gist**, **GitHub**, **Google Drive**, **WordPress** and **Zendesk**. With [Handlebars templates](http://handlebarsjs.com/), you have full control over what you export.

> Before starting to publish, you must link an account in the **Publish** sub-menu.

## Publish a File

You can publish your file by opening the **Publish** sub-menu and by clicking **Publish to**. For some locations, you can choose between the following formats:

- Markdown: publish the Markdown text on a website that can interpret it (**GitHub** for instance),
- HTML: publish the file converted to HTML via a Handlebars template (on a blog for example).

## Update a publication

After publishing, StackEdit keeps your file linked to that publication which makes it easy for you to re-publish it. Once you have modified your file and you want to update your publication, click on the **Publish now** button in the navigation bar.

> **Note:** The **Publish now** button is disabled if your file has not been published yet.

## Manage file publication

Since one file can be published to multiple locations, you can list and manage publish locations by clicking **File publication** in the **Publish** sub-menu. This allows you to list and remove publication locations that are linked to your file.


# Markdown extensions

StackEdit extends the standard Markdown syntax by adding extra **Markdown extensions**, providing you with some nice features.

> **ProTip:** You can disable any **Markdown extension** in the **File properties** dialog.


## SmartyPants

SmartyPants converts ASCII punctuation characters into "smart" typographic punctuation HTML entities. For example:

 


## KaTeX

You can render LaTeX mathematical expressions using [KaTeX](https://khan.github.io/KaTeX/):

The *Gamma function* satisfying $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ is via the Euler integral

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

> You can find more information about **LaTeX** mathematical expressions [here](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).


## UML diagrams

You can render UML diagrams using [Mermaid](https://mermaidjs.github.io/). For example, this will produce a sequence diagram:

```美人魚
序列
圖表愛麗絲 -  >>鮑勃：你好鮑勃，你好嗎？
鮑勃 -  >>約翰：約翰，你呢？
鮑勃 -  x愛麗絲：我很感謝！
Bob-x John：我很感謝！
注意約翰的權利：鮑勃認為很長很長一段時間，因為文本不適合連續。鮑勃 - >愛麗絲：和約翰一起檢查......愛麗絲 - > 約翰：是的......約翰，你好嗎？```





這將產生一個流程圖：

``美人魚
圖LR 
A [方形矩形]  - 鏈接文字 - > B（（圓圈））
A  - > C（圓形矩形）
B  - > D {菱形} 
C  - > D```
