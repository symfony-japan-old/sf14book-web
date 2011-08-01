======================
トラブルシューティング
======================

本書を読み進める上で、読者の方から頂いたトラブルとその解決方法についての情報を掲載します。

.. contents::
   :depth: 1
   :local:


第2章でインストールしたsymfonyアプリケーションのあるコンピュータの外部からアクセスしている場合
----------------------------------------------------------------------------------------------

第2章で解説しているインストール手順では、最後にfrontend_dev.phpへアクセスしてsymfonyの初期画面の表示を確認しています。
この時、インストールしたコンピュータとは別のコンピュータのWebブラウザからアクセスする場合、frontend_dev.php内の以下の箇所をコメントアウトする必要があります。

.. code-block:: php

    // this check prevents access to debug front controllers that are deployed by accident to production servers.
    // feel free to remove this, extend it or make something more sophisticated.
    if (!in_array(@$_SERVER['REMOTE_ADDR'], array('127.0.0.1', '::1')))
    {
      die('You are not allowed to access this file. Check '.basename(__FILE__).' for more information.');
    }


ご指摘いただいたブログ記事

  * `ただいまsymfony1.4を勉強中！ <http://online-shortcut.com/blog/?p=1350>`_


Windows環境でXAMPP付属のMercury/32を使ってメールを送信する
----------------------------------------------------------

Windowsで開発されている方の場合、XAMPPに付属するMercury/32をSMTPサーバーとして動作させることで、実際にメールを送信することができます。この場合、Mercury/32の以下の点をあらかじめ設定しておいてください。

   XAMPP Control PanelよりMercuryのAdminボタンをクリックし、Mercury/32の管理画面を起動してください。
  * メニューの [Configuration] にある [Mercury SMTP Server] を選択します。
  * [Connection Control] タブで [Do not permit SMTP relaying of non-local mail] のチェックを外し、[OK] をクリックしてください。
  * メニューの [Configuration] にある [Mercury SMTP Client] を選択します。
  * [Name Servers] の欄に、お使いのプロバイダの DNS サーバーの IP アドレスを入力し、[OK] をクリックしてください。
  * XAMPP Control PanelよりMercuryを一旦Stopし、その後Startしてください。

また、symfonybandプロジェクトでは、メールの送信にSendmailを利用するようになっていますが、これをSMTPに変更します。
``apps/frontend/config/factories.yml`` ファイルを開き、mailerの設定を以下のように変更してください。

.. code-block:: yaml

     mailer:
       param:
         charset: 'UTF-8'
         delivery_strategy: realtime
         transport:
           class: Swift_SmtpTransport
           param:
             host: localhost
             port: 25


