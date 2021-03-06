WheelPicker
===
iOS-style scroll wheel picker

![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/ty0x2333/WheelPicker)
![Maven Central](https://img.shields.io/maven-central/v/sh.tyy/wheelpicker)
[![codebeat badge](https://codebeat.co/badges/346d671e-d683-4471-be7d-a3d6f742de86)](https://codebeat.co/projects/github-com-ty0x2333-wheelpicker-master)

Read this in other languages: [*简体中文*](README.zh-cn.md)

Feature
---
1. `Day` / `Night` Mode Support
2. Customizable style
3. Support circular scrolling
4. Support vibration feedback

Preview
---
![Preview](resources/preview.gif)

Component
---
1. DatePicker

    [DatePicker Usage](example/src/main/java/sh/tyy/wheelpicker/example/DatePickerExampleActivity.kt)

    `year-month-day` or `year-month` picker

    support `max` and `min` date limits

    |Day|Night|
    |---|---|
    |![Day](resources/datepicker_day.png)|![Night](resources/datepicker_night.png)|

2. WeekdayTimePicker

    [WeekdayTimePicker Usage](example/src/main/java/sh/tyy/wheelpicker/example/WeekdayTimePickerExampleActivity.kt)

    `weekday-hour-minute` picker

    |Day|Night|
    |---|---|
    |![Day](resources/weektimepicker_day.png)|![Night](resources/weektimepicker_night.png)|

3. DayTimePicker

    [DayTimePicker Usage](example/src/main/java/sh/tyy/wheelpicker/example/DayTimePickerExampleActivity.kt)

    `day-hour-minute` picker

Download
---

Download the latest AAR from [Maven Central](https://search.maven.org/search?q=g:%20sh.tyy%20a:%20wheelpicker) via Gradle:

```gradle
implementation 'sh.tyy:wheelpicker:0.4.0'
```

Custom
---
Customize the style of the item in the same way as the `RecyclerView`.
You need to provide a `BaseWheelPickerView.Adapter` and a `BaseWheelPickerView.ViewHolder`.

***Special note: the itemView of the ViewHolder needs to be a fixed height view.***

> After all, `WheelPicker` is based on `RecyclerView`. Doing so will ensure as much performance and reliability as possible.

Custom WheelPicker please refer to [CustomWheelPickerView.kt](app/src/main/java/sh/tyy/wheelpicker/example/custom/CustomWheelPickerView.kt)

This is what the custom example looks like:
![Custom](resources/custom.png)

**For more complex customizations (e.g. multiple columns), please refer to [WeekdayTimePickerView](WheelPicker/src/main/java/sh/tyy/wheelpicker/WeekdayTimePickerView.kt)**

Inspiration and Reference
---
WheelPicker is inspired by [devilist/RecyclerWheelPicker](https://github.com/devilist/RecyclerWheelPicker).

License
---
WheelPicker is available under the Apache 2.0 license. See the LICENSE file for more info.