# git 簡單教學

## 先 Clone 遠端倉到本地

- 先到指令目錄
- 下指令 git clone https://github.com/ossian-to/test.git
- 如果使用 clone 的話，就不需要指令遠端倉的路徑，也不需要對本地倉的目錄初始化。

## 如何指定本地倉，並連結到遠端倉的路徑及指定分支

  - 先來到本地倉的目錄位置
  - 初始化 git init
  - 連結到遠端倉的路徑 git remote add origin 遠端倉的路徑
  - 指定推送到遠端倉的分支名稱 git push origin master (預設通常都叫 master 或 main)
  - 將本地倉的檔案送暫存 git add .
  - 註解檔案並設定斷點 git commit -m "註解的內容"
  - 推送到遠端倉 git push

## 指定本地倉的遠端倉路徑

  - git remote add origin 遠端倉的路徑

## 常用指令

- 第零步：查看目前 git 的狀態 git status
- 第一步：初始化 git init
- 第二步：建立索引 git add .
- 第三步：commit 到本地倉 git commit -m "文字註解"
- 第四步：推送到遠端倉 git push


