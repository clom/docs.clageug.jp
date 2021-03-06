CLAGEUG Docs ドキュメント規約
#############################

.. sidebar:: 目次

   .. contents::
      :depth: 2
      :local:

見出し
======

Markdown
---------
::

  # 見出し1（h1）

  ## 見出し2（h2)

  ### 見出し3

  #### 見出し4

  ##### 見出し5


reStructuredText
----------------
::

  見出し1
  =============

  見出し2
  ------------

  見出し3
  ~~~~~~~

  見出し4
  ^^^^^^^

  見出し5
  '''''''

--------------

段落
=====

Markdown
---------
::

  ここは段落です。♪もーもたろさん もーもたーろさん おっこしーにつっけたーちーびまーるこー

  ここは段落です。
  ↑半角スペース2個で強制改行しています。
  ♪もーもたろさん もーもたーろさん おっこしーにつっけたーちーんあーなごー

  - **強い強調（strong）です。** __これも強い強調です。__ `<strong>`strongタグです。`</strong>`
  - *強調（em）です。* _これも強調です。_ 斜体の`<em>`タグになります。
  - ***強調斜体です。*** ___強調斜体です。___ `<strong>`＋`<em>`タグになります。


  > 引用（Blockquote）です

  > > 引用のネストです

  > 上に一行空けないとネストのままです

  引用（Blockquote）の中にはMarkdown要素を入れられます

reStructuredText
----------------
::

  ここは段落です。♪もーもたろさん もーもたーろさん
  おっこしーにつっけたーちーびまーるこー

  | ここは段落です。
  | ↑半角スペース2個で強制改行しています。
  | ♪もーもたろさん もーもたーろさん
    おっこしーにつっけたーちーんあーなごー

  -  **強い強調（strong）です。** **これも強い強調です。**
    ``<strong>``\ strongタグです。\ ``</strong>``
  -  *強調（em）です。* *これも強調です。*
    斜体の\ ``<em>``\ タグになります。
  -  ***強調斜体です。*** ***強調斜体です。***
    ``<strong>``\ ＋\ ``<em>``\ タグになります。

      引用（Blockquote）です

          引用のネストです

      上に一行空けないとネストのままです

  引用（Blockquote）の中にはMarkdown要素を入れられます
      .. rubric:: 見出し
        :name: 見出し

      1. 数字リスト
      2. 数字リスト

エスケープ文字
==============

Markdown
---------
::

  \*アスタリスクをバックスラッシュでエスケープ\*

  \## 見出しハッシュ文字をエスケープ

  HTMLタグをバックスラッシュでエスケープ→（\<p>）

  HTMLをバッククォートでインラインコード→（`<p>`）

reStructuredText
----------------
::

  \*アスタリスクをバックスラッシュでエスケープ\*

  ## 見出しハッシュ文字をエスケープ

  HTMLタグをバックスラッシュでエスケープ→（<p>）

  HTMLをバッククォートでインラインコード→（\ ``<p>``\ ）

水平線（\ ``<hr>``\ ）各種
==========================

Markdown
---------
::

  ## 水平線（`<hr>`）各種

  アスタリスク3個半角スペース空けて

  * * *
  アスタリスク3個以上

  ******
  ハイフン半角スペース空けて

  - - -
  続けてハイフン3個以上


reStructuredText
----------------
::

  アスタリスク3個半角スペース空けて

  --------------

  アスタリスク3個以上

  --------------

  ハイフン半角スペース空けて

  --------------

  続けてハイフン3個以上

  --------------



リスト
======

Markdown
---------
::

  - ハイフン箇条書きリスト
  + プラス箇条書きリスト
  * 米印箇条書きリスト
      - 二階層め・箇条書きリスト
        - 三階層め・箇条書きリスト
        - 四階層め・箇条書きリスト
  - 箇条書きリスト

  ---

  1. 番号付きリスト
    1. 二階層め・番号付きリスト1
    1. 二階層め・番号付きリスト2
  1. 番号付きリスト2
    1. 二階層め・番号付きリスト1
      1. 三階層め・番号付きリスト1
      1. 三階層め・番号付きリスト2
        1. 四階層め・番号付きリスト1
    1. 二階層め・番号付きリスト2
  1. 番号付きリスト3


  定義リストタイトル
  : 定義リスト要素1
  : 定義リスト要素2
  : 定義リスト要素3


reStructuredText
----------------
::

  -  ハイフン箇条書きリスト
  -  プラス箇条書きリスト
  -  米印箇条書きリスト

    -  二階層め・箇条書きリスト
    -  三階層め・箇条書きリスト
    -  四階層め・箇条書きリスト

  -  箇条書きリスト

  --------------

  1. 番号付きリスト

    1. 二階層め・番号付きリスト1
    2. 二階層め・番号付きリスト2

  2. 番号付きリスト2

    1. 二階層め・番号付きリスト1

        1. 三階層め・番号付きリスト1
        2. 三階層め・番号付きリスト2
        3. 四階層め・番号付きリスト1

    2. 二階層め・番号付きリスト2

  3. 番号付きリスト3

  定義リストタイトル
      定義リスト要素1
      定義リスト要素2
      定義リスト要素3

コードブロック
==============

Markdown
---------
::

  ```
  バッククォート or 半角チルダ3個でくくります。
  ###ここにはMarkdown書式は効きません
  /* コメント */
  testtest // コメント
  ```

  ~~~
  <!DOCTYPE html>
  <head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <title>ニョロニョロ囲みhtml</title>
  /* コメント */
  ~~~

  ```
  <!DOCTYPE html>
  <head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <title>バッククォート囲みhtml</title>
  ```

  ```
  body { display: none; } /* バッククォート囲みcss */
  // コメント
  ```

      // 先頭に半角スペース4つでcode囲い
      <?php if (is_tag()){ $posts = query_posts($query_string . '&showposts=20'); } ?>

  バッククォート1個ずつで囲むとインラインのコード（`<code></code>`）です。`body { visibility: hidden; }`



