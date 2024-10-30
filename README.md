# **實驗三、UML靜態建模之類的分析與設計**
11024134 陳家蓁 11024225 林晉維
## 實驗目的
透過UML建模過程掌握類別的分析與設計方法。
## 實驗環境
[PowerDesigner](https://gitcode.com/open-source-toolkit/92ac6/overview?utm_source=highlight_word_gitcode&word=PowerDesigner)
## 實驗任務
針對「迷你[圖書管理系統](https://gitcode.com/open-source-toolkit/ede4c/overview?utm_source=highlight_word_gitcode&word=%E5%9B%BE%E4%B9%A6%E7%AE%A1%E7%90%86%E7%B3%BB%E7%BB%9F)」的使用案例圖(圖1)，進行分析，完成類別建模。
![image](https://github.com/11024134/midterm/blob/main/%E5%9C%961.jpg)
圖1：迷你圖書管理系統用例圖
## 實驗步驟
分析實驗任務內容，並利用UML完成類別的建模並產生對象，主要包括： 
  1.定義類別（包括類別名稱、屬性、操作等） 
  2.建模類別之間的關係（包含關聯、泛化、依賴、實作等） 
  3.建構完整的類別圖（至少包含抽象類別、組合、聚合、多重性、可見性和介面等） 
  4.根據類別圖，產生系統某一時刻的物件圖 
注意：上述括號內的內容必須體現在圖中，缺少一項本實驗得分扣5分；請自行設計類別圖和物件圖，注意邏輯。
## 實驗過程
1.完整類別圖:
![image](https://github.com/11024134/midterm/blob/main/%E5%9C%962.jpg)
分析： 上圖總的來說共有六個類，其中分別是User,RegisteredUser,OrdinaryUser,LibraryManager,MailSystem, [Library](https://gitcode.com/gh_mirrors/lib/library/overview?utm_source=highlight_word_gitcode&word=library)_ .
其中，MailSystem是介面。 User類別關聯RegisterUser和OrdinaryReader類，同時這兩個類別和User之間也存在聚集關係，LibraryManager和OrdinaryReader都繼承RegisterUser類別。 Library 類別依賴RegisterUser和OrdinaryReader類別；LibraryManager也實作了MailSystem介面,又 和Library之間存在著組成關係，各個類別都設定了一定的可見性，有的定義了一些操作方法。 
2.對象圖：
