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

2ページ
~~~~~~~

1-1-1 13行目

    * 誤：PHPでもRauby on Railsのコンセプトを取り入れた「新しい世代のMVCフレームワーク」への期待が高まっていました。
    * 正：PHPでも\ **Ruby**\  on Railsのコンセプトを取り入れた「新しい世代のMVCフレームワーク」への期待が高まっていました。

66ページ
~~~~~~~~

「図2-3 インストール成功確認画面」のスクリーンキャプチャ内のブラウザのアドレスバーのURL

    * 誤：http://localhost/sf14/frontend_dev.php/
    * 正：http://localhost/sf14/\ **web/**\ frontend_dev.php/

94ページ
~~~~~~~~

「図3-1 プロジェクトの基本構成」内のlib/vendor/symfonyディレクトリという枠内の記述

    * 誤：sfCoreAutoload.class.php
    * 正：\ **lib/autoload/**\ sfCoreAutoload.class.php

（この箇所では、「symfonyライブラリのかたまりと、そのかたまりを指定する際の起点ファイル」という意図で図を作成しましたが、lib/vendor/symfonyディレクトリ直下にsfCoreAutoload.class.phpが存在するようにも読めるため、上記のようにディレクトリ以下のパスを追加します）


97ページ
~~~~~~~~

「図3-2 プロジェクトの基本構成2」内のlib/vendor/symfonyディレクトリという枠内の記述

    * 誤：sfCoreAutoload.class.php
    * 正：\ **lib/autoload/**\ sfCoreAutoload.class.php


117ページ
~~~~~~~~~

テンプレート内でのPHPの節 10 行目（requireは関数ではないため訂正します）

    * 誤：コンパイルなどの中間処理は施されず、require()関数を使って直接読み込まれます。
    * 正：コンパイルなどの中間処理は施されず、\ **require**\ を使って直接読み込まれます。


125ページ
~~~~~~~~~

リスト4-11の上の本文。

    * 誤：最終的に、リスト4-7のschema.ymlは、次のようなSQLでテーブルを作成するのと同じことになります。
    * 正：最終的に、リスト4-\ **9**\ のschema.ymlは、次のようなSQLでテーブルを作成するのと同じことになります。

（リスト4-11についての補足）
data/sqlディレクトリに生成されるschema.sqlファイルでは、リスト4-11のような整形されたSQL文ではなく、改行やインデントが入っていない状態で出力されます。
また、CREATE文のオプションとして「CHARACTER SET utf8 COLLATE utf8_unicode_ci」も追加されたものになっています。


127ページ
~~~~~~~~~

図4-9内のディレクトリ名、および図4-9の下の説明文

    * 誤：filters、forms
    * 正：filter、form (\ **s** が不要）

図4-9内のファイル名

    * 誤：PageFilter.class.php
    * 正：Page\ **Form**\ Filter.class.php


132ページ
~~~~~~~~~

    * 誤：表4-2のURLから分かるように、楽団ホームページには大きく分けて4つの機能があります。
    * 正：表4-\ **5**\ のURLから分かるように、楽団ホームページには大きく分けて4つの機能があります。


135ページ
~~~~~~~~~

図4-11「最初のShowアクションの表示」のブラウザの画面キャプチャで、ブラウザのアドレスバーに表示されているURLが本文の表記と異なっていました。正しくは本文の通り「http://symfony-band.local/frontend_dev.php/\ **P**\ age/\ **S**\ how」となります。


151ページ
~~~~~~~~~

ページ下部include_partial()ヘルパーの説明部分

    * 誤：特定のアクションから引数で指定する別のアクションへ、処理を引き渡す。呼び出し元アクションのforward()メソッド呼び出し以降の処理は実行されない。
    * 正：指定した名前のテンプレートを埋め込みます

155ページ
~~~~~~~~~

「スロットを使う」の上の本文

    * 誤：左側にお知らの一覧が表示されるようになっているはずです。
    * 正：左側にお知ら\ **せ**\ の一覧が表示されるようになっているはずです。

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


263-264ページ
~~~~~~~~~~~~~

263ページ下から始まるリスト7-13内（修正箇所は264ページ）
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


274ページ
~~~~~~~~~

下から3行目

    * 誤：リスト7-22のタスクの雛形のececute()メソッドに記述されていた
    * 正：リスト7-22のタスクの雛形のe\ **x**\ ecute()メソッドに記述されていた

282ページ
~~~~~~~~~

下から4行目

    * 誤：有効にしたいプラグン名をenablePlugins()メソッドのパラメータ配列に追加します。
    * 正：有効にしたいプラグ\ **イ**\ ン名をenablePlugins()メソッドのパラメータ配列に追加します。

283ページ
~~~~~~~~~

リスト8-1内 5行目のコメント内

    * 誤：sfDocgrineGuardPluginとsfFormExtraPluginを有効にする
    * 正：sfDoc\ **t**\ rineGuardPluginとsfFormExtraPluginを有効にする


363ページ
~~~~~~~~~

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


386ページ
~~~~~~~~~

11-3-2 「symfony コマンドによるデプロイ」の2行目

    * 誤：これはsymofnyのタスク（symfonyコマンド）で実現されており、
    * 正：これはsym\ **fo**\ nyのタスク（symfonyコマンド）で実現されており、


422ページ
~~~~~~~~~

    * 誤：JavaのStrustやHibernate等、自分で組み合わせる個別のフレームワークを使用していました。
    * 正：Javaの\ **Struts**\ やHibernate等、自分で組み合わせる個別のフレームワークを使用していました。


