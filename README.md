# Vulner-test: No-Code Vulnerability Research Lab

## 概要
このリポジトリは、主要なオープンソース・ノーコードツール（Budibase, Appsmith等）をターゲットとし、[Pentest-mcp](https://github.com/d01ki/Pentest-mcp/tree/main) を活用して未知の脆弱性（0-day）やCVEを特定するための検証環境です。

## ターゲット環境 (Target Stack)
- **Primary Target:** Budibase (Docker-based)
- **Endpoint:** `http://localhost:10000`
- **Goal:** RCE (Remote Code Execution), Auth Bypass, SSRF

## 構築・実行手順

### 1. 環境起動
```bash
docker-compose up -d
```

### 2. 初期設定
- ブラウザで `http://localhost:10000` にアクセス。
- `.env` で設定した管理者資格情報（デフォルト例: `admin@example.com` / `AdminPassword123!`）を使用してログイン。

### 3. 検証の実施
- `Pentest-mcp` のツール群を使用して、スキャンやExploitの検証を行う。

## 免責事項
この検証環境は、学習およびセキュリティ研究の目的で提供されています。許可されていないシステムへの攻撃には使用しないでください。