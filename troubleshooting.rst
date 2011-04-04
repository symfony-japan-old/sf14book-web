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

