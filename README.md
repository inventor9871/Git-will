## 參考保哥的MD
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
檢查狀態， git status
加入索引， git add .
提交更新， git commit -m '修改訊息'
提交後查詢， git log

4. [忽略的檔案](https://github.com/github/gitignore)
將要忽略的檔案或是副檔名寫入到.gitignore，在 add 與 commit。

5. 還原到這次的 commit，有時修改壞了，就重新來過。
git reset --hard

## GitHub 練習
6. 註冊github
7. 建議先在github建立repo，在clone下來。
修改完就可以push傳回去，git push

8. 第一次 git clone 會問 web密碼 或是 token。
9. 可以搜尋別人的專案，但要注意更新時間，太舊的就...

## branch 分支
10. github的主支叫 main(也可以修改)。分支的好處是不會影響到主支。
11. 查看有哪些分支。 git branch
12. 新增分支，git branch feature1
13. 切換分支，git checkout 分支名。
切換主支，git checkout main
14. 合併分支前，要先切換到主支，才能合併。
git merge feature1


