# 智能闹钟

## 何为智能？

1. 当响铃时间到时，如果你醒了，闹铃就不会再响了
2. 如果今天是法定休息日，即使不是周末，闹铃也不会响；如果今天是法定工作日，即使是周末，闹铃也会响

## 判断逻辑

判断逻辑有点复杂，尽量往简单了说。其实大的逻辑只有两块：

- 判断今天要不要响铃
- 判断手机连没连上充电器

再给每个大逻辑添加完整的判断逻辑，最后出来的逻辑大致是：

- 判断今天要不要响铃
    - 今天是不是节假日换班
        - 是 - 响
        - 否 - 不响
    - 今天是不是节假日
        - 是 - 不响
        - 否 - 响
    - 今天是不是周末
        - 是 - 不响
        - 否 - 响
- 判断手机连没连上充电器
    - 连上 - 把预设好的闹铃打开
    - 没连上 - 把预设好的闹铃关闭

![](https://babyno.top/imgs/posts/2024-02-04-smart-alarm-with-apple-shortcuts/%e6%97%a0%e6%a0%87%e9%a2%98.webp)

如果你想了解更详细的细节，请查看：https://babyno.top/posts/2024/02/smart-alarm-with-apple-shortcuts/

## 下载地址

https://www.icloud.com/shortcuts/a340b291860341a88c0ab59aab208627