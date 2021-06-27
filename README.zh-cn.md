WheelPicker
===
iOS风格的滚轮选择器


[![codebeat badge](https://codebeat.co/badges/346d671e-d683-4471-be7d-a3d6f742de86)](https://codebeat.co/projects/github-com-ty0x2333-wheelpicker-master)

其他语言版本: [*English*](README.md)

预览
---
![Preview](resources/preview.gif)

|亮色模式|暗色模式|
|---|---|
|![Day](resources/day.png)|![Night](resources/night.png)|

自定义
---
自定义item的样式的方式如同 `RecyclerView` 一样.
你需要提供一个 `BaseWheelPickerView.Adapter` 和 `BaseWheelPickerView.ViewHolder`.

需要特别注意的是: ViewHolder 的 itemView 需要是一个固定高度的视图.

> 毕竟 `WheelPicker` 是基于 `RecyclerView` 的. 这样做可以尽可能保证其性能和可靠性.

自定义 WheelPicker 请参考 [CustomWheelPickerView.kt](app/src/main/java/sh/tyy/wheelpicker/example/custom/CustomWheelPickerView.kt)

这是自定义示例的样子:
![Custom](resources/custom.png)

**更复杂的自定义 (例如 多列), 请参考 [WeekdayTimePickerView](WheelPicker/src/main/java/sh/tyy/wheelpicker/WeekdayTimePickerView.kt)**

灵感及参考
---
WheelPicker 灵感来自于 [devilist/RecyclerWheelPicker](https://github.com/devilist/RecyclerWheelPicker).

License
---
WheelPicker is available under the Apache 2.0 license. See the LICENSE file for more info.