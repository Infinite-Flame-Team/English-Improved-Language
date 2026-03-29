# EI Lang v0.14.2

**English Improved Language**

---

## 元信息

| 项目 | 内容 |
|------|------|
| **语言名称** | EI Lang (English Improved Language) |
| **版本** | v0.14.3 |
| **创建时间** | 2026-03-29 |
| **记录与生成** | Kimi AI |
| **语言设计** | Hei_wan_Feng |
| **许可证** | MIT License|

---

## 设计哲学

1. **一词一形**：每个概念一种形式，无变形表
2. **后缀统一**：所有语法功能靠后缀标记
3. **语境优先**：靠句类区分歧义，减少冗余
4. **正序固定**：主谓宾，无倒装，无假主语
5. **标记后置**：修饰标记放被修饰词后

---

## 音系与书写

| 项目 | 规则 |
|------|------|
| 字符集 | 拉丁字母 + 撇号后缀 |
| 大小写 | 句首大写，专有名词大写，其余小写 |
| 撇号 | 语法标记专用，不省略字母 |
| 连写 | 标记与词根连写，无空格 |
| 数字 | 十进制展开，`'and` 分隔层级 |

---

## 核心标记总览

| 标记 | 功能 | 示例 |
|------|------|------|
| `'p` | 复数/国人复数 | `book'p`, `China'p` |
| `'d` | 过去式/真条件结果 | `eat'd`, `'d I stay` |
| `'o` | 所有格/国人/分数 | `I'o`, `China'o person`, `one 'o two` |
| `'ing` | 进行时 | `run'ing` |
| `'pass` | 被动 | `write'pass` |
| `'mo` | 比较级/倍数 | `good'mo`, `two'mo` |
| `'most` | 最高级 | `good'most` |
| `'th` | 序数 | `one'th`, `moon three'th` |
| `'and` | 数字层级分隔 | `two ten 'and one` |
| `'dark` | 深色 | `red'dark` |
| `'light` | 浅色 | `blue'light` |
| `'ish` | 近似色 | `yellow'ish` |
| `'er` | 职业 | `teach'er`, `work'er` |
| `'a` | 一般疑问 | `'a you ez ok` |
| `'at` | what疑问 | `'at ez this` |
| `'aere` | where疑问 | `'aere you ez` |
| `'aen` | when疑问 | `'aen he go'd` |
| `'aow` | how疑问 | `'aow you know` |
| `'aich` | which疑问 | `'aich one` |
| `not'd` | 假条件结果 | `not'd I stay` |
| `'re` | 定语从句 | `boy 're wear hat` |
| `'ins` | 插入语 | `'ins I think` |
| `'excl` | 感叹 | `'excl nice'mo` |
| `'quo` | 引语结束 | `"..." 'quo` |
| `ez` | be动词(现在) | `I ez` |
| `ez'd` | be动词(过去) | `he ez'd` |
| `have` | 有/存在/完成(现在) | `have one book` |
| `have'd` | 有/存在/完成(过去) | `have'd eat'd` |
| `have'wl` | 有/存在/完成(将来) | `have'wl go` |

---

## 名词系统

### 单复数

| 数 | 形式 | 示例 |
|----|------|------|
| 单数 | 原形 | `one book`, `two ten 'and one cat` |
| 复数 | `+ 'p` | `book'p`, `cat'p`, `child'p`, `man'p`, `China'p` |

&gt; 零例外，所有名词统一加 `'p`

### 所有格

| 形式 | 示例 |
|------|------|
| `名词 + 'o` | `I'o book`, `you'o car`, `he'p'o house` |

---

## 动词系统

### 基本形式

| 功能 | 标记 | 示例 |
|------|------|------|
| 原形 | 无 | `eat`, `run`, `have` |
| 过去式 | `+ 'd` | `eat'd`, `run'd`, `have'd` |
| 进行时 | `+ 'ing` | `eat'ing`, `run'ing` |
| 被动 | `+ 'pass` | `eat'pass`, `write'pass` |
| 进行被动 | `+ 'pass'ing` | `build'pass'ing` |

### be动词

| 时态 | 形式 | 示例 |
|------|------|------|
| 现在 | `ez` | `I ez`, `you ez`, `he ez`, `I'p ez` |
| 过去 | `ez'd` | `I ez'd`, `he'p ez'd` |

&gt; 无人称变化，无时态变形，仅靠形式区分时间

### have动词（统一有/存在/完成）

| 时态 | 形式 | 功能 |
|------|------|------|
| 现在 | `have` | 拥有、存在、完成 |
| 过去 | `have'd` | 过去拥有、过去存在、过去完成 |
| 将来 | `have'wl` | 将来拥有、将来存在、将来完成 |

