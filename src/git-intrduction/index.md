# 講稿

## 如何管理程式碼

你一定有使用檔案系統做版本控制的經驗
也就像使用 `期末報告完成版.ptt` 、 `期末報告最終版.ppt` 、 `期末報告真的不會再修改.ppt` ，
我們很容易的發現，這麼做有很多缺點，
在每次編輯檔案的時候，都要把整個 project 複製一遍，

光從檔案命名的資訊不夠詳細，我們不容易去推斷，

而且如果你使用複製貼上在管理版本時，
有可能意外覆蓋掉別人的檔案，
而且這個操作很有可能是無法挽回的。

## git

git 就是一種版本控制系統，
也是目前業界最流行的版本控制系統，
最初目的是為更好地管理 Linux 核心開發而設計，
git 與其他版本控制工具不同的點在 git 是分散式，
也就是 git 不需要一台遠端伺服器，
就算沒有網路，在你的電腦上也可以操作，
待有網路的時候再與其它人同步即可。

git 與 react 並沒有直接的關聯，
但學習 git 的目標為了管理程式碼，並且與他人合作，

這邊特別說明，使用 Git 是一種習慣。在單人實作時還沒有很深的感覺，但在與人合作時，能妥善管理自己的程式碼、每筆 commit 都有清楚說明、不會誤刪別人程式碼的工程師，想必是比較令人喜歡的合作對象。

## commit

每一次更動都稱之為 commit ，
在每一個 commit 都有 `訊息` 、 `日期` 、 `修改者`

## 利用分支同時開發不同功能


## 接下來

「Git 可以幫你做哪些事」，但另外準備一套圖形操作軟體，實務上搭配圖形介面來管理程式碼

- 安裝 git CLI / GUI
- 你的第一個 commit (1)
  - config
  - alias
  - init
  - status
  - add / .gitignore
  - commit
- 你的第一個 commit (2)
  - log / log --oneline
  - show / diff
  - remote
  - push
  - Github Pages
  - pull
- 如何修改過去的 commit ?
  - commit --amend
  - revert
  - reset
  - rebase
  - reflog
- 多人合作開發
  - stash
  - branch
  - checkout
  - merge
  - blame

br = branch
cm = commit -n
st = status
cd = checkout
save = stash
load = stash apply
undo = reset HEAD^
acm = commit --amend -n
qcm = commit -m 'hello world' -n
ls = branch
ll = branch
brm = branch -D
fpush = push -f
sync = pull origin master:master
syncd = pull origin develop:develop
