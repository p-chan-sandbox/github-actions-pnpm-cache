# github-actions-pnpm-cache

## やりたいこと

GitHub Actions と pnpm で、キャッシュを用いたインストールのベストプラクティスを見つける。

## 分からないこと

### 複数の方法が見つかる

`github actions pnpm cache` とかでググると、複数の方法が見つかる。

1. [setup-node のドキュメントに書かれた方法](https://github.com/actions/setup-node/blob/main/docs/advanced-usage.md#caching-packages-data)
2. [pnpm のドキュメントに書かれた方法](https://pnpm.io/ja/continuous-integration#github-actions)

1 の方が簡単そうなので、1 でいけるなら 1 でいきたい。

### キャッシュしたデータをリストアする方法

分からん。

## 結論

setup-node の pnpm でキャッシュして、pnpm install すれば、よしなにキャッシュを再利用してくれる

## 調べたこと

https://x.com/p1ch_jp/status/1743053977963594155?s=20