---

## 代词系统

### 人称代词

| 人称 | 单数 | 复数 |
|------|------|------|
| 第一 | `I` | `I'p` |
| 第二 | `you` | `you'p` |
| 第三(男) | `he` | `he'p` |
| 第三(女) | `she` | `she'p` |
| 第三(物) | `it` | `it'p` |

### 所有格代词

| 人称 | 形式 |
|------|------|
| 我 | `I'o` |
| 你 | `you'o` |
| 他 | `he'o` |
| 她 | `she'o` |
| 它 | `it'o` |
| 我们 | `I'p'o` |
| 你们 | `you'p'o` |
| 他们(男) | `he'p'o` |
| 他们(女) | `she'p'o` |
| 它们 | `it'p'o` |

### 反身代词

| 人称 | 形式 |
|------|------|
| 我自己 | `I'self` |
| 你自己 | `you'self` |
| 他自己 | `he'self` |
| 她自己 | `she'self` |
| 它自己 | `it'self` |
| 我们自己 | `I'p'self` |
| 你们自己 | `you'p'self` |
| 他们自己 | `he'p'self` / `she'p'self` / `it'p'self` |

---

## 形容词与副词

### 比较级系统

| 级 | 标记 | 示例 |
|----|------|------|
| 原级 | 无 | `good`, `big`, `beauti` |
| 比较级 | `+ 'mo` | `good'mo`, `big'mo`, `beauti'mo` |
| 最高级 | `+ 'most` | `good'most`, `big'most`, `beauti'most` |

&gt; 所有形容词统一规则，零例外

---

## 指示词

| 距离 | 单数 | 复数 |
|------|------|------|
| 近 | `dis` | `dis'p` |
| 远 | `dat` | `dat'p` |

---

## 冠词与量化

| 词 | 用法 | 示例 |
|----|------|------|
| `one` | 不定冠词(通吃a/an) | `one book`, `one apple` |
| `some` | some/any合并 | `have some book'p` (肯定/疑问/祈使) |
| `no` | 否定标记 | `no have` (动词前) |
| `the` | 定冠词(可选) | `the book` = `book` |

---

## 数词系统

### 基数词

