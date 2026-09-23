# policies

App Store / Google Play に提出するプライバシーポリシーの公開先です。
アプリのソースは含みません。

| アプリ | URL |
|---|---|
| ペースロッカー | https://nakamurrbiz-afk.github.io/policies/pacelock/ |
| ParkWash | https://nakamurrbiz-afk.github.io/policies/parkwash/ （プライバシー `privacy/`・サポート `support/`・利用規約 `terms/`） |

## 更新のしかた

本文は各アプリのリポジトリで管理しています。ここを直接編集しないでください。

ペースロッカーの場合:

```
# otokeshi リポジトリで
node scripts/gen-privacy-doc.js     # lib/privacy-text.ts から site/pacelock/index.html を生成
```

生成された `site/` の中身をこのリポジトリにコピーして push します。
本文の唯一の出典は `lib/privacy-text.ts` で、アプリ内の表示もそこから描かれます。

ParkWash の場合:

```
# parkwash リポジトリで
node scripts/gen-site.mjs                    # legal/*.md から site/ を生成
node scripts/sync-policies.mjs ../policies   # site/ をこのリポジトリの parkwash/ に写す
```

本文の唯一の出典は parkwash の `legal/*.md` です。弁護士レビューが済むまでは各ページに「下書き」の帯が出ます。
