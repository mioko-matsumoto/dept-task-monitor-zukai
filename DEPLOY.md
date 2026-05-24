# 図解デプロイ手順

## 1. プレビュー（ローカル確認）

ブラウザでこのファイルを直接開く:
```
open /Users/mioko/dept-task-monitor/zukai/index.html
```

## 2. Surgeにデプロイ

ターミナルで:
```bash
cd /Users/mioko/dept-task-monitor/zukai
surge .
```

**初回のみ** メールアドレス/パスワードを聞かれる（無料アカウント作成）:
- `email:` 自分のメールアドレス
- `password:` 任意のパスワード

ドメイン入力:
- `domain:` Enterだけ押せばランダムなURLが付与される
  - 例: `https://abcd-xxxx.surge.sh`
- 自分で指定する場合は `levela-dept-task.surge.sh` のような形で入力

完了したらURLが表示される。それを提出フォームに貼る。

## 3. 後からデプロイし直したい場合

同じドメインに上書きデプロイ:
```bash
cd /Users/mioko/dept-task-monitor/zukai
surge . your-domain.surge.sh
```

## 4. デプロイしたサイトを消したい場合

```bash
surge teardown your-domain.surge.sh
```

---

## ⚠️ 提出前チェックリスト

- [ ] `screenshot.png` 内の個人情報がマスクされているか確認
- [ ] 図解(index.html)の文言に誤りがないか確認
- [ ] ローカルブラウザで開いて全体の見た目を確認
- [ ] Surgeにデプロイ
- [ ] デプロイURLを開いて公開状態で表示されるか確認
- [ ] そのURLを提出フォームに貼る