reStructuredText
----------------
::

  ::

      バッククォート or 半角チルダ3個でくくります。
      ###ここにはMarkdown書式は効きません
      /* コメント */
      testtest // コメント

  ::

      <!DOCTYPE html>
      <head>
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <title>ニョロニョロ囲みhtml</title>
      /* コメント */

  ::

      <!DOCTYPE html>
      <head>
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <title>バッククォート囲みhtml</title>

  ::

      body { display: none; } /* バッククォート囲みcss */
      // コメント

  ::

      // 先頭に半角スペース4つでcode囲い
      <?php if (is_tag()){ $posts = query_posts($query_string . '&showposts=20'); } ?>

  バッククォート1個ずつで囲むとインラインのコード（\ ``<code></code>``\ ）です。\ ``body { visibility: hidden; }``

リンク
======

Markdown
---------
::

  markdownでテキストリンク [WIRED.jp](http://wired.jp/ "WIRED.jp")

  <カッコ>でくくってリンク <http://wired.jp/>

  定義参照リンクです。SNSには [Twitter] [1] や [Facebook] [2] や [Google+] [3]  などがあります。

    [1]: https://twitter.com/        "Twitter"
    [2]: https://ja-jp.facebook.com/  "Facebook"
    [3]: https://plus.google.com/    "Google+"

reStructuredText
----------------
::

  markdownでテキストリンク `WIRED.jp`_

  でくくってリンク http://wired.jp/

  定義参照リンクです。SNSには `Twitter`_ や `Facebook`_ や `Google+`_
  などがあります。


画像
=====

Markdown
---------
::

  ![うきっ！](http://mkb.salchu.net/image/salchu_image02.jpg "salchu_image02.jpg")

reStructuredText
----------------
::

  .. figure:: http://mkb.salchu.net/image/salchu_image02.jpg
    :alt: salchu_image02.jpg

    うきっ！


table
======

Markdown
---------
::

  | Left align | Right align | Center align |
  |:-----------|------------:|:------------:|
  | This       |        This |     This     |
  | column     |      column |    column    |
  | will       |        will |     will     |
  | be         |          be |      be      |
  | left       |       right |    center    |
  | aligned    |     aligned |   aligned    |


reStructuredText
----------------
::

  +--------------+---------------+----------------+
  | Left align   | Right align   | Center align   |
  +==============+===============+================+
  | This         | This          | This           |
  +--------------+---------------+----------------+
  | column       | column        | column         |
  +--------------+---------------+----------------+
  | will         | will          | will           |
  +--------------+---------------+----------------+
  | be           | be            | be             |
  +--------------+---------------+----------------+
  | left         | right         | center         |
  +--------------+---------------+----------------+
  | aligned      | aligned       | aligned        |
  +--------------+---------------+----------------+


GFM
====

リンク
------

Markdown
~~~~~~~~
::

  URLそのまま貼り付け http://wired.jp/


reStructuredText
~~~~~~~~~~~~~~~~
::

  URLそのまま貼り付け http://wired.jp/


段落中の改行
------------

Markdown
~~~~~~~~
::

  ここは段落です。
  ↑returnで改行しています。
  ♪もーもたろさん もーもたーろさん おっこしーにつっけたーちー○○ー○○ー


reStructuredText
~~~~~~~~~~~~~~~~
::

  | ここは段落です。
  | ↑returnで改行しています。
  | ♪もーもたろさん もーもたーろさん おっこしーにつっけたーちー○○ー○○ー


コードブロック
--------------

Markdown
~~~~~~~~
::

  バッククォートの開始囲みに続けて拡張子でシンタックスハイライト

  ```html
  <!DOCTYPE html>
  <head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <title>バッククォート囲みに拡張子付きhtml</title>
  /* コメント */
  ```

  ```css
  body { display: none; } /* コメント */
  ```

  ```php
  <?php if (is_tag()){ $posts = query_posts($query_string . '&showposts=20'); } ?>
  ```

reStructuredText
~~~~~~~~~~~~~~~~
::

  バッククォートの開始囲みに続けて拡張子でシンタックスハイライト

  .. code:: html

      <!DOCTYPE html>
      <head>
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <title>バッククォート囲みに拡張子付きhtml</title>
      /* コメント */

  .. code:: css

      body { display: none; } /* コメント */

  .. code:: php

      <?php if (is_tag()){ $posts = query_posts($query_string . '&showposts=20'); } ?>

取り消し線
----------

Markdown
~~~~~~~~
::

  ~~取り消し線（GFM記法）~~
  <s>sタグです。</s>


reStructuredText
~~~~~~~~~~~~~~~~
::

| [STRIKEOUT:取り消し線（GFM記法）]
| sタグです。


単語中のアンダースコアの無効
----------------------------
Markdown
~~~~~~~~
::

  GitHub_Flavored_Markdown_test_test


reStructuredText
~~~~~~~~~~~~~~~~
::

  GitHub\_Flavored\_Markdown\_test\_test


tasklist
--------

Markdown
~~~~~~~~
::

  - [ ] task1
  - [ ] task2
  - [x] completed task

reStructuredText
~~~~~~~~~~~~~~~~
::

  -  [ ] task1
  -  [ ] task2
  -  [x] completed task


