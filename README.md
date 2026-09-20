# vLeco (`vigle.co`) — System & Brand Specification

> **Official Open Source Standard Site & Repository**  
> Managed as a new project within **株式会社asfact**  

---

## 1. Overview & Brand Identity

**vLeco** (ブイレコ) は、現代人の生活・身体・ITシステムにおける雑音や無駄（Vanofino）を断絶し、本質的な生命力（Vigleco）を取り戻すための、ブランドおよび統合システムエコシステムです。


* **Official Domain:** [https://vigle.co](https://vigle.co)
* **Standard Brand Mark:** `vLeco`（小文字の `v` と大文字の `L` による視覚的構造）
* **Current Operating Entity:** **株式会社asfact**
* **Project Name:** **vLeco** (フリガナ: ブイレコ)

---

## 2. Web Architecture & Visual Features

本リポジトリで公開されているランディングページ（`index.html`）は、以下の要素で構成されています。

1. **Hexagonal Heart Dot Logo (六角形ドットハート)**
   - 2Dグラフィック過多を排した低認知負荷デザイン。
2. **Revolving Orbit System (背景周回リング)**
   - ブランドの核となる概念（`Ordigo`, `Nutro-Regado`, `Kuir-Artigo`, `Korp-Kultivado`, `Spatio-Optimumo`, `Ordo`, `Logit`, `Vivi la Nunon`, `Kultivi la Ĉirkaŭaĵon`, `Kompari kun Si Mem`）が、円周上を自動周回。
   - **初期表示制限 (Default: 6)** および **軽量フランク・ランダム抽出算法 (Fisher-Yates)** を搭載。
3. **Control Overlay**
   - フッターの `Orbit Settings` より、最大表示数・回転速度・半径・コンテンツ上下位置・アクセントカラーの即時書き換えが可能。
   - 変更した設定はURLクエリに反映されるため、同じ表示状態をURLで共有できます。
4. **Keyword Definition**
   - 表示キーワードと初期表示設定は `site-config.json` で管理します。
   - `keywords.json` は旧形式のフォールバックとして残しています。
   - アクセス時にランダム順へ並び替え、各キーワードが一周するとフェードアウトして次のキーワードへ切り替わります。
   - Orbit Settingsで変更した内容はブラウザに保存され、次回アクセス時にも反映されます。
5. **Braille Tool**
   - `braille.html` でLatin / Esperanto文字の簡易点字化とデコードができます。
   - 入力内容は `?mode=encode&text=...` または `?mode=decode&text=...` のURLクエリで保持できます。

### URL Query Settings

```text
https://vigle.co/?max=6&radius=0.38&speed=0.0012&offset=-4&color=ff7b54
```

* `max`: 表示数 (`1`〜`12`)
* `radius`: 周回半径 (`0.15`〜`0.55`)
* `speed`: 周回速度 (`0.0002`〜`0.005`)
* `offset`: Orbit・六角形・トップコンテンツの上下位置 (`-18`〜`12`、単位は `vh`)
* `color`: アクセントカラー
* `words`: カンマ区切りのキーワード上書き

---

## 3. Rights & Corporate Information

* **Current Owner / Management:** 株式会社asfact
