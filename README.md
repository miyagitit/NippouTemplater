<html>
<body>

<!--StartFragment-->

<h1>NippouTemplater🍤</h1>

<p>
日報入力を高速化するための
Markdown 補助 Userscript / Bookmarklet です。
</p>

<p>
選択文字の Markdown 化、見出し変更、箇条書き化、
コードブロック化、テンプレート自動挿入などを
ショートカットキーで実行できます。
</p>

<hr>

<h1>主な機能</h1>

<ul>
<li>Markdown 記法のショートカット入力</li>
<li>行頭 Markdown の一括変更</li>
<li>複数行対応</li>
<li>コードブロック自動生成</li>
<li>日報テンプレート保存 / 呼び出し</li>
<li>Ctrl + S で下書き保存</li>
</ul>

<hr>

<h1>ショートカット一覧</h1>

<h2>選択範囲を囲む系</h2>

<table>
<tr>
<th>Shortcut</th>
<th>動作</th>
</tr>

<tr>
<td>Ctrl + H</td>
<td><code>==text==</code></td>
</tr>

<tr>
<td>Ctrl + B</td>
<td><code>**text**</code></td>
</tr>

<tr>
<td>Ctrl + I</td>
<td><code>*text*</code></td>
</tr>

<tr>
<td>Ctrl + ^</td>
<td><code>~~text~~</code></td>
</tr>

<tr>
<td>Ctrl + @</td>
<td><code>``text``</code></td>
</tr>

<tr>
<td>Ctrl + Shift + @</td>
<td>コードブロック化(<code>```[言語名] ... ```</code>)</td>
</tr>
</table>

<hr>

<h2>行頭 Markdown 系</h2>

<table>
<tr>
<th>Shortcut</th>
<th>動作</th>
</tr>

<tr>
<td>Ctrl + 1</td>
<td><code># 見出し1</code></td>
</tr>

<tr>
<td>Ctrl + 2</td>
<td><code>## 見出し2</code></td>
</tr>

<tr>
<td>Ctrl + 3</td>
<td><code>### 見出し3</code></td>
</tr>

<tr>
<td>Ctrl + 4</td>
<td><code>#### 見出し4</code></td>
</tr>

<tr>
<td>Ctrl + 5</td>
<td><code>##### 見出し5</code></td>
</tr>

<tr>
<td>Ctrl + 6</td>
<td><code>###### 見出し6</code></td>
</tr>

<tr>
<td>Ctrl + O</td>
<td><code>- 箇条書き</code></td>
</tr>

<tr>
<td>Ctrl + .</td>
<td><code>&gt; 引用</code></td>
</tr>
</table>

<p>
Ctrl + O は複数行選択時にも対応。<br>
既存の行頭 Markdown 記号は自動除去されます。
</p>

<hr>

<h2>独自テンプレート機能</h2>

<table>
<tr>
<th>Shortcut</th>
<th>動作</th>
</tr>

<tr>
<td>Ctrl + Shift + Y</td>
<td>テンプレート作成 / 呼び出し</td>
</tr>
</table>

<p>
初回実行時はテンプレート作成画面を表示します。<br>
テンプレート保存後、Ctrl + Shift + Y で
自作テンプレートを使用できます。
</p>

<hr>

<h2>下書き保存</h2>

<table>
<tr>
<th>Shortcut</th>
<th>動作</th>
</tr>

<tr>
<td>Ctrl + S</td>
<td>下書き保存</td>
</tr>
</table>

<p>
既存の Ctrl + S ショートカットを
日報の下書き保存にオーバーライドしています。<br>
Ctrl + Sを使わなくても、17時より前は下書き状態、17時以降 && 600文字以上の記述があれば公開状態で5秒毎にオートセーブされます！
</p>

<hr>

<h2>プレビュー画面、編集画面の切り替え</h2>

<table>
<tr>
<th>Shortcut</th>
<th>動作</th>
</tr>
  
<tr>
<td>Ctrl + P</td>
<td>プレビュー画面、編集画面の切り替え</td>
</tr>
</table>

<p>
プレビューと編集画面を簡単に行き来して確認できます。
</p>

<hr>

<h2>コードブロック例</h2>

```java
System.out.println("Hello");
```

<p>
言語入力ダイアログ付き。<br>
選択範囲をそのままコードブロック化します。
</p>

<hr>

<h1>注意点</h1>

<ul>
<li>
<code>document.execCommand()</code>
を使用しているため、
将来的なブラウザ仕様変更の影響を受ける可能性があります
</li>

<li>
localStorage を使用してテンプレートを保存しています
</li>
</ul>

<hr>

<h1>使用方法</h1>

<h2>Bookmarklet</h2>

<p>
このリポジトリ内の「<a href="https://github.com/miyagitit/NippouTemplater/issues/2">NippouTemplater.js</a>」issueをコピー・ブックマークバーへ貼り付け<br>
あとは日報書くページでクリックすれば動いてくれます。
</p>

<hr>

<h1>謝辞</h1>
<code>Ctrl + S</code>を下書き保存に割り当てるというアイデアをくれた@FumikaShigemasa に感謝します！
<!--EndFragment-->

</body>
</html>
