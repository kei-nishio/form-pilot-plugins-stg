# form-pilot-plugins-stg

form-pilot の**検証環境（staging）**用のプラグインです。開発・検証用で、利用者の方は本番用の [kei-nishio/form-pilot-plugins](https://github.com/kei-nishio/form-pilot-plugins) を使ってください。

入れると、AI が staging の MCP サーバー（`https://form-pilot-stg.plutoid.jp/mcp`）につながります。本番用のプラグインと同時に入れておけます。

## Claude Code で使う

```bash
claude plugin marketplace add kei-nishio/form-pilot-plugins-stg
claude plugin install form-pilot-stg@form-pilot-plugins-stg
claude mcp login plugin:form-pilot-stg:form-pilot-stg
```

## Codex で使う

```bash
codex plugin marketplace add kei-nishio/form-pilot-plugins-stg
codex plugin add form-pilot-stg@form-pilot-plugins-stg
codex mcp login form-pilot-stg
```

ブラウザで Google のログイン画面が開きます。staging に登録した Google アカウントを選び、「許可する」を押してください。

## 削除する

```bash
# Claude Code
claude plugin uninstall form-pilot-stg@form-pilot-plugins-stg
claude plugin marketplace remove form-pilot-plugins-stg

# Codex
codex plugin remove form-pilot-stg@form-pilot-plugins-stg
codex plugin marketplace remove form-pilot-plugins-stg
```
