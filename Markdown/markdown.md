# Markdown #
![avatar](https://markdown.tw/images/208x128.png)

# Markdown語法說明

---
<h2 id="lnk00001"></h2>

# 內文超連結 
```
[內文超連結]((#lnk00001))  
[字型大小](#lnk00002)  
[分隔線 ](#lnk00003)
...

<h2 id="lnk00002"></h2>    /* 設定id */
# 字型大小
``` 
[內文超連結]((#lnk00001))  
[字型大小](#lnk00002)  
[分隔線 ](#lnk00003)  
[字體及刪除線](#lnk00004)  
[任務列表語法介紹](#lnk00005)  
[超連結](#lnk00006)  
[引用](#lnk00007)  
[等寬字](#lnk00008)  
[表格](#lnk00009)  
[插入圖片](#lnk00010)   
[行內 HTML](#lnk00011)   
[Youtube 影片](#lnk00012)  
---
<h2 id="lnk00002"></h2>

# 字型大小

```
語法格式
-------------------------
# *H1
## *H2
### *H3
#### *H4
##### *H5
###### *H6
####### *H7   <<  失效
```
# H1  
## H2
### H3
#### H4
##### H5
###### H6
####### H7   <<  失效

---
<h2 id="lnk00003"></h2>

# 分隔線
```
上一段
Enter <-
---
下一段

--- 連字符
*** 星號
___ 下劃線

```
---
***
___
<h2 id="lnk00004"></h2>

# 粗除體及刪除線
```
  *斜體*
  **粗體**
  ***粗除體***
  ~~刪除線~~
```
  *斜體*  
  **粗體**   
  ***粗除體***  
  ~~刪除線~~  

---
<h2 id="lnk00005"></h2>

# 任務列表語法介紹
```
- [] A
- [] B
- [*] C
```
- [] A
- [] B
- [*] C

---
<h2 id="lnk00006"></h2>

# 超連結
```
[google](https://www.google.com)

[這是一個行內樣式的連結](https://www.google.com)

[這是一個加上標題的行內樣式連結](https://www.google.com "Google 的首頁")

[這是一個引用樣式的連結][任意不區分大小寫的文字]

[以相對的文件路徑引用其他文件](../blob/master/LICENSE)

[可以用數字來宣告一個引用樣式的連結][1]

或讓他空白並使用[連結文字本身]。

網址，或是尖括號中的網址會自動轉換成連結。
http://www.example.com 或 <http://www.example.com> 甚至有時候 example.com 也可以（只是舉例，Github上無效）。

引用連結可以在一些文字後面。

[任意不區分大小寫的文字]: https://www.mozilla.org
[1]: http://slashdot.org
[連結文字本身]: http://www.reddit.com
```
[google](https://www.google.com)  

[test.txt](./test.txt)  

[這是一個行內樣式的連結](https://www.google.com)

[這是一個加上標題的行內樣式連結](https://www.google.com "Google 的首頁")

[這是一個引用樣式的連結][任意不區分大小寫的文字]

[以相對的文件路徑引用其他文件](../blob/master/LICENSE)

[可以用數字來宣告一個引用樣式的連結][1]

或讓他空白並使用[連結文字本身]。

網址，或是尖括號中的網址會自動轉換成連結。
http://www.example.com 或 <http://www.example.com> 甚至有時候 example.com 也可以（只是舉例，Github上無效）。

引用連結可以在一些文字後面。

[任意不區分大小寫的文字]: https://www.mozilla.org
[1]: http://slashdot.org
[連結文字本身]: http://www.reddit.com

---
<h2 id="lnk00007"></h2>

# 引用
```
> A
>> B
>>> C
```
> A
>> B
>>> C

---
<h2 id="lnk00008"></h2>

# 等寬字
```
Project --無等寬語法
`Project` --有等寬語法
```
Project  
`Project`

---
<h2 id="lnk00009"></h2>

# 表格
```
|姓名|性别|年龄|國籍|
  |---|----|----|---|
  |有大JJ的妹子|男|94|日本|
  |有大ㄋㄋ的漢子|女|87|美國|


冒號可以用來標示欄位的對齊方式

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| 第三欄        | 靠右對齊      | $1600 |
| 第二欄        | 置中對齊      |   $12 |
| 斑馬條紋      | 是整齊的      |    $1 |

每個標頭元件都要用至少三個破折號分隔開來。
最外面的豎線可以省略，你也不需要讓原始的文字排列整齊。你也可以使用行內樣式的 Markdown。

不 | 漂亮 | 的文字
--- | --- | ---
*依然* | `渲染的` | **很好**
1 | 2 | 3

```
|姓名|性别|年龄|國籍|
  |---|----|----|---|
  |有大JJ的妹子|男|94|日本|
  |有大ㄋㄋ的漢子|女|87|美國|

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| 第三欄        | 靠右對齊      | $1600 |
| 第二欄        | 置中對齊      |   $12 |
| 斑馬條紋      | 是整齊的      |    $1 |

不 | 漂亮 | 的文字
--- | --- | ---
*依然* | `渲染的` | **很好**
1 | 2 | 3

---
<h2 id="lnk00010"></h2>

# 插入圖片
```
插入本地(Local)圖片
![avatar](./Ex.jpg "Local Picture") //與.md檔在同一個目錄下面

插入網路(Internet)圖片
![avatar](https://markdown.tw/images/208x128.png "Internet Picture")

"文字" 或 (文字) -- 游標移動到上面會顯示文字
```
插入本地圖片  
![avatar](./Ex.jpg "Local Picture")

插入網路圖片  
![avatar](https://markdown.tw/images/208x128.png "Internet Picture")

---
<h2 id="lnk00011"></h2>

# 行內 HTML
```
<dl>
  <dt>定義列表</dt>
  <dd>有時候，人們偶爾會用到。</dd>

  <dt>在 HTML 中撰寫 Markdown</dt>
  <dd>*無法* 運作的 **非常** 好。改用 HTML<em>標籤</em>。</dd>
</dl>
```
<dl>
  <dt>定義列表</dt>
  <dd>有時候，人們偶爾會用到。</dd>

  <dt>在 HTML 中撰寫 Markdown</dt>
  <dd>*無法* 運作的 **非常** 好。改用 HTML<em>標籤</em>。</dd>
</dl>

---
<h2 id="lnk00012"></h2>

# Youtube 影片
Youtube 影片無法直接加入頁面，我們可經由點選圖片，在圖片上設定連結到影片

```
<a href="https://www.youtube.com/watch?v=h-AJ0ApCjVI
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE影片ID放在這裡/0.jpg" 
alt="圖片 ALT 文字放在這裡" width="240" height="180" border="10" /></a>
```
<a href="https://www.youtube.com/watch?v=h-AJ0ApCjVI
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE影片ID放在這裡/0.jpg" 
alt="圖片 ALT 文字放在這裡" width="240" height="180" border="10" /></a>

---
