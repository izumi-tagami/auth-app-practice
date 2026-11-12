# auth-app-practice

## 概要
COACHTECH 教材 Tutorial 10-1「認証機能 ハンズオン演習」で作成した成果物です。
（**ここに、何を作ったかを1〜2行で書きましょう**）

## 使用技術
- PHP 8.x
- Laravel 10.x
- Laravel Fortify（認証）
- MySQL
（**他に使ったものがあれば追記してください**）

## 学んだこと
- Laravel Fortify を使ったユーザー登録(/register) / ログイン(/login) / ログアウトの仕組み。
- 未ログインでログインしようとするとログインページへリダイレクト。middleware('auth')にアクセスするにはログインが必要。
- ダッシュボードは自動生成されないので自作する。

## 動作確認
（**どうやって動かして確認するかを記載してください**）
http://localhost/loginにアクセスし、ユーザー登録、ログイン、ログアウトを実行する。

## 詰まったポイントと解決方法
リダイレクト先をRouteServiceProvider::HOMEにしたかったが、どうしてもエラーになってしまうので、'home' => '/dashboard',にした。

<img width="1438" height="859" alt="ダッシュボード" src="https://github.com/user-attachments/assets/81481081-6fd4-4a7f-8df1-bb7a789bc17f" />
