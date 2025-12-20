# 開発者からのお知らせの更新方法
## 動作原理
* アプリ起動時に notices.html のお知らせを読み込む
* ポップアップ、タイムライン表示する

## 更新方法
以下を notices.html に追加
        
        <div class="notice-record">
            
            <span class="data-field" data-type="id">1001</span>
            
            <span class="data-field" data-type="title">【テスト】イベントを実施します</span>
            
            <span class="data-field" data-type="content">【テスト】ここでオフ会を実施します。ご希望の方は、本お知らせをクリックし、予約してください。</span>
            
            <span class="data-field" data-type="published_at">2025-12-14</span>
            
            <span class="data-field" data-type="url">https://irukabando.github.io/irubabandoApp/</span>
            
            <span class="data-field" data-type="is_critical">false</span>
            
        </div>

* id は連番
* url は本ディレクトリに html を作るなどして指定
* お知らせは念のため1つ残す
