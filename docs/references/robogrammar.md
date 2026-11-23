# RoboGrammar: Graph Grammar for Terrain-Optimized Robot Design

- 著者: Allan Zhao, Jie Xu, Mina Konaković Luković, Josephine Hughes, Andrew Spielberg, Daniela Rus, Wojciech Matusik（MIT）
- 発表: ACM Transactions on Graphics 39(6), SIGGRAPH Asia 2020
- プロジェクトページ: https://people.csail.mit.edu/jiex/papers/robogrammar/
- 論文: https://people.csail.mit.edu/jiex/papers/robogrammar/paper.pdf
- コード: https://github.com/allanzhao/RoboGrammar （MIT ライセンス、2023 年 10 月にアーカイブ済み・更新停止）

## 概要

- ロボットの設計をグラフで表し、少数のグラフ文法規則で、製作可能な構成の空間を表現する。設計は文法規則の適用列として表される。
- Graph Heuristic Search で設計空間を探索する。作りかけの設計から到達できる最良性能を予測する関数を学習し、見込みの高い候補から先に調べる。
- 各候補の制御器は MPC で最適化する。
- 地形ごとに、性能の高い構成と制御器の組を得る。
- コードに含まれる地形タスク: 平地（Flat）、凹凸（Ridged）、溝（Gap）、低摩擦面（FrozenLake）

## Kawasemi Rover への応用

- 構成の探索までは行わない。12 自由度・1 脚 3 自由度の四足構成は固定し、脚長・股関節配置・胴体寸法・足先形状・関節可動範囲などの寸法パラメータを最適化の対象にする。
- 評価は MuJoCo で行い、対象地形（平地・芝生・砂利・段差・斜面）を模した地形を用意する。
- 複数の地形を同時に扱うため、多目的最適化が必要になる。
- 設計計画: [design.md §6.3](../../design.md)、詳細は [02_mechanical](../02_mechanical/) に記録する。

## 未確認事項

- 論文中の定量結果（地形ごとの性能、ベースラインとの比較）
- 使用している物理シミュレータの詳細
- 実機での検証の有無

## 関連研究

- Multi-Objective Graph Heuristic Search for Terrestrial Robot Design（Xu, Spielberg, Zhao, Rus, Matusik, ICRA 2021）
  https://people.csail.mit.edu/jiex/papers/MOGHS/index.html
