# Git 基礎教學

## 如何指定本地倉，並連結到遠端倉的路徑及指定分支

  - 先來到本地倉的目錄位置
  - 初始化 git init
  - 連結到遠端倉的路徑 git remote add origin 遠端倉的路徑
  - 將遠端倉的內容拉回本機端(如果有的話) git pull origin master (預設通常都叫 master 或 main)
  - 將本地倉的檔案送暫存 git add .
  - 註解檔案並設定斷點 git commit -m "註解的內容"
  - 推送到遠端倉 git push origin master
    > 如果不想每次推送都要加 origin master 的話，可以再推送前先設定源頭的位置，方式如下 git push --set-upstream origin master (master 遠端分支的名稱，通常不是 master 要不就是 main)
  - 完成

## 如何將遠端倉的內容複製到自己的電腦裡

  - 先到指定的目錄(自己的電腦)
  - git clone 遠端倉的路徑

    這樣就完成一次的複製動作，接下來你在自己電腦中進行任何的修改，修改完成後再將檔案 push 推回遠端倉

  - 將本地倉的檔案送到盤點的暫存區 git add .
  - 註解檔案並設定 git 斷點 git commit -m "註解的內容"
  - 推送到遠端倉 git push origin master
    > 如果不想每次推送都要加 origin master 的話，可以再推送前先設定源頭的位置，方式如下 git push --set-upstream origin master (master 遠端分支的名稱，通常不是 master 要不就是 main)
  - 完成

## 如何查詢當前目錄下的遠端倉有哪些?

  - git remote -v

## 如何 fork 其他人的 github 專案?

    如果想要參與一個沒有推送權限的專案，可以先「fork」一份到自己的 github 下，你可以對它進行各種操作，完成後，你可以繼續停留在自己的 github，也可以通知原作者進行合併。
    就像拿叉子將別人盤中的食物，叉到自己的盤子裡一樣。
