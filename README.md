
# 📋 社員管理 CRUD アプリケーション (java_ShainBeanCRUD)

Java (Servlet / JSP) を用いた、社員データの登録・閲覧・更新・削除（CRUD）機能を持つWebアプリケーションです。
MVCモデルの設計

---

## 🚀 画面イメージ / 動作デモ

<img width="746" height="688" alt="GIF-demo" src="https://github.com/user-attachments/assets/fb1048cd-8f0e-41cc-b80b-573e2b5594b5" />


---

## ✨ 主な機能

1. **社員一覧表示機能**
   * 登録されている全社員の情報をリスト形式で一覧表示します。
2. **社員情報登録機能**
   * 新しい社員の情報を入力・送信し、データベースに新規登録します。
3. **社員情報更新機能**
   * 既存の社員情報を編集・上書き保存します。
4. **社員情報削除機能**
   * 不要になった社員データを一覧から削除します。

---

## 📂 ディレクトリ構成

```text
java_ShainBeanCRUD/
 ┣ src/main/java/
 ┃  ┣ beans/             # データ保持用Beanクラス
 ┃  ┃  ┗ ShainBean.java
 ┃  ┣ controller/        # リクエストを受け付け、処理を制御するサーブレット群
 ┃  ┃  ┣ ShainIndex.java
 ┃  ┃  ┣ ShainInsert.java
 ┃  ┃  ┣ ShainInsertComplete.java
 ┃  ┃  ┣ ShainUpdate.java
 ┃  ┃  ┣ ShainUpdateComplete.java
 ┃  ┃  ┣ ShainDelete.java
 ┃  ┃  ┗ ShainDeleteComplete.java
 ┃  ┗ model/             # データベース接続やビジネスロジックを担うクラス
 ┃     ┣ ConnectionBase.java
 ┃     ┗ ShainLogic.java
 ┗ src/main/webapp/
    ┣ WEB-INF/
    ┃  ┣ lib/
    ┃  ┃  ┗ mysql-connector-j-8.0.33.jar
    ┃  ┗ view/              # 画面描画用JSPファイル群
    ┃     ┣ index.jsp
    ┃     ┣ insert.jsp
    ┃     ┣ update.jsp
    ┃     ┣ delete.jsp
    ┃     ┗ error.jsp
      ┗ web.xml
