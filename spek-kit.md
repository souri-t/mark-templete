---
marp: true
theme: ownstyle-theme
paginate: true
title: サンプルスライド
description: サンプルスライドです。
---

<!-- _class: title -->
<!-- _paginate: false -->


<div></div>


# Spec Kitの活用

hogehoge

---

<!-- _class: content-image -->
# Spec Kitとは
Spec Kitは、GitHubが2025年9月に発表した、仕様駆動開発（Spec-Driven Development）を支援するオープンソースのツールキット。
AIを活用してソフトウェア開発の仕様策定からタスク洗い出しまで行える。
[github/spec-kit](https://github.com/github/spec-kit.git)

![w:500px](https://placehold.jp/300x200.png)

---

# Spec Kitの準備
1.  Spec Kitの実行
  ```bash
  uvx --from git+https://github.com/github/spec-kit.git specify init --here
  ```
2. 使用しているAIツールなどが聞かれるため質問に答えていく。

---

# Spec Kitの進め方

<ul class="timeline">
  <li class="timeline-item">
    <h3>Phase 1: 仕様策定（/specify）</h3>
    <p>AIに完成物のイメージを伝え、仕様を考えてもらう。</p>
  </li>
  <li class="timeline-item">
    <h3>Phase 2: 不明点の明確化（/clarify）</h3>
    <p>仕様策定で不明確な箇所を対話的に補完する。</p>
  </li>
  <li class="timeline-item">
    <h3>Phase 3: 計画立案（/plan）</h3>
    <p>仕様を元に実装計画を練る。</p>
  </li>
  <li class="timeline-item">
    <h3>Phase 4: タスクの洗い出し（/tasks）</h3>
    <p>task.mdファイルとしてTodoリストを作成する。</p>
  </li>
  <li class="timeline-item">
    <h3>Phase 5: 実装</h3>
    <p>計画に沿って実装する。</p>
  </li>
</ul>


<style scoped>
  .timeline {
    list-style: none;
    padding: 0;
    position: relative;
  }
  .timeline:before {
    content: '';
    position: absolute;
    top: 20px;
    left: 20px;
    bottom: 20px;
    width: 4px;
    background: #ddd;
  }
  .timeline-item {
    position: relative;
    margin-bottom: 30px;
    padding-left: 50px;
  }
  .timeline-item:before {
    content: '';
    position: absolute;
    left: 10px;
    top: 12px;
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background: white;
    border: 4px solid #4A90E2;
  }
  .timeline-item h3 {
    margin: 0 0 5px 0;
    font-size: 1.2em;
    color: #4A90E2;
  }
  .timeline-item p {
    margin: 0;
    font-size: 0.9em;
  }
</style>

