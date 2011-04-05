========
正誤情報
========

このページには、書籍『symfony 1.4によるWebアプリケーション開発』の正誤情報について掲載しています。
ご不便をおかけして、大変申し訳ございません。

記述の誤りを見つけられた方は、hidenorigoto@gmail.com までご連絡ください。

.. contents::
   :depth: 1
   :local:

.. _updates-1:

-------------
第1版正誤情報
-------------

.. contents::
   :depth: 1
   :local:


117ページ
~~~~~~~~~

    * 誤：コンパイルなどの中間処理は施されず、require()関数を使って直接読み込まれます。
    * 正：コンパイルなどの中間処理は施されず、requireを使って直接読み込まれます。

125ページ
~~~~~~~~~

    * 誤：最終的に、リスト4-7のschema.ymlは、次のようなSQLでテーブルを作成するのと同じことになります。
    * 正：最終的に、リスト4-\ **9**\ のschema.ymlは、次のようなSQLでテーブルを作成するのと同じことになります。


132ページ
~~~~~~~~~

    * 誤：表4-2のURLから分かるように、楽団ホームページには大きく分けて4つの機能があります。
    * 正：表4-\ **5**\ のURLから分かるように、楽団ホームページには大きく分けて4つの機能があります。


166ページ
~~~~~~~~~

    * 誤：［リスト4-51］－ InquryForm クラスのconfigure() メソッドでウィジェットのHTML 属性とオプションを指定
    * 正：［リスト4-51］－ Inqu\ **i**\ ryForm クラスのconfigure() メソッドでウィジェットのHTML 属性とオプションを指定


184ページ
~~~~~~~~~

    * コラム末尾の参照先にある「More with symfony 生産性を高める」の1行は誤植です。


203ページ
~~~~~~~~~

    * 誤：■ [R]. 22 日目 - デプロイ
    * 正：■ [\ **P**\ ]. 22 日目 - デプロイ


206ページ
~~~~~~~~~

    * 誤：■ [G]. 第12章 - Adminジェネレータ
    * 正：■ [G]. 第\ **14**\ 章 - Adminジェネレータ


207ページ
~~~~~~~~~

    * 誤：■ [G]. Adminジェネレーター
    * 正：■ [G]. **第14章 -** Adminジェネレータ


209ページ
~~~~~~~~~

    * 誤：■ [P]. 17 日目 - AJAX
    * 正：■ [P]. **18** 日目 - AJAX


210ページ
~~~~~~~~~

    * 誤：■ [R]. タスク 設定ファイル
    * 正：■ [R]. タスク


214ページ
~~~~~~~~~

リスト6-1 3行目

    * 誤： Timestampable: {}
    * 正： Timestampable: ~

動作上「{}」でも問題はありませんが、中身を指定しないにも関わらず配列記法にすることは冗長であることと、他のページでの解説との一貫性の点から、「~」に訂正いたします。


263ページ
~~~~~~~~~

誤

.. code-block:: php

    //  ［リスト7-13］――メールアドレスの検証にsjValidatorEmailRFCを使う
    class TestForm extends BaseForm
    {
      public function configure()
      {
        // :
        $this->setValidators(array(
          'email' => new sjValidatorEmailRFC();
        ));
        // :
      }
    }


正（※コメントの行）

.. code-block:: php

    // ［リスト7-13］――メールアドレスの検証にsjValidatorEmailRFCを使う
    class TestForm extends BaseForm
    {
      public function configure()
      {
        // :
        $this->setValidators(array(
          'email' => new sjValidatorEmailRFC(),      // ※カンマに修正
        ));
        // :
      }
    }



266ページ
~~~~~~~~~

誤

.. code-block:: php

    // ［リスト7-16］――入力内容を自動的に半角に変換する
    class TestForm extends BaseForm
    {
      public function configure()
      {
        // :
        $this->setValidators(array(
          'email' => new sjValidatorEmailKtai(array(
            'convert_multibyte' => true,
          ));
        ));
        // :
      }
    }


正（※コメントの行）

.. code-block:: php

    // ［リスト7-16］――入力内容を自動的に半角に変換する
    class TestForm extends BaseForm
    {
      public function configure()
      {
        // :
        $this->setValidators(array(
          'email' => new sjValidatorEmailKtai(array(
            'convert_multibyte' => true,
          )),  // ※カンマに修正
        ));
        // :
      }
    }


363ページ
---------

    * 誤：SELECTであればマスターを、それ以外であればスレーブを参照するように自動で切り替えます。
    * 正：SELECTであれば\ **スレーブ**\ を、それ以外であれば\ **マスター**\ を参照するように自動で切り替えます。


364ページ
~~~~~~~~~

    * 誤：リスト10-5の末尾にあるexecuteMasterKist()がMasterListアクションのコードです。
    * 正：リスト10-5の末尾にあるexecuteMaster\ **L**\ ist()がMasterListアクションのコードです。


384ページ
~~~~~~~~~

    * 誤：http://localhost/frontend_dev.php/page/about
    * 正：http://\ **symfony-band.local**\ /frontend_dev.php/page/about


422ページ
~~~~~~~~~

    * 誤：JavaのStrustやHibernate等、自分で組み合わせる個別のフレームワークを使用していました。
    * 正：Javaの\ **Struts**\ やHibernate等、自分で組み合わせる個別のフレームワークを使用していました。


