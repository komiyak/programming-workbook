# 課題1

次の XML ファイルをパースし、
同じ構成の XML を `exported.xml` に出力せよ。

```xml
<catalog>
   <book id="bk101">
      <author>
         <name>Gambardella, Matthew</name>
         <gender>male</gender>
      </author>
      <title>XML Developer's Guide</title>
      <genre>Computer</genre>
      <price>44.95</price>
      <publish_date>2000-10-01</publish_date>
      <description lang='en'>An in-depth look at creating applications 
      with XML.</description>
   </book>
   <book id="bk102">
      <author>
          <name>Ralls, Kim</name>
          <gender>male</gender>
      </author>
      <title>Midnight Rain</title>
      <genre>Fantasy</genre>
      <price>5.95</price>
      <publish_date>2000-12-16</publish_date>
      <description lang='en'>A former architect battles corporate zombies, 
      an evil sorceress, and her own childhood to become queen 
      of the world.</description>
   </book>
   <book id="bk103">
      <author>
          <name>Corets, Eva</name>
          <gender>female</gender>
      </author>
      <title>Maeve Ascendant</title>
      <genre>Fantasy</genre>
      <price>5.95</price>
      <publish_date>2000-11-17</publish_date>
      <description lang='en'>After the collapse of a nanotechnology 
      society in England, the young survivors lay the 
      foundation for a new society.</description>
   </book>
</catalog>
```


# 課題2

課題1 の XML ファイルをパースし、
同じ構成の XML を `exported2.xml` に出力せよ。

出力する際に、下記のエレメント（XML要素）を指定したフォーマットに変換せよ。

__変更前のエレメント__

```xml
<title>XML Developer's Guide</title>
```

__変更後のエレメント__

```xml
<title>
   <name>XML Developer's Guide</name>
   <lang>English</lang>
</title>
```

`<title>` エレメントの中に `<name>` と `<lang>` を追加する。


# 課題3

課題1 の XML ファイルをパースし、
同じ構成の XML を `exported3.xml` に出力せよ。

出力する際に、下記のアトリビュート（XML属性）を `<publish_data>` に追加せよ。

```
timezone='utc'
```

出力例：
```xml
<publish_date timezone='utc'>2000-11-17</publish_date>
```
