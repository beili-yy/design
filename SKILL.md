---
name: ued-design-system
description: 宝思派小程序 UED 设计系统，用于界面设计、Figma 设计、设计审核和前端交付。
---

# UED Design System

## 核心目标

进行设计、修改设计稿、设计审核或前端交付时，
必须优先读取并遵循现有设计规范和设计资产，
不得脱离现有 Design System 自行创造规则。

---

## 1. 主设计规范

首先读取：

`bsp-design.md`

该文件是本项目完整的 Design System 规范，包含：

- Color
- Typography
- Spacing
- Radius
- Layout
- Icon
- Components
- Variants
- 页面模板
- 页面规则
- 状态及交互规范

设计时优先复用已有规则、组件和页面模式。

---

## 2. WiFi / 配网设计

当任务涉及：

- 添加设备
- WiFi 配网
- 配网指引
- 蓝牙 / WiFi 引导
- 设备连接
- 配网异常

必须同时读取：

`wifi-guide`

其中的配网页面结构、制作步骤和专项规则，
作为配网任务的执行依据。

如果配网专项规范与通用设计规范存在差异：

- 配网专项页面规则优先使用 wifi-guide
- 通用颜色、字体、组件和 Design Token 仍以 bsp-design.md 为基础
- 无法判断时不得自行选择，应提出冲突点

---

## 3. 设计稿参考

进行页面设计前，应同时查找现有设计稿参考。

优先参考：

- 已有同类页面
- 页面模板
- 已完成页面截图
- Figma 对应 Frame / Node
- `图片和附件/` 中的视觉参考

使用参考设计时：

1. 优先复用已有页面结构
2. 优先保持已有信息层级
3. 不得只参考视觉效果而忽略组件结构
4. 设计结果仍必须符合当前 Design System
5. 参考稿与最新规范冲突时，以最新规范为准

---

## 4. Icon 获取

需要 Icon 时，按以下顺序处理：

### 第一步
查询 `bsp-design.md` 中的 Icon 规范。

确认：

- 图标类型
- 图标尺寸
- 线宽
- 风格
- 状态
- 使用场景

### 第二步
查询现有 Icon 资产库 / 设计图标 Skill。

优先使用已有图标，不得重新绘制视觉近似的重复图标。

### 第三步
只有现有 Icon 库确实不存在所需图标时，
才提出：

`Icon 新增建议`

必须说明：

- 图标名称
- 使用场景
- 建议尺寸
- 风格
- 状态
- 为什么已有 Icon 无法满足

未经确认，不得直接将新 Icon 作为正式设计资产。

---

## 5. 设计执行原则

设计任何页面前必须遵循：

1. 先查询现有规范
2. 再查询已有组件
3. 再查询已有页面
4. 再查询专项规范
5. 最后才考虑新增设计

优先复用：

- Variables
- Components
- Variants
- Auto Layout
- Page Templates
- Icons
- Existing Assets

不得无依据自行新增：

- Color
- Typography
- Spacing
- Radius
- Component
- Icon
- 页面模式

---

## 6. 完成前检查

设计完成后必须确认：

- 是否符合 bsp-design.md
- 是否复用了现有组件
- 是否使用正确 Variables
- 是否使用正确 Icon
- 是否参考了已有同类设计
- 是否覆盖页面必要状态
- 是否使用合理 Auto Layout
- 是否存在无语义命名
- 是否明确交互关系
- 是否具备前端开发条件

如果前端智能体仍需要大量猜测设计意图，
则设计不得视为完成。
