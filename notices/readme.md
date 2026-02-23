# 開発者からのお知らせの更新方法
## 動作原理
* スクレイピング時に notices.html のお知らせを読み込む
* お知らせのテーブルに追加される

## 更新方法
以下を notices.html に追加

```
        <div class="notice-record">
            
            <span class="data-field" data-type="id">【xxxx】</span>
            
            <span class="data-field" data-type="title">【タイトル】</span>
            
            <span class="data-field" data-type="content">【内容】</span>
            
            <span class="data-field" data-type="published_at">【yyyy-mm-dd】</span>
            
            <span class="data-field" data-type="url">【https://irukabando.github.io/irubabandoApp/notices/[xxxx]_notice.html】</span>
            
            <span class="data-field" data-type="is_critical">false</span>
            
        </div>
```

* id は4桁の連番
* title, content はお知らせの内容に合わせて適宜書き換え
* published_at はお知らせの公開日
* url はお知らせの詳細ページへのリンク
* 詳細ページは，本ディレクトリに html を事前に作成しておく
* url は，[id]_notice.html を基本とする
* is_critical は未使用だが，ひとまず false 固定
* お知らせは1つ残す（Parsing Error が出るため）
