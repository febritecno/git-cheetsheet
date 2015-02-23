gitリポジトリ作成
================
## git init
(カレントディレクトリがgitリポジトリのルートディレクトリになる)

参照系
=====

## コミットログ表示
git log

## 
git status

git status -s


indexへの追加/削除など
====================

## 追加
git add


コミットの作成
===============

## ステージングされているファイルからコミット作成
git commit

## コミット作成()

ブランチ系
## ブランチ移動
git checkout {branch名}

## 現在のブランチを表示
git branch

## 全てのブランチを表示(origin/***も表示される)
git branch -a

## ブランチ作成(現在のHEAD)
git checkout -b {新規ブランチ名}

リモートに関する操作
====

## リモートリポジトリの登録
git remote add {リモートリポジトリ名} {リモートリポジトリURL}

## リモートリポジトリを更新 (細かく指定する場合)
`git push [リモートリポジトリ名] [更新元ブランチ][:リモートブランチ名]`

リモートリポジトリを省いた場合、多くの場合 origin にpushされる
リモートブランチ名を省いた場合(git push origin )
詳細は man git-pushのEXAMPLESを参照されたし

## master
git push

## リモートリポジトリのj

stash系
========

git stash



履歴修正系
============

ワーキングツリーをキレイにしておくこと
(git status -s で M, A, R, U  のファイルががない状態)

## 直近のコミットメッセージを再編集
git commit --amend


## 
