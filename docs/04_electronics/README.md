# 04 電気・電子

アクチュエータ、計算機、電源、配線の設計。

- アクチュエータの比較と選定（トルク、速度、重量、価格、エンコーダ）
- 計算機構成（メイン: Jetson Orin Nano に決定 → [0001](../decisions/0001-main-computer-jetson-orin-nano.md)。マイコン: STM32 / ESP32 は未定）
- Jetson Orin Nano の電源（最大 25 W 程度、モータ系と分離）と放熱
- 電源系（バッテリー、BMS、ヒューズ、電源監視）
- 通信（CAN など）と配線図
- 非常停止回路

関連: [design.md §3, §12.2](../../design.md)
