# Compose 练习手册

> 本文件包含 10 个 Compose 练习，从基础到进阶

---

## 环境命令

```bash
./gradlew assembleDebug   # 构建调试 APK
./gradlew test           # 运行单元测试
./gradlew connectedCheck # 运行 instrumented 测试
```

---

## 练习 1：登录/注册界面

**涉及组件**：TextField、OutlinedTextField、Button
**核心技能**：表单验证、用户输入处理
**文档参考**：
- [Validate input as the user types](kb://android/develop/ui/compose/quick-guides/content/validate-input)
- [Text in Compose](kb://android/develop/ui/compose/text/index)
- [Configure text fields](kb://android/develop/ui/compose/text/user-input)

**实现要点**：
- 单账号登录界面
- 用户名/密码输入框
- 登录按钮
- 表单验证（空检查、格式验证）

**验证方式**：在设备上运行，观察输入验证效果

---

## 练习 2：列表展示

**涉及组件**：LazyColumn、LazyRow、Card
**核心技能**：列表渲染、Item 点击事件
**文档参考**：[Lists and grids](kb://android/develop/ui/compose/lists)

**实现要点**：
- 展示文章列表
- 每个 Item 包含：标题、摘要、图片
- 使用 Card 包装
- Item 点击事件

**验证方式**：运行后上下滑动列表，点击 Item

---

## 练习 3：底部导航栏

**涉及组件**：Scaffold、BottomNavigation、NavigationBar
**核心技能**：脚手架布局、导航状态管理
**文档参考**：
- [Navigation bar](kb://android/develop/ui/compose/components/navigation-bar)
- [Navigation Compose](kb://android/develop/ui/compose/navigation)

**实现要点**：
- 带底部导航的壳
- 三个 Tab：首页、搜索、我的
- Tab 切换状态保持

**验证方式**：运行后点击不同 Tab，观察页面切换

---

## 练习 4：计数器应用

**涉及 API**：remember、mutableStateOf、State hoisting
**核心技能**：状态声明与更新、状态提升
**文档参考**：[State in Jetpack Compose](kb://android/develop/ui/compose/state)

**实现要点**：
- 点击按钮加减数字
- 理解 Composable 状态与重组
- 状态提升到父组件

**验证方式**：运行后点击按钮，观察数字变化

---

## 练习 5：待办事项列表

**涉及组件/架构**：ViewModel、StateFlow、增删改查
**核心技能**：单向数据流（UDF）、ViewModel 集成
**文档参考**：
- [StateFlow and SharedFlow](kb://android/kotlin/flow/stateflow-and-sharedflow)
- [UI State Production and Management](kb://android/topic/architecture/ui-layer/state-production)
- [Unidirectional data flow in Compose](kb://android/develop/ui/compose/architecture)

**实现要点**：
- Todo list
- ViewModel 管理 StateFlow
- 支持：添加、完成、删除

**验证方式**：运行后添加任务、标记完成、删除

---

## 练习 6：表单与验证

**涉及组件**：多个 TextField 联动、实时验证反馈
**核心技能**：跨组件状态共享、验证逻辑
**文档参考**：[Validate input as the user types](kb://android/develop/ui/compose/quick-guides/content/validate-input)

**实现要点**：
- 注册表单：用户名、邮箱、密码、确认密码
- 实时显示验证错误
- 密码确认一致性检查

**验证方式**：输入不同内容，观察实时验证反馈

---

## 练习 7：自定义动画

**涉及 API**：animateFloatAsState、AnimatedVisibility、transition
**核心技能**：值动画、可见性动画
**文档参考**：
- [Value-based animations in Compose](kb://android/develop/ui/compose/animation/value-based)
- [Animation modifiers and composables](kb://android/develop/ui/compose/animation/composables-modifiers)
- [Choose an animation API](kb://android/develop/ui/compose/animation/choose-api)

**实现要点**：
- 卡片展开/收起动画
- 按钮点击反馈动画

**验证方式**：点击卡片观察展开动画，点击按钮观察反馈

---

## 练习 8：Canvas 绘图

**涉及 API**：Canvas、drawBehind、DrawScope
**核心技能**：自定义绘制、形状组合
**文档参考**：
- [Graphics in Compose](kb://android/develop/ui/compose/graphics/draw/overview)
- [Drawing and graphics modifiers in Compose](kb://android/develop/ui/compose/graphics/draw/modifiers)
- [Shapes in Compose](kb://android/develop/ui/compose/graphics/draw/shapes)

**实现要点**：
- 使用 Canvas 绘制自定义进度环
- 或绘制饼图
- 或绘制简单图形组合

**验证方式**：运行后观察自定义绘制的图形

---

## 练习 9：复杂列表

**涉及组件**：LazyColumn 多类型 Item
**核心技能**：内容类型分类、差异化 UI
**文档参考**：[Build a list using multiple item types](kb://android/develop/ui/compose/quick-guides/content/build-list-multiple-item-types)

**实现要点**：
- 动态 feeds 流
- 三种帖子类型：纯文本、图片帖子、视频帖子
- 每种类型不同的 UI 展示

**验证方式**：运行后列表中应看到不同类型的帖子

---

## 练习 10：仿社交媒体动态页面

**涉及组件**：综合前面所有技能
**核心技能**：完整页面开发、性能考量
**文档参考**：
- [Lists and grids](kb://android/develop/ui/compose/lists)
- [Navigation Compose](kb://android/develop/ui/compose/navigation)

**实现要点**：
- 顶部 AppBar + 底部 Tab 导航
- 动态列表（图片、视频、文字）
- 点赞、评论、分享按钮交互
- 下拉刷新、上拉加载更多
- 状态管理与数据流

**验证方式**：完整运行，观察整体交互效果

---

## 练习安排

- 代码注释：中文
- 每次练习时间：1-2 小时
