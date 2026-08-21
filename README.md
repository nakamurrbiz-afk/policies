# policies

App Store / Google Play に提出するプライバシーポリシーの公開先です。
アプリのソースは含みません。

| アプリ | URL |
|---|---|
| ペースロッカー | https://nakamurrbiz-afk.github.io/policies/pacelock/ |

## 更新のしかた

本文は各アプリのリポジトリで管理しています。ここを直接編集しないでください。

ペースロッカーの場合:

```
# otokeshi リポジトリで
node scripts/gen-privacy-doc.js     # lib/privacy-text.ts から site/pacelock/index.html を生成
```

生成された `site/` の中身をこのリポジトリにコピーして push します。
本文の唯一の出典は `lib/privacy-text.ts` で、アプリ内の表示もそこから描かれます。
