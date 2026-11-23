# ドキュメント

Kawasemi Rover の設計・開発ドキュメント。全体の開発計画は [design.md](../design.md) を参照。

| フォルダ | 内容 | 関連 Phase |
|---|---|---|
| [01_requirements](01_requirements/) | 目標仕様・利用シナリオ・運用条件 | 全体 |
| [02_mechanical](02_mechanical/) | CAD 設計・3D プリント・屋外対応機構 | 1, 2, 4 |
| [03_kinematics_dynamics](03_kinematics_dynamics/) | 運動学・動力学・歩容・制御 | 1, 2, 3 |
| [04_electronics](04_electronics/) | アクチュエータ・計算機・電源・配線 | 1, 2 |
| [05_ros2](05_ros2/) | ROS 2 ノード・トピック・URDF | 2, 5 |
| [06_simulation_rl](06_simulation_rl/) | MuJoCo / Isaac Lab・RL・Sim2Real | 3 |
| [07_navigation](07_navigation/) | センサ統合・SLAM・Nav2 | 5 |
| [08_ai](08_ai/) | VLA・World Model・Agentic AI・失敗回復 | 6 |
| [09_safety](09_safety/) | 安全対策・試験前チェックリスト | 全体 |
| [10_experiments](10_experiments/) | 実験記録 | 全体 |
| [decisions](decisions/) | 設計判断の記録（ADR） | 全体 |
| [references](references/) | 外部資料・ライセンス調査・論文メモ | 全体 |
