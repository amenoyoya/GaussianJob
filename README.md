# GaussianJob

## 使用言語
[SeleneTalk](https://github.com/amenoyoya/SeleneTalk)（LuaJITベースの独自スクリプト言語）

## 最終バージョン
ver. 3.0.0

## 概要
化学数値計算用ソフトウェア"Gaussian"の支援ツール

SeleneTalk（ver. 2.2.5）にて実装

Gaussianは計算したいジョブを複数登録して順次処理することができるが、Windows版のGaussianは、一度計算を始めると途中でジョブを追加したり削除したりできない仕様だった

この支援ツールは、計算途中でのGaussianのジョブ管理を可能にしたものである

基本的に、Win32APIのSendMessage等を使って、支援ツール側からGaussianにジョブを送信して計算させるという仕組みになっている

## 動作環境
Microsoft Windows 7 64bit, Windows 10 64bit環境で動作確認済み

Gaussian9W用の支援ツールなので、Gaussian9Wがインストールされていないと起動しない