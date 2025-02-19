## 參考保哥的MD與github
[對象：保哥](https://github.com/doggy8088/Learn-Git-in-30-days/blob/master/README.md)

## 觀念
* 安裝git，是在自己的電腦安裝git數據庫。
* 註冊github，是要使用github提供的數據庫。
* 不管在本機或是github編輯完，都要 add 與 commit (加入到數據庫)。
* push上傳，pull下載，都是抓commit傳送。

## Git 基本操作
1. 安裝Git，點選下一步即可。用gitbash 看版本
```
git version
```
2. 設定使用者與email
```
git config --list
git config --global user.email '您的email'
git config --global user.name '您的帳號'
```
3. 基本指令
* 檢查狀態， git status
* 加入索引， git add .
* 提交更新， git commit -m '修改訊息'
* 提交後查詢， git log

4. [忽略的檔案](https://github.com/github/gitignore)
將要忽略的檔案或是副檔名寫入到.gitignore，在 add 與 commit。

5. 還原到這次的 commit，有時修改壞了，就重新來過。
git reset --hard

## GitHub 練習
6. 註冊github
7. 建議先在github建立repo，在clone下來。修改完就可以push傳回去(16會說明)。

8. 第一次 git clone 會問 web密碼 或是 token。
9. 可以搜尋別人的專案，但要注意更新時間，太舊的就...

## branch 分支
10. github的主支叫 main(也可以修改)。分支的好處是不會影響到主支。
11. 查看有哪些分支。 git branch
12. 新增分支，git branch feature1
13. 切換分支，git checkout 分支名。
切換主支，git checkout main
14. 合併分支前，要先切換到主支，才能合併。
```
git merge feature1
```
15. tag標籤。因為會有很多commit，可以利用標籤來劃分版本。
* 新增版本，git tag v1
* 看詳細說明，git tag -n
* 刪除標籤，git tag -d 標籤名
* add、commit標籤一起處理，git tag -am '說明文字'  標籤名
* 移動到標籤名，git checkout 標籤名

## 團隊合作
16. 查詢遠端數據庫(github)，git remote
* 將主支推到遠端，git push
* 將分支推到遠端，需先切換到分支f1，再git push。
這時會跳出訊息(git push --set-upstream origin f1)，照著指令輸入即可。
下次只要輸入 git push origin 分支名。
* 修改遠端數據庫名，git remote rename origin 修改名

17. pull 將遠端拉下來。git pull
* 若B寫好code，通知A，此時A只要git pull，就可以將B寫好的拉下來。
* 若兩個人都在寫，這時就會產生衝突(跟merge一樣)，只要修改好即可。

18. 使用github的靜態網頁。點選repo的settings→pages，中間的none改成想要的分支(通常是主支)
，儲存後等一下，再點選剛剛的pages，就會出現網址。

19. 其他資源
[連猴子都會GIT](https://backlogtool.com/git-guide/tw/)
[GIT官方網站](https://git-scm.com/book/zh-tw/v1)

