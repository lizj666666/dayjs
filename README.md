# dayjs
Day.js ：用小巧的身形满足你
Moment.js 是一个大而全的 JS 时间库，很大地方便了我们处理日期和时间。但是 Moment.js太重了(200k+ with locals)，可能一般项目也只使用到了她几个常用的API。虽然社区也有几个轻量的时间库，要想迁移过去又会增加新的学习和迁移成本。
Day.js 是一个轻量的 JavaScript 时间日期处理库，和 Moment.js 的 API 设计保持完全一样. 如果你曾经用过 Moment.js, 那么你已经知道如何使用 Day.js
* 和 Moment.js 相同的 API 和用法
* 不可变数据 (Immutable)
* 支持链式操作 (Chainable)
* 仅 2kb 大小的微型库
* 全浏览器兼容
### 创建
```
  dayjs() // 当前时间

  dayjs('1995-12-25') // 1995-12-25

  dayjs(Date.now() - 24 * 60 * 60 * 1000) // 昨天
```
### 格式化
``` 
  dayjs().format('YYYY年MM月DD日 HH:mm:ss') // 2018年08月08日 00:00:00

  dayjs().format('[YYYY]') // "[2018]"。[] 里的会原样输出。
```
### 操作
```
  dayjs().add(7, 'days') // 之后的第7天

  dayjs().subtract(1, 'months') // 上个月

  dayjs().startOf('months') // 获取一月初

  dayjs().endOf('year') // 获取一年年末
```
### 查询
```
  dayjs('2010-10-20').isBefore('2010-10-21') // 早于

  dayjs('2010-10-20').isAfter('2010-10-19') // 晚于

  dayjs().isLeapYear() // 闰年
```