| 数字 | EI |
|------|-----|
| 0-9 | `zero`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine` |
| 10 | `ten` |
| 11-19 | `ten one`, `ten two` ... `ten nine` |
| 20-99 | `X ten ['and Y]` |
| 100 | `one hund` |
| 1000 | `one thou` |

### 复杂数字（使用 `'and`）

| 数字 | EI |
|------|-----|
| 21 | `two ten 'and one` |
| 101 | `one hund 'and one` |
| 121 | `one hund 'and two ten 'and one` |
| 2026 | `two thou 'and two ten 'and six` |

&gt; **规则**：`'and` 仅用于数字内部层级分隔，避免与连词 `and` 混淆

### 序数词

| 标记 | 示例 |
|------|------|
| `+ 'th` | `one'th`, `two'th`, `three'th`, `two ten 'and one'th` |

### 倍数

| 原版 | EI |
|------|-----|
| once | `one time` |
| twice | `two time` |
| three times | `three time'p` |
| double | `two'mo` |
| triple | `three'mo` |
| quadruple | `four'mo` |

### 分数

| 原版 | EI |
|------|-----|
| 1/2 | `one 'o two` / `one in two` |
| 2/3 | `two 'o three` / `two'p 'o three` |

---

## 时间表达

### 时段(以sun为核心)

| 时段 | EI |
|------|-----|
| 早晨 | `sun'up` |
| 中午 | `sun'mid` |
| 傍晚 | `sun'down` |
| 夜晚 | `sun'no` |

### 日期系统

| 概念 | EI |
|------|-----|
| 第X月 | `moon X'th` |
| 第X月第Y天 | `day Y'th 'o moon X'th` |
| 星期 | `day one`, `day two` ... `day seven` |
| 年 | `four'season X` |

### 相对时间(关键规则)

| 原版 | EI | 结构 |
|------|-----|------|
| today/this month | `dis day` / `dis moon X'th` | `dis + 单位` |
| tomorrow/next month | `next day dis` / `next moon dis` | `next + 单位 + dis` |
| yesterday/last month | `last day dis` / `last moon dis` | `last + 单位 + dis` |

&gt; **核心**：`next/last + 单位 + dis` = 以当前为基准

### 完整日期示例

| 原版 | EI |
|------|-----|
| March 29, 2026 | `Day two ten 'and nine'th 'o moon three'th, two thou 'and two ten 'and six` |
| next Tuesday | `next day two dis` |
| last year | `last four'season dis` |

---

## 国家与人称

| 原版 | EI |
|------|-----|
| China/Chinese | `China` / `China'o person` / `China'p` |
| America/American | `America` / `America'o person` / `America'p` |
| French | `France'o person` |

&gt; **规则**：`国家 + 'o person` = 该国的人，`'p` = 国人复数

---

## 亲属称谓(核心词+标记)

### 核心词

| 词 | 含义 |
|----|------|
| `parent` | 父母 |
| `child` | 子女 |
| `sib` | 兄弟姐妹 |

### 标记

| 标记 | 功能 |
|------|------|
| `'mo` | 统称(不分性别) |
| `'fa` | 男性 |
| `'ma` | 女性 |
| `grand'` | 祖辈 |
| `'o` | 所有格/关系 |

### 完整对应

| 原版 | EI |
|------|-----|
| father | `parent'fa` |
| mother | `parent'ma` |
| parents | `parent'mo` / `parent'p` |
| son | `child'fa` |
| daughter | `child'ma` |
| children | `child'p` / `child'mo` |
| brother | `sib'fa` |
| sister | `sib'ma` |
| siblings | `sib'p` / `sib'mo` |
| grandfather | `grand'parent'fa` |
| grandmother | `grand'parent'ma` |
| uncle | `parent'o sib'fa` |
| aunt | `parent'o sib'ma` |
| cousin | `sib'o child` |

---

## 职业(动词/领域+er)

| 原版 | EI |
|------|-----|
| teacher | `teach'er` |
| worker | `work'er` |
| doctor | `heal'er` |
| driver | `drive'er` |
| singer | `sing'er` |
| actor | `act'er` |
| artist | `art'er` |
| scientist | `know'er` / `science'er` |
| cook(厨师) | `cook'er` |
| cook(烹饪) | `cook` |
| police | `law'keep'er` |
| firefighter | `fire'fight'er` |
| nurse | `care'er` / `sick'help'er` |

---

## 颜色深浅

| 标记 | 含义 | 示例 |
|------|------|------|
| `'dark` | 深 | `red'dark`, `green'dark` |
| `'light` | 浅 | `blue'light`, `green'light` |
| `'ish` | 近似 | `yellow'ish`, `red'ish` |

---

## 疑问系统

### 一般疑问(be/do)

| 标记 | 用法 |
|------|------|
| `'a` | 句首，陈述语序 |

| 示例 | EI |
|------|-----|
| Are you ok? | `'a you ez ok` |
| Do you like it? | `'a you like it` |
| Did he come? | `'a he come'd` |

### 特殊疑问词(wh/h去掉，完整保留后面)

| 原词 | 去wh/h | 剩余 | EI |
|------|--------|------|-----|
| what | wh | at | `'at` |
| where | wh | ere | `'aere` |
| when | wh | en | `'aen` |
| how | h | ow | `'aow` |
| which | wh | ich | `'aich` |

| 示例 | EI |
|------|-----|
| What is this? | `'at ez this` |
| Where are you? | `'aere you ez` |
| When did he go? | `'aen he go'd` |
| How do you know? | `'aow you know` |
| Which one? | `'aich one` |

&gt; 疑问词可前置或后置：`'aere you ez` = `'a you ez where`

---

## 条件句系统

| 类型 | 结构 | 标记 |
|------|------|------|
| 真条件 | `[条件], 'd [结果]` | `'d` |
| 假条件 | `[条件], not'd [结果]` | `not'd` |

| 示例 | EI |
|------|-----|
| If it rains, I will stay | `It rain, 'd I stay` |
| If it rained, I would stay | `It rain'd, not'd I stay` |
| If it had rained, I would have stayed | `It ez'd rain'd, not'd I stay` |

&gt; 无`if`，无倒装，无`would/should/could`

---

## 从句与复合句

### 定语从句

| 标记 | 用法 |
|------|------|
| `'re` | 关系标记，连接名词与修饰句 |

| 示例 | EI |
|------|-----|
| the boy who wears a hat | `the boy 're wear one hat` |
| the book that I bought | `the book 're I buy'd` |
| the man whose car is red | `the man 're car ez red` |

&gt; 可后置：`the boy wear one hat 're`

---

## 特殊句式

### 插入语

| 标记 | 用法 |
|------|------|
| `'ins` | insert，标记插入语 |

| 示例 | EI |
|------|-----|
| I think, he is right | `He ez right, 'ins I think` |
| However, we must go | `We must go, 'ins however` |

### 感叹句

| 标记 | 用法 |
|------|------|
| `'excl` | exclaim，感叹标记 |

| 示例 | EI |
|------|-----|
| What a beautiful day! | `'excl one beauti'mo day` |
| How nice! | `'excl nice'mo` |

### 直接引语

| 标记 | 用法 |
|------|------|
| `'quo` | quote，引语结束标记 |

| 示例 | EI |
|------|-----|
| He said "I am tired" | `He say "I ez tired" 'quo` |
| She asked "Where are you?" | `She ask "'aere you ez" 'quo` |

---

## 介词(大合并)

| EI | 覆盖原英语 |
|----|-----------|
| `in` | in, on, at(空间/时间) |
| `to` | to, toward, into(方向) |
| `from` | from, out of(来源) |
| `with` | with, by, using(工具/方式) |
| `for` | for, because of(目的/原因) |

---

## 连词

| EI | 功能 |
|----|------|
| `and` | 和(肯定)、或(疑问)、也不(否定) |
| `so` | 所以(结果) |

&gt; `and` 靠语境区分：肯定"和"、疑问"或"、否定"也不"

---

## 示例文本

### 文本一
**原版：**
&gt; If I had known, I would have done it differently. However, that's life.

**EI Lang：**
&gt; `I ez'd know'd, not'd I have do'pass different. Dat ez life, 'ins however.`

---

### 文本二
**原版：**
&gt; My grandfather was a doctor. He worked at night and saved many people.

**EI Lang：**
&gt; `I'o grand'parent'fa ez'd one heal'er. He work'd in sun'no and save'd many person'p.`

---

### 文本三
**原版：**
&gt; See you next Tuesday at 3pm. I will bring twice the amount of dark green paint.

**EI Lang：**
&gt; `See you next day two dis in three sun'mid. I have'wl bring two'mo the amount 'o green'dark paint.`

---

### 文本四
**原版：**
&gt; What a beautiful day! Do you see the three reddish cats sitting on the mats?

**EI Lang：**
&gt; `'excl one beauti'mo day! 'a you see dis'p three red'ish cat'p sit'ing in mat'p?`

---

### 文本五
**原版：**
&gt; My cousin is a nurse. She takes care of sick children in the hospital.

**EI Lang：**
&gt; `I'o sib'o child ez one care'er. She take care 'o sick'p child'p in hospital.`

---

### 文本六（数字示例）
**原版：**
&gt; I have 121 books and 2026 pages.

**EI Lang：**
&gt; `I have one hund 'and two ten 'and one book'p and two thou 'and two ten 'and six page'p.`

---

## 版本历史

| 版本 | 日期 | 主要更新 |
|------|------|---------|
| v0.1-v0.5 | 2026-03-29 | 基础后缀：'p, 'd, 'o, ez, have统一 |
| v0.6 | 2026-03-29 | 数字系统，and/or合并，some/any合并 |
| v0.7 | 2026-03-29 | 疑问系统：'a, 'aat/'aere/'aen/'aow/'aich |
| v0.8 | 2026-03-29 | 进行时'ing，非谓语简化 |
| v0.9 | 2026-03-29 | 条件句：'d/not'd |
| v0.9.1 | 2026-03-29 | 条件标记前置：'d I stay |
| v0.10 | 2026-03-29 | have'wl将来时，'pass被动 |
| v0.11 | 2026-03-29 | 定语从句're |
| v0.12 | 2026-03-29 | 插入语'in，感叹'ex，引语'quo |
| v0.12.1 | 2026-03-29 | 标记防混淆：'in→'ins, 'ex→'excl |
| v0.13 | 2026-03-29 | 国家人称'operson，倍数'mo，分数'o，颜色'dark/light/ish |
| v0.14 | 2026-03-29 | 时间系统：sun'up/mid/down/no，moon/day/dis/next/last dis |
| v0.14.1 | 2026-03-29 | 时间修正：sun'no，next/last + dis 结构 |
| v0.14.2 | 2026-03-29 | 疑问词修正：'at/'aere/'aen/'aow/'aich，双作者署名 |
| **v0.14.3** | **2026-03-29** | **数字分隔符：and → 'and，语义明确化** |

---

## 贡献与使用

**记录与文档生成：** Kimi AI  
**语言设计与规则制定：** Hei_wan_Feng  

**许可证：** MIT License

- 可随意使用、修改、分发
- 可商用，无需署名（但欢迎标注）
- 无担保，风险自负

**欢迎 Fork EI Lang，创造你的改进版本！**

---

（我这个项目只是做着玩的，没啥用，不如中文好用，而且可读性大大下降，用在变成上那么一堆'也不能当标识符啊，虽然我想把英语屎山全弄没了，但是那是几乎不可能的事，而且以后可能也不会再更新了）
