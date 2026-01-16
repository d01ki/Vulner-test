# Project: No-Code Vulnerability Research Lab

## 概要
このリポジトリは、主要なオープンソース・ノーコードツール（Budibase, Appsmith等）をターゲットとし、`Pentest-mcp` (https://github.com/d01ki/Pentest-mcp/tree/main) を活用して未知の脆弱性（0-day）やCVEを特定するための検証環境です。

## ターゲット環境 (Target Stack)
- **Primary Target:** Budibase (Docker-based)
- **Endpoint:** `http://localhost:10000`
- **Goal:** RCE (Remote Code Execution), Auth Bypass, SSRF

## 構築・実行手順
1. **環境起動:**
   ```bash
   docker-compose up -d
