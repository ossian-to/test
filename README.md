# Git 基礎教學

## 第一次初始化設定

  - 先來到本地倉的目錄位置
  - 初始化 git init
  - 設定遠端倉的位置 git remote add origin 遠端倉位置
  - 設定 pull 來源的分支名稱 git pull --set-upstream origin master (預設通常都叫 master 或 main)
  - 設定 push 來源的分支名稱 git push --set-upstream origin master (預設通常都叫 master 或 main)
    > pull & push 只需在第一次使用時設定 --set-upstream 即可，這兩個其中一個設定好後，另一個就可以直接使用，不用個別設定。

## 如何指定本地倉，並連結到遠端倉的路徑及指定分支

  - 先完成初始化的動作
  - 將遠端倉的內容拉回本機端 git pull

    接下來你可以在本機端做任何修改，修改完成後，需要將檔案回推到遠端倉，方法如下

  - 將本地倉的檔案送暫存 git add .
  - 註解檔案並設定斷點 git commit -m "註解的內容"
  - 推送到遠端倉 git push
  - 完成

## 如何將遠端倉的內容複製到自己的電腦裡

  - 先到指定的目錄(自己的電腦)
  - git clone 遠端倉的路徑

    這樣就完成一次的複製動作，接下來你在自己電腦中進行任何的修改，修改完成後再將檔案 push 推回遠端倉

  - 將本地倉的檔案送到盤點的暫存區 git add .
  - 註解檔案並設定 git 斷點 git commit -m "註解的內容"
  - 推送到遠端倉 git push
  - 完成

## 如何查詢當前目錄下的遠端倉有哪些?

  - git remote -v

## 如何 fork 其他人的 github 專案?

    如果想要參與一個沒有推送權限的專案，可以先「fork」一份到自己的 github 下，你可以對它進行各種操作，完成後，你可以繼續停留在自己的 github，也可以通知原作者進行合併。
    就像拿叉子將別人盤中的食物，叉到自己的盤子裡一樣。
