+++
date = '2025-11-06T14:56:16+08:00'
draft = false
title = '如何用Hugo架設網站？'
+++

### 首先我們需要下載hugo,git插件
```brew install hugo```

```brew install git```

---

### 再來我們在終端機上輸入
- ```hugo new site "資料夾名稱"``` 

### 進入到資料夾 
- ```cd "資料夾名稱"```

### 初始化git資料庫
- ```git init```

### 匯入範本
- ```git submodule add "你想要的範本" themes/"名稱"```
- ### ```git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke```

[hugo範本連結](https://themes.gohugo.io/)

### 把範本讀進hugo.toml
- ```echo "theme = 'anank e'" >> hugo.toml```

### 在本地啟動hugo.toml
- ```hugo server```

---

# 如何新增一個內容content

### 在content/posts資料夾新增.md檔
- ```hugo new content content/posts/"檔案名稱".md```

### 生成出.md檔案
```
+++
title = 'My First Post' #檔案的title
date = 2024-01-14T07:07:07+01:00
draft = true #草稿
+++
```

### .md檔案編輯
```
+++
title = 'My First Post'
date = 2024-01-14T07:07:07+01:00
draft = true
+++
## 從這裡開始寫內容 "#"是h標籤
這是我的示範檔案
```