# 📱 Daily Digest Capsule - 产品需求文档 (PRD)

**版本**: v1.0  
**日期**: 2025-11-02  
**状态**: Draft  
**平台**: iOS  

---

## 📋 目录

1. [产品概述](#1-产品概述)
2. [市场分析](#2-市场分析)
3. [用户画像](#3-用户画像)
4. [核心功能](#4-核心功能)
5. [技术架构](#5-技术架构)
6. [信息架构](#6-信息架构)
7. [UI/UX设计规范](#7-uiux设计规范)
8. [数据管理](#8-数据管理)
9. [变现策略](#9-变现策略)
10. [开发路线图](#10-开发路线图)
11. [成功指标](#11-成功指标)
12. [风险与挑战](#12-风险与挑战)

---

## 1. 产品概述

### 1.1 产品定位

**Daily Digest Capsule** 是一款专注于对抗信息过载的iOS应用，通过每日定时推送精选信息"胶囊"，帮助用户高效获取当日关键资讯、知识和娱乐内容。

### 1.2 核心价值主张 (USP)

> **"你的每日信息营养剂"**

- 🎯 **聚焦而非过载**：摘要式内容，避免信息焦虑
- ⏰ **定时而非随机**：培养固定阅读习惯，建立仪式感
- 🎁 **精选而非信息流**：多维度整合，一次满足多种信息需求
- 🚀 **高效而非碎片**：3-5分钟完成每日信息摄入

### 1.3 目标用户

**主要用户群体**：
- 📊 年龄：25-45岁
- 💼 职业：白领、创业者、学生、知识工作者
- 🎯 需求：追求高效信息管理，对抗信息过载
- 💡 特征：有固定的晨间或通勤阅读习惯

### 1.4 产品愿景

成为用户每日必开的"信息胶囊"，建立稳固的日活习惯，通过简洁高效的信息聚合服务，提升用户的信息获取质量和生活幸福感。

---

## 2. 市场分析

### 2.1 市场机会

| 维度 | 现状 | 机会 |
|------|------|------|
| **信息过载问题** | 日益严重，用户焦虑感增加 | 提供"少而精"的解决方案 |
| **新闻聚合市场** | 竞品多但同质化严重 | 差异化定位：定时胶囊 + 多元内容 |
| **习惯培养需求** | 用户渴望建立良好阅读习惯 | 通过通知和仪式感培养习惯 |
| **付费意愿** | 用户愿意为优质内容付费 | 轻量付费模式（$0.99去广告） |

### 2.2 竞品分析

| 竞品 | 优势 | 劣势 | 差异化策略 |
|------|------|------|-----------|
| **Apple News** | 官方支持、内容丰富 | 信息过载、无定时推送 | ✅ 定时胶囊概念 |
| **Flipboard** | 精美排版、个性化 | 需要频繁互动 | ✅ 被动接收，无需选择 |
| **SmartNews** | 智能推荐 | 广告多、干扰大 | ✅ 简洁无干扰（付费版） |
| **Pocket** | 稍后读功能强 | 需主动收集 | ✅ 自动聚合推送 |

**我们的独特优势**：
1. "胶囊"概念 - 一日一囊，克制设计
2. 多维内容整合 - 新闻+天气+知识+娱乐
3. 定时推送仪式感 - 培养固定习惯
4. 低价去广告 - 降低付费门槛

---

## 3. 用户画像

### 3.1 核心用户：高效的莉莉 (Efficient Lily)

**基本信息**：
- 👤 年龄：28岁
- 💼 职业：产品经理
- 📍 地点：旧金山
- 💰 收入：$85,000/年

**痛点**：
- 信息过载严重，每天被各种推送淹没
- 想了解世界动态但没时间深度阅读
- 需要在通勤路上高效获取信息

**使用场景**：
1. 早上8:00收到通知，地铁上打开App
2. 3分钟浏览当日胶囊（新闻+天气+金句）
3. 偶尔点开感兴趣的新闻详情
4. 分享有趣的金句到社交媒体

**期待价值**：
- ✅ 定时推送，不需要主动想起
- ✅ 内容精选，节省筛选时间
- ✅ 简洁界面，快速获取信息

---

### 3.2 次要用户：好奇的大卫 (Curious David)

**基本信息**：
- 👤 年龄：35岁
- 💼 职业：软件工程师
- 📍 地点：北京
- 💰 收入：￥400,000/年

**痛点**：
- 想学习有趣知识但缺少渠道
- 喜欢冷知识和笑话但不知去哪找
- 希望每天有点"小惊喜"

**使用场景**：
1. 晚上9:00收到通知（自定义时间）
2. 睡前刷App，查看历史事件和笑话
3. 开启星座运势模块（娱乐）
4. 将有趣内容分享给朋友

**期待价值**：
- ✅ 趣味内容（笑话、冷知识、幸运签）
- ✅ 可自定义模块和时间
- ✅ 双语支持（中英文）

---

## 4. 核心功能

### 4.1 功能架构图

```
Daily Digest Capsule
│
├── 📦 每日胶囊（主功能）
│   ├── 核心模块（默认开启，不可关闭）
│   │   ├── 💭 每日金句
│   │   ├── 📅 历史上的今天
│   │   └── 📰 新闻头条
│   │
│   └── 可选模块（设置中启用，默认全部开启）
│       ├── ⭐ 星座运势
│       ├── 🤓 趣味知识
│       ├── 😄 每日笑话
│       ├── 🥠 幸运签语
│       └── 💡 生活技巧
│
│   注：V1.0不包含天气功能（需API key），V1.5可能添加
│
├── ⚙️ 设置与个性化
│   ├── 通知设置（时间、频率）
│   ├── 内容偏好（模块开关）
│   ├── 语言选择（中文/英文）
│   ├── 个人信息（位置、星座）
│   └── 深色模式
│
├── 💰 变现功能
│   ├── 开屏广告
│   ├── Banner广告
│   └── 应用内购买（去广告）
│
└── 📚 辅助功能
    ├── 缓存显示（显示上次数据，新数据覆盖）
    └── 系统分享（使用iOS原生分享菜单）
```

---

### 4.2 功能详细说明

#### 4.2.1 每日胶囊（核心功能）

**功能描述**：
每天在用户设定的时间自动生成并推送一个"信息胶囊"，包含当日精选的多维度内容。

**✅ 重大更新 (2025-11-03)**: 所有8个API现已统一使用ViewBits平台！  
**统一基础URL**: `https://api.viewbits.com/v1/`

**核心模块**（默认启用，不可关闭，全部免费无需API key）：

| 模块 | API来源 | 内容 | 展示形式 | API端点 |
|------|---------|------|----------|---------|
| **每日金句** | ViewBits ZenQuotes | 1条励志/哲理名言 | 卡片：引用文字+作者 | `v1/zenquotes?mode=today` |
| **历史上的今天** | ViewBits OnThisDay | 3-5条历史事件（60个中选5个） | 列表：年份+事件描述 | `v1/onthisday?m=&d=` |
| **新闻头条** | ViewBits Headlines | 5-7条新闻摘要（24条中选7条） | 卡片：标题+来源+时间 | `v1/headlines` |

**注**：~~天气信息~~已从V1.0移除（需API key），可能在V1.5添加。

**可选模块**（用户可在设置中启用/关闭，默认全部开启）：

| 模块 | API来源 | 内容 | 展示形式 | API端点 |
|------|---------|------|----------|---------|
| **星座运势** | ViewBits Horoscope | 当日星座运势 | 卡片：运势文字+日期 | `v1/horoscope?sign=` |
| **趣味知识** | ViewBits UselessFacts | 1条有趣冷知识 | 卡片：知识描述+来源 | `v1/uselessfacts?mode=today` |
| **每日笑话** | ViewBits Jester | 1个笑话 | 卡片：笑话文字 | `v1/jester?mode=today` |
| **幸运签语** | ViewBits Fortune | 1条幸运语+幸运数字 | 卡片：签语文字+数字 | `v1/fortunecookie?mode=today` |
| **生活技巧** | ViewBits LifeHacks | 1条生活小贴士 | 卡片：技巧描述 | `v1/lifehacks?mode=today` |

**✅ 100% ViewBits统一平台优势**：单一提供商、统一管理、更稳定可靠

**注意**：可选模块默认全部开启，用户可在设置中主动关闭不需要的模块。

**交互流程**：
```
定时到达（如 8:00 AM）
   ↓
发送推送通知："今日信息胶囊已准备好 🎁"
   ↓
用户点击通知打开App
   ↓
检查本地缓存
   ├─ 有当日数据 → 直接展示
   └─ 无当日数据 → 调用API获取
   ↓
显示"胶囊打开"动画
   ↓
卡片依次展示（支持上下滚动）
   ↓
用户可点击卡片查看详情/分享
```

**业务规则**：
1. ✅ 每日只生成1次胶囊（基于自然日判断，0点失效）
2. ✅ 自动刷新：App启动时检查本地数据日期，非当日则自动刷新
3. ✅ 手动刷新：下拉刷新，但有当日缓存时不发送API请求
4. ✅ 缓存策略：保留上一次数据，获取新数据后覆盖（无需历史记录功能）
5. ✅ 离线支持：显示上次缓存的数据
6. ✅ 完全免费：所有API无需keys，零门槛启动
7. ✅ 权限要求最少：
   - 仅需通知权限（可选，用于定时提醒）
   - 无需定位权限（V1.0不提供天气功能）

---

#### 4.2.2 智能刷新逻辑（关键特性）

**设计目标**：
- 减少API调用次数（遵守速率限制）
- 提升用户体验（避免重复加载）
- 节省流量和电量

**刷新策略**：

**场景1：App启动时（自动刷新）**
```swift
func onAppLaunch() {
    let cachedCapsule = loadFromCache()
    
    if cachedCapsule == nil || !isToday(cachedCapsule.date) {
        // 缓存为空或非当日数据 → 自动刷新
        await fetchNewCapsule()
    } else {
        // 有当日缓存 → 直接展示
        displayCapsule(cachedCapsule)
    }
}
```

**场景2：用户手动下拉刷新**
```swift
func onManualRefresh() {
    let cachedCapsule = loadFromCache()
    
    if cachedCapsule != nil && isToday(cachedCapsule.date) {
        // 有当日缓存 → 不发送API请求，直接展示
        displayCapsule(cachedCapsule)
        showToast("已是最新数据")
    } else {
        // 无缓存或缓存过期 → 发送API请求
        await fetchNewCapsule()
    }
}
```

**场景3：后台刷新（可选）**
```swift
// 使用 Background Tasks Framework
// 在夜间（如 2:00 AM）预加载次日数据
func scheduleBackgroundRefresh() {
    BGTaskScheduler.shared.schedule(identifier: "com.dailydigest.refresh") {
        await prefetchTomorrowCapsule()
    }
}
```

**缓存策略**：
- 存储位置：UserDefaults（小数据）
- 缓存时长：按自然日，每天0点失效
- 数据覆盖：获取新数据后直接覆盖旧数据（仅保留最新一次）
- 离线显示：无网络时显示上次缓存的数据 + "离线模式"提示
- 数据判断：
  ```swift
  func isToday(date: Date) -> Bool {
      Calendar.current.isDateInToday(date)
  }
  ```

---

#### 4.2.3 推送通知系统

**通知类型**：

| 类型 | 触发时机 | 内容 | 频率 |
|------|----------|------|------|
| **每日提醒** | 用户设定时间（默认8:00） | "今日信息胶囊已准备好 🎁" | 每天1次 |
| **权限引导** | 首次打开App | "开启通知，每日准时送达" | 仅1次 |

**通知设置**：
- ✅ 自定义通知时间（时间选择器）
- ✅ 周末开关（是否在周末推送）
- ✅ 静音时段（免打扰模式）
- ✅ 通知预览（显示金句或新闻标题）

**实现方案**：
```swift
import UserNotifications

func scheduleNotification(at time: Date) {
    let content = UNMutableNotificationContent()
    content.title = "Daily Digest Capsule"
    content.body = "今日信息胶囊已准备好 🎁"
    content.sound = .default
    
    var dateComponents = Calendar.current.dateComponents([.hour, .minute], from: time)
    let trigger = UNCalendarNotificationTrigger(dateMatching: dateComponents, repeats: true)
    
    let request = UNNotificationRequest(identifier: "dailyCapsule", content: content, trigger: trigger)
    UNUserNotificationCenter.current().add(request)
}
```

---

#### 4.2.4 设置与个性化

**设置页面结构**：

```
⚙️ 设置
│
├── 🔔 通知设置
│   ├── 每日提醒时间 [时间选择器]
│   ├── 周末推送 [开关]
│   └── 通知预览 [开关]
│
├── 📦 内容偏好
│   ├── 核心模块 [固定显示，不可关闭]
│   │   ├── ✅ 每日金句（英文）
│   │   ├── ✅ 历史上的今天（支持中英文）
│   │   └── ✅ 新闻头条（全球新闻）
│   │
│   └── 可选模块 [开关列表，默认全部开启]
│       ├── ⭐ 星座运势 [ON] ← 默认开启（英文）
│       ├── 🤓 趣味知识 [ON] ← 默认开启（英文）
│       ├── 😄 每日笑话 [ON] ← 默认开启（英文）
│       ├── 🥠 幸运签语 [ON] ← 默认开启（英文）
│       └── 💡 生活技巧 [ON] ← 默认开启（英文）
│
├── 🌐 语言与地区
│   └── 语言选择 [英文 / 中文]
│
├── 👤 个人信息（用于星座运势模块）
│   ├── 生日 [日期选择器]
│   └── 星座 [自动推算或手动选择]
│
├── 🎨 外观
│   ├── 深色模式 [跟随系统 / 浅色 / 深色]
│   └── 字体大小 [小 / 中 / 大]
│
├── 💰 支持我们
│   ├── 移除广告 [$0.99]
│   └── 恢复购买
│
└── ℹ️ 关于
    ├── 版本号
    ├── 服务条款
    ├── 隐私政策
    └── 反馈与建议
```

---

#### 4.2.5 语言支持（双语功能）

**支持语言**：
- 🇺🇸 英文（默认）
- 🇨🇳 简体中文

**语言切换流程**：
```
用户进入设置 → 语言选择
   ↓
选择中文
   ↓
界面文本立即切换（使用本地化字符串）
   ↓
显示提示："已切换至中文，下拉刷新获取中文内容"
   ↓
用户返回主页，手动下拉刷新
   ↓
发送API请求时携带 language=zh 参数
   ↓
显示中文内容（新闻、天气等）
```

**语言参数映射**：

| 模块 | 英文参数 | 中文参数 | 中文用户显示 | V1.0状态 |
|------|----------|----------|-------------|---------|
| **每日金句** | 仅英文 | - | ✅ 保持英文 | ✅ 包含 |
| **历史上的今天** | `/wikipedia/en/` | `/wikipedia/zh/` | ✅ 显示中文 | ✅ 包含 |
| **新闻头条** | ViewBits默认 | ViewBits默认 | ✅ 全球新闻 | ✅ 包含 |
| ~~**天气**~~ | `lang=en` | `lang=zh_cn` | - | ❌ V1.0不包含 |
| **星座运势** | 仅英文 | - | ✅ 保持英文 | ✅ 包含（可选）|
| **趣味知识/笑话/签语** | 仅英文 | - | ✅ 保持英文 | ✅ 包含（可选）|

**V1.0 语言支持策略**：
- ✅ **核心模块**：历史支持中英文切换，新闻为全球默认
- ✅ **金句模块**：保持英文（英文金句更有品质感）
- ✅ **可选模块**：保持英文（用户可自行关闭）
- ✅ **界面文本**：完整支持中英文本地化
- 🔮 **未来升级**：V1.5可添加天气（支持中英文）

**本地化文件**：
```swift
// Localizable.strings (English)
"daily_capsule" = "Daily Capsule";
"quote_of_day" = "Quote of the Day";
"on_this_day" = "On This Day";
"news_headlines" = "News Headlines";

// Localizable.strings (Chinese)
"daily_capsule" = "每日胶囊";
"quote_of_day" = "每日金句";
"on_this_day" = "历史上的今天";
"news_headlines" = "新闻头条";
```

---

## 5. 技术架构

### 5.1 技术栈

**前端框架**：
- **SwiftUI** - 现代化、声明式UI框架
- **Combine** - 响应式编程
- **Async/Await** - 异步网络请求

**数据存储**：
- **UserDefaults** - 用户设置、简单数据
- **CoreData** - 历史胶囊数据、收藏
- **Keychain** - API密钥安全存储

**网络层**：
- **URLSession** - 原生网络请求
- **Alamofire**（可选）- 更便捷的网络库

**第三方SDK**：
- **Google AdMob** - 广告平台
- **StoreKit** - 应用内购买

**其他**：
- **UserNotifications** - 本地推送
- **CoreLocation** - 定位服务
- **BackgroundTasks** - 后台刷新

---

### 5.2 架构设计（MVVM）

```
┌─────────────────────────────────────┐
│           View (SwiftUI)            │
│  ┌──────────┐  ┌──────────┐        │
│  │ MainView │  │ Settings │        │
│  └──────────┘  └──────────┘        │
└─────────────────────────────────────┘
              ↕️
┌─────────────────────────────────────┐
│         ViewModel                   │
│  ┌─────────────────────────────┐   │
│  │ CapsuleViewModel            │   │
│  │ - loadCapsule()             │   │
│  │ - refreshCapsule()          │   │
│  │ - toggleModule()            │   │
│  └─────────────────────────────┘   │
└─────────────────────────────────────┘
              ↕️
┌─────────────────────────────────────┐
│           Model + Services          │
│  ┌──────────────┐ ┌──────────────┐ │
│  │ Data Models  │ │ API Manager  │ │
│  │ - Capsule    │ │ - fetchQuote │ │
│  │ - Quote      │ │ - fetchNews  │ │
│  │ - News       │ │ - fetchWeather│ │
│  └──────────────┘ └──────────────┘ │
│  ┌──────────────┐ ┌──────────────┐ │
│  │ Cache Manager│ │ IAP Manager  │ │
│  └──────────────┘ └──────────────┘ │
└─────────────────────────────────────┘
```

---

### 5.3 项目文件结构

```
DailyDigestCapsule/
│
├── App/
│   ├── DailyDigestCapsuleApp.swift
│   └── AppDelegate.swift
│
├── Models/
│   ├── Capsule.swift
│   ├── Quote.swift
│   ├── NewsArticle.swift
│   ├── WeatherInfo.swift
│   ├── Horoscope.swift
│   └── UserSettings.swift
│
├── ViewModels/
│   ├── CapsuleViewModel.swift
│   ├── SettingsViewModel.swift
│   └── AdViewModel.swift
│
├── Views/
│   ├── Main/
│   │   ├── MainView.swift
│   │   ├── CapsuleCardView.swift
│   │   └── OpeningAnimationView.swift
│   │
│   ├── Settings/
│   │   ├── SettingsView.swift
│   │   ├── NotificationSettingsView.swift
│   │   └── ModuleTogglesView.swift
│   │
│   └── Components/
│       ├── QuoteCard.swift
│       ├── NewsCard.swift
│       ├── WeatherCard.swift
│       └── LoadingView.swift
│
├── Services/
│   ├── APIManager.swift
│   ├── ZenQuotesService.swift
│   ├── NewsService.swift
│   ├── WeatherService.swift
│   ├── CacheManager.swift
│   ├── NotificationManager.swift
│   ├── IAPManager.swift
│   └── AdManager.swift
│
├── Utilities/
│   ├── Constants.swift
│   ├── Extensions.swift
│   └── Helpers.swift
│
├── Resources/
│   ├── Assets.xcassets
│   ├── Localizable.strings (en)
│   ├── Localizable.strings (zh-Hans)
│   └── Info.plist
│
└── Tests/
    ├── UnitTests/
    └── UITests/
```

---

### 5.4 API集成方案

#### 5.4.1 API Manager 基础类

```swift
import Foundation

class APIManager {
    static let shared = APIManager()
    
    private let session: URLSession
    private let decoder: JSONDecoder
    
    init() {
        let config = URLSessionConfiguration.default
        config.timeoutIntervalForRequest = 15
        self.session = URLSession(configuration: config)
        self.decoder = JSONDecoder()
    }
    
    func fetch<T: Decodable>(url: URL) async throws -> T {
        let (data, response) = try await session.data(from: url)
        
        guard let httpResponse = response as? HTTPURLResponse,
              httpResponse.statusCode == 200 else {
            throw APIError.invalidResponse
        }
        
        return try decoder.decode(T.self, from: data)
    }
}

enum APIError: Error {
    case invalidURL
    case invalidResponse
    case networkError(Error)
    case decodingError(Error)
}
```

#### 5.4.2 具体API服务示例

**✅ 更新后使用ViewBits统一平台**

**ZenQuotes Service**:
```swift
class ZenQuotesService {
    private let baseURL = "https://api.viewbits.com/v1"
    
    func fetchTodayQuote() async throws -> Quote {
        guard let url = URL(string: "\(baseURL)/zenquotes?mode=today") else {
            throw APIError.invalidURL
        }
        
        let quotes: [QuoteResponse] = try await APIManager.shared.fetch(url: url)
        guard let first = quotes.first else {
            throw APIError.invalidResponse
        }
        
        return Quote(text: first.q, author: first.a)
    }
}

struct QuoteResponse: Codable {
    let q: String  // quote
    let a: String  // author
}

struct Quote {
    let text: String
    let author: String
}
```

**News Service**:
```swift
class NewsService {
    private let baseURL = "https://newsapi.org/v2"
    private let apiKey = APIKeyManager.shared.getKey(for: .newsAPI)
    
    func fetchHeadlines(language: String, category: String = "general") async throws -> [NewsArticle] {
        let urlString = "\(baseURL)/top-headlines?language=\(language)&category=\(category)&apiKey=\(apiKey)"
        
        guard let url = URL(string: urlString) else {
            throw APIError.invalidURL
        }
        
        let response: NewsResponse = try await APIManager.shared.fetch(url: url)
        return response.articles.map { NewsArticle(from: $0) }
    }
}

struct NewsResponse: Codable {
    let status: String
    let articles: [ArticleResponse]
}

struct ArticleResponse: Codable {
    let title: String
    let description: String?
    let url: String
    let urlToImage: String?
    let publishedAt: String
    let source: Source
    
    struct Source: Codable {
        let name: String
    }
}

struct NewsArticle: Identifiable {
    let id = UUID()
    let title: String
    let description: String
    let url: URL
    let imageURL: URL?
    let publishedAt: Date
    let source: String
}
```

---

### 5.5 数据模型

**主数据模型：DailyCapsule**
```swift
import Foundation

struct DailyCapsule: Codable {
    let id: UUID
    let date: Date
    let quote: Quote?
    let historyEvents: [HistoricalEvent]
    let news: [NewsArticle]
    let weather: WeatherInfo?
    let horoscope: Horoscope?
    let joke: String?
    let fortune: String?
    let lifehack: String?
    let fact: String?
    
    var isToday: Bool {
        Calendar.current.isDateInToday(date)
    }
}

struct HistoricalEvent: Codable, Identifiable {
    let id = UUID()
    let year: Int
    let description: String
    let wikipediaURL: URL?
}

struct WeatherInfo: Codable {
    let temperature: Double
    let condition: String
    let feelsLike: Double
    let humidity: Int
    let cityName: String
    let forecast: [DailyForecast]
    
    struct DailyForecast: Codable {
        let date: Date
        let tempMax: Double
        let tempMin: Double
        let condition: String
    }
}

struct Horoscope: Codable {
    let sign: ZodiacSign
    let date: Date
    let prediction: String
    let luckyColor: String?
    let luckyNumber: Int?
    let mood: String?
}

enum ZodiacSign: String, Codable, CaseIterable {
    case aries, taurus, gemini, cancer, leo, virgo
    case libra, scorpio, sagittarius, capricorn, aquarius, pisces
    
    var displayName: String {
        rawValue.capitalized
    }
}
```

---

## 6. 信息架构

### 6.1 主要页面流程

```
启动页
   ↓
[首次使用] → 欢迎引导（3屏） → 权限请求 → 初始设置
   ↓
[再次使用] → 开屏广告（可跳过） → 主页
   ↓
主页（胶囊展示）
   ├→ 下拉刷新
   ├→ 点击卡片查看详情
   ├→ 点击设置按钮 → 设置页
   └→ 底部Banner广告
```

### 6.2 主页布局（线框图）

```
┌───────────────────────────────────┐
│  ☀️ 11月2日 星期六    ⚙️         │ <- Header
├───────────────────────────────────┤
│                                   │
│  ┌─────────────────────────────┐  │
│  │ 🎁 今日胶囊已开启           │  │ <- 状态指示器
│  │ 下次更新：明天 8:00         │  │
│  └─────────────────────────────┘  │
│                                   │
│  ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━┓  │
│  ┃ 💭 Quote of the Day       ┃  │ <- 卡片 1
│  ┃                           ┃  │
│  ┃ "The only way to do       ┃  │
│  ┃  great work is to love    ┃  │
│  ┃  what you do."            ┃  │
│  ┃                           ┃  │
│  ┃ — Steve Jobs              ┃  │
│  ┃                           ┃  │
│  ┃           [分享 ↗]        ┃  │
│  ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━┛  │
│                                   │
│  ┌─────────────────────────────┐  │
│  │ ☀️ San Francisco · 22°C    │  │ <- 卡片 2
│  │                             │  │
│  │ 🌡️ 22°  ☁️ Clear Sky       │  │
│  │ 体感 21°C · 湿度 60%        │  │
│  │                             │  │
│  │ 未来3天：                   │  │
│  │ 周日 25° ☀️ 周一 23° ⛅     │  │
│  │ 周二 20° 🌧️                 │  │
│  └─────────────────────────────┘  │
│                                   │
│  ┌─────────────────────────────┐  │
│  │ 📅 On This Day             │  │ <- 卡片 3
│  │                             │  │
│  │ 🔹 1755                     │  │
│  │ The Lisbon earthquake...    │  │
│  │                             │  │
│  │ 🔹 1947                     │  │
│  │ Howard Hughes flew the...   │  │
│  │                             │  │
│  │ [查看全部 5 条]             │  │
│  └─────────────────────────────┘  │
│                                   │
│  ┌─────────────────────────────┐  │
│  │ 📰 News Headlines          │  │ <- 卡片 4
│  │                             │  │
│  │ 🔸 BBC News · 2小时前       │  │
│  │ Breaking: Major tech...     │  │
│  │ [缩略图]                    │  │
│  │                             │  │
│  │ 🔸 CNN · 5小时前            │  │
│  │ Election results show...    │  │
│  │                             │  │
│  │ [查看全部 7 条]             │  │
│  └─────────────────────────────┘  │
│                                   │
│  ... 更多可选模块卡片 ...         │
│                                   │
├───────────────────────────────────┤
│  [   Google AdMob Banner 广告  ]  │ <- Footer Ad
└───────────────────────────────────┘
```

---

## 7. UI/UX设计规范

### 7.1 设计原则

1. **简洁克制**：每屏信息量控制在用户3-5分钟可消化的范围
2. **视觉层次**：重要信息（金句、天气）优先展示
3. **一致性**：所有卡片遵循统一设计语言
4. **仪式感**：通过动画和视觉隐喻强化"打开胶囊"的体验
5. **无障碍**：支持动态字体、VoiceOver

### 7.2 配色方案

**浅色模式**：
```
主色调：#007AFF (系统蓝)
背景色：#F2F2F7 (浅灰)
卡片背景：#FFFFFF (白色)
文字主色：#000000 (黑色)
文字副色：#8E8E93 (灰色)
强调色：#FF9500 (橙色)
```

**深色模式**：
```
主色调：#0A84FF (亮蓝)
背景色：#000000 (黑色)
卡片背景：#1C1C1E (深灰)
文字主色：#FFFFFF (白色)
文字副色：#8E8E93 (灰色)
强调色：#FF9F0A (亮橙)
```

### 7.3 字体规范

```
标题（H1）：SF Pro Display - Bold - 28pt
副标题（H2）：SF Pro Display - Semibold - 22pt
卡片标题（H3）：SF Pro Display - Semibold - 18pt
正文：SF Pro Text - Regular - 16pt
辅助文字：SF Pro Text - Regular - 14pt
时间戳：SF Pro Text - Regular - 12pt
```

### 7.4 卡片设计规范

**卡片基础样式**：
- 圆角：16pt
- 阴影：`shadow(color: .black.opacity(0.05), radius: 8, x: 0, y: 2)`
- 内边距：16pt
- 卡片间距：12pt
- 最小高度：120pt

**卡片状态**：
- 默认：白色背景（深色模式为深灰）
- 点击：轻微缩放动画（scale: 0.98）
- 加载中：骨架屏占位

**SwiftUI示例**：
```swift
struct CapsuleCardStyle: ViewModifier {
    func body(content: Content) -> some View {
        content
            .padding(16)
            .background(Color(.systemBackground))
            .cornerRadius(16)
            .shadow(color: .black.opacity(0.05), radius: 8, x: 0, y: 2)
    }
}
```

### 7.5 动画设计

**胶囊打开动画**（首次查看当日胶囊时）：
```swift
struct CapsuleOpeningAnimation: View {
    @State private var isOpened = false
    
    var body: some View {
        ZStack {
            // 胶囊图标
            Image(systemName: "capsule")
                .font(.system(size: 100))
                .rotationEffect(.degrees(isOpened ? 90 : 0))
                .opacity(isOpened ? 0 : 1)
            
            // 卡片展开
            CardsView()
                .opacity(isOpened ? 1 : 0)
                .scaleEffect(isOpened ? 1 : 0.8)
        }
        .onAppear {
            withAnimation(.spring(response: 0.6, dampingFraction: 0.7)) {
                isOpened = true
            }
        }
    }
}
```

**下拉刷新动画**：
- 使用系统默认的 `.refreshable` modifier
- 加载时显示旋转菊花图标
- 刷新完成时有轻微的回弹效果

**卡片进入动画**（依次滑入）：
```swift
ForEach(Array(cards.enumerated()), id: \.offset) { index, card in
    CardView(card: card)
        .transition(.move(edge: .trailing).combined(with: .opacity))
        .animation(.easeOut(duration: 0.3).delay(Double(index) * 0.1), value: cards)
}
```

---

## 8. 数据管理

### 8.1 数据流架构

```
View (用户交互)
   ↓
ViewModel (业务逻辑)
   ↓
检查缓存
   ├─ 有效缓存 → 返回数据
   └─ 无缓存/过期 ↓
API Services (网络请求)
   ↓
解析数据
   ↓
保存缓存
   ↓
返回ViewModel
   ↓
更新View
```

### 8.2 缓存管理器

```swift
class CacheManager {
    static let shared = CacheManager()
    
    private let userDefaults = UserDefaults.standard
    private let cacheKey = "dailyCapsuleCache"
    
    func saveCapsule(_ capsule: DailyCapsule) {
        let encoder = JSONEncoder()
        if let data = try? encoder.encode(capsule) {
            userDefaults.set(data, forKey: cacheKey)
        }
    }
    
    func loadCapsule() -> DailyCapsule? {
        guard let data = userDefaults.data(forKey: cacheKey) else {
            return nil
        }
        
        let decoder = JSONDecoder()
        return try? decoder.decode(DailyCapsule.self, from: data)
    }
    
    func clearCache() {
        userDefaults.removeObject(forKey: cacheKey)
    }
    
    func isCacheValid() -> Bool {
        guard let capsule = loadCapsule() else {
            return false
        }
        return Calendar.current.isDateInToday(capsule.date)
    }
}
```

### 8.3 用户设置管理

```swift
class UserSettings: ObservableObject {
    static let shared = UserSettings()
    
    @AppStorage("notificationTime") var notificationTime: Date = Date()
    @AppStorage("language") var language: String = "en"
    @AppStorage("enabledModules") var enabledModulesData: Data = Data()
    @AppStorage("zodiacSign") var zodiacSign: String = ""
    @AppStorage("isPremiumUser") var isPremiumUser: Bool = false
    
    var enabledModules: Set<CapsuleModule> {
        get {
            guard let decoded = try? JSONDecoder().decode(Set<CapsuleModule>.self, from: enabledModulesData) else {
                return [.quote, .history, .news, .weather] // 默认核心模块
            }
            return decoded
        }
        set {
            if let encoded = try? JSONEncoder().encode(newValue) {
                enabledModulesData = encoded
            }
        }
    }
}

enum CapsuleModule: String, Codable, CaseIterable {
    // 核心模块（不可关闭）
    case quote = "quote"
    case history = "history"
    case news = "news"
    case weather = "weather"
    
    // 可选模块
    case horoscope = "horoscope"
    case fact = "fact"
    case joke = "joke"
    case fortune = "fortune"
    case lifehack = "lifehack"
    
    var isCore: Bool {
        [.quote, .history, .news, .weather].contains(self)
    }
}
```

---

## 9. 变现策略

### 9.1 广告系统

#### 9.1.1 开屏广告（App Open Ad）

**展示时机**：
- 用户打开App时（冷启动）
- 从后台切换回前台时（可选，避免过度打扰）

**技术实现**：
```swift
import GoogleMobileAds

class AppOpenAdManager: NSObject, ObservableObject, GADFullScreenContentDelegate {
    @Published var isAdReady = false
    private var appOpenAd: GADAppOpenAd?
    private var loadTime: Date?
    
    // 测试ID: ca-app-pub-3940256099942544/5662855259
    // 生产ID: ca-app-pub-XXXXX/YYYYY
    private let adUnitID = "ca-app-pub-XXXXX/YYYYY"
    
    func loadAd() {
        // 付费用户不加载广告
        if UserSettings.shared.isPremiumUser {
            return
        }
        
        GADAppOpenAd.load(
            withAdUnitID: adUnitID,
            request: GADRequest()
        ) { [weak self] ad, error in
            if let error = error {
                print("开屏广告加载失败: \(error)")
                self?.isAdReady = false
                return
            }
            
            self?.appOpenAd = ad
            self?.appOpenAd?.fullScreenContentDelegate = self
            self?.loadTime = Date()
            self?.isAdReady = true
        }
    }
    
    func showAdIfAvailable(from viewController: UIViewController) {
        // 付费用户直接跳过
        if UserSettings.shared.isPremiumUser {
            return
        }
        
        // 检查广告是否过期（4小时）
        if let loadTime = loadTime,
           Date().timeIntervalSince(loadTime) > 4 * 3600 {
            loadAd()
            return
        }
        
        guard let ad = appOpenAd, isAdReady else {
            return
        }
        
        ad.present(fromRootViewController: viewController)
    }
    
    // MARK: - GADFullScreenContentDelegate
    
    func adDidDismissFullScreenContent(_ ad: GADFullScreenPresentingAd) {
        appOpenAd = nil
        isAdReady = false
        // 预加载下一次广告
        loadAd()
    }
    
    func ad(_ ad: GADFullScreenPresentingAd, didFailToPresentFullScreenContentWithError error: Error) {
        print("开屏广告展示失败: \(error)")
        appOpenAd = nil
        isAdReady = false
    }
}
```

#### 9.1.2 Banner 广告

**展示位置**：主页底部（固定）

**技术实现**：
```swift
struct BannerAdView: UIViewRepresentable {
    @EnvironmentObject var settings: UserSettings
    
    func makeUIView(context: Context) -> GADBannerView {
        let banner = GADBannerView(adSize: GADAdSizeBanner)
        banner.adUnitID = "ca-app-pub-XXXXX/ZZZZZ"
        banner.rootViewController = UIApplication.shared.windows.first?.rootViewController
        banner.delegate = context.coordinator
        
        // 付费用户不加载广告
        if !settings.isPremiumUser {
            banner.load(GADRequest())
        }
        
        return banner
    }
    
    func updateUIView(_ uiView: GADBannerView, context: Context) {
        // 付费后隐藏广告
        uiView.isHidden = settings.isPremiumUser
    }
    
    func makeCoordinator() -> Coordinator {
        Coordinator(self)
    }
    
    class Coordinator: NSObject, GADBannerViewDelegate {
        var parent: BannerAdView
        
        init(_ parent: BannerAdView) {
            self.parent = parent
        }
        
        func bannerViewDidReceiveAd(_ bannerView: GADBannerView) {
            print("Banner广告加载成功")
            bannerView.isHidden = false
        }
        
        func bannerView(_ bannerView: GADBannerView, didFailToReceiveAdWithError error: Error) {
            print("Banner广告加载失败: \(error)")
            // 加载失败时隐藏
            bannerView.isHidden = true
        }
    }
}
```

**预加载策略**：
- App启动时预加载开屏广告
- 进入主页时预加载Banner广告
- 失败时静默处理，不影响用户体验

---

### 9.2 应用内购买（IAP）

#### 9.2.1 产品配置

**产品ID**: `com.dailydigest.removeads`  
**类型**: 非消耗型（Non-Consumable）  
**价格**: $0.99 USD  
**本地化名称**:
- 英文: "Remove Ads & Support Developer"
- 中文: "移除广告并支持开发者"

**描述**:
- 英文: "Remove all ads and enjoy an ad-free experience while supporting the developer."
- 中文: "移除所有广告，享受纯净体验，同时支持开发者持续改进。"

#### 9.2.2 购买流程

```
用户进入设置页
   ↓
点击"移除广告 $0.99"
   ↓
显示确认弹窗："确定购买？"
   ↓
调用 StoreKit 购买
   ↓
Apple支付流程（Touch ID / Face ID）
   ↓
购买成功
   ↓
更新本地状态 (isPremiumUser = true)
   ↓
隐藏所有广告
   ↓
显示成功提示："感谢支持！广告已移除"
```

#### 9.2.3 技术实现

```swift
import StoreKit

class IAPManager: NSObject, ObservableObject, SKProductsRequestDelegate, SKPaymentTransactionObserver {
    static let shared = IAPManager()
    
    @Published var products: [SKProduct] = []
    @Published var isPurchasing = false
    
    private let productID = "com.dailydigest.removeads"
    
    override init() {
        super.init()
        SKPaymentQueue.default().add(self)
        fetchProducts()
    }
    
    // 获取产品信息
    func fetchProducts() {
        let request = SKProductsRequest(productIdentifiers: [productID])
        request.delegate = self
        request.start()
    }
    
    // SKProductsRequestDelegate
    func productsRequest(_ request: SKProductsRequest, didReceive response: SKProductsResponse) {
        DispatchQueue.main.async {
            self.products = response.products
        }
    }
    
    // 购买
    func purchase() {
        guard let product = products.first else {
            print("产品未加载")
            return
        }
        
        isPurchasing = true
        let payment = SKPayment(product: product)
        SKPaymentQueue.default().add(payment)
    }
    
    // 恢复购买
    func restorePurchases() {
        SKPaymentQueue.default().restoreCompletedTransactions()
    }
    
    // SKPaymentTransactionObserver
    func paymentQueue(_ queue: SKPaymentQueue, updatedTransactions transactions: [SKPaymentTransaction]) {
        for transaction in transactions {
            switch transaction.transactionState {
            case .purchased:
                completePurchase(transaction)
            case .restored:
                completePurchase(transaction)
            case .failed:
                failedPurchase(transaction)
            case .deferred, .purchasing:
                break
            @unknown default:
                break
            }
        }
    }
    
    private func completePurchase(_ transaction: SKPaymentTransaction) {
        DispatchQueue.main.async {
            UserSettings.shared.isPremiumUser = true
            self.isPurchasing = false
            // 发送通知，隐藏广告
            NotificationCenter.default.post(name: .purchaseCompleted, object: nil)
        }
        SKPaymentQueue.default().finishTransaction(transaction)
    }
    
    private func failedPurchase(_ transaction: SKPaymentTransaction) {
        DispatchQueue.main.async {
            self.isPurchasing = false
            if let error = transaction.error as? SKError {
                if error.code != .paymentCancelled {
                    // 显示错误提示
                    print("购买失败: \(error.localizedDescription)")
                }
            }
        }
        SKPaymentQueue.default().finishTransaction(transaction)
    }
}

extension Notification.Name {
    static let purchaseCompleted = Notification.Name("purchaseCompleted")
}
```

#### 9.2.4 设置页购买按钮

```swift
struct PurchaseSection: View {
    @ObservedObject var iapManager = IAPManager.shared
    @EnvironmentObject var settings: UserSettings
    
    var body: some View {
        Section {
            if settings.isPremiumUser {
                HStack {
                    Image(systemName: "checkmark.circle.fill")
                        .foregroundColor(.green)
                    Text("已购买 - 感谢支持！")
                }
            } else {
                Button(action: {
                    iapManager.purchase()
                }) {
                    HStack {
                        VStack(alignment: .leading) {
                            Text("移除广告")
                                .font(.headline)
                            Text("支持开发者，享受纯净体验")
                                .font(.caption)
                                .foregroundColor(.secondary)
                        }
                        Spacer()
                        if iapManager.isPurchasing {
                            ProgressView()
                        } else {
                            Text("$0.99")
                                .font(.headline)
                                .foregroundColor(.blue)
                        }
                    }
                }
                .disabled(iapManager.isPurchasing)
                
                Button("恢复购买") {
                    iapManager.restorePurchases()
                }
                .font(.caption)
            }
        } header: {
            Text("支持我们")
        }
    }
}
```

---

### 9.3 收入预测

**假设**：
- 日活用户（DAU）：10,000
- 广告展示率：80%（付费用户20%）
- 开屏广告 eCPM：$5
- Banner广告 eCPM：$2
- 付费转化率：2%

**月收入估算**：
```
广告收入：
- 开屏广告：10,000 × 0.8 × 30 × ($5/1000) = $1,200
- Banner广告：10,000 × 0.8 × 30 × ($2/1000) = $480
小计：$1,680/月

付费收入：
- 新用户：10,000 × 30 × 2% × $0.99 = $5,940/月
  （假设每日新增10,000，转化率2%）

总计：约 $7,620/月
```

---

## 10. 开发路线图

### 10.1 开发阶段（10周计划）

#### **Week 1: 项目初始化**
- [x] 创建Xcode项目（SwiftUI + MVVM）
- [x] 配置Git仓库
- [x] 设计项目文件结构
- [x] 集成依赖管理（SPM）
- [x] 创建基础数据模型

#### **Week 2-3: 核心功能开发**
- [ ] 实现网络层（APIManager）
- [ ] 开发各API Service（ZenQuotes, News, Weather等）
- [ ] 实现缓存管理器
- [ ] 开发智能刷新逻辑
- [ ] 单元测试（网络层）

#### **Week 4-5: UI开发**
- [ ] 设计并实现主页布局
- [ ] 开发卡片组件（QuoteCard, NewsCard等）
- [ ] 实现"胶囊打开"动画
- [ ] 实现下拉刷新
- [ ] 开发设置页面

#### **Week 6: 推送通知**
- [ ] 实现本地通知系统
- [ ] 开发通知设置页面
- [ ] 实现后台刷新（可选）
- [ ] 测试通知准时性

#### **Week 7: 广告集成**
- [ ] 注册AdMob账户
- [ ] 集成AdMob SDK
- [ ] 实现开屏广告
- [ ] 实现Banner广告
- [ ] 测试广告加载失败隐藏逻辑

#### **Week 8: 应用内购买**
- [ ] 在App Store Connect创建IAP产品
- [ ] 实现IAPManager
- [ ] 实现购买流程
- [ ] 实现恢复购买
- [ ] 测试沙盒购买

#### **Week 9: 多语言与优化**
- [ ] 实现国际化（i18n）
- [ ] 翻译所有界面文字
- [ ] 适配中文API参数
- [ ] 性能优化（减少API调用）
- [ ] UI/UX打磨

#### **Week 10: 测试与发布**
- [ ] 单元测试覆盖率 > 60%
- [ ] UI测试（关键流程）
- [ ] 真机测试（多设备）
- [ ] TestFlight内测（邀请10-20人）
- [ ] 修复bug
- [ ] 准备App Store素材（截图、描述）
- [ ] 提交审核

---

### 10.2 V1.0 功能清单

#### ✅ 必须功能（MVP）
- [x] **3个核心模块**（金句、历史、新闻）- 完全免费，无需API keys
- [x] **5个可选模块**（星座、笑话等）- 默认全部开启，完全免费
- [x] 智能刷新逻辑（自动+手动，优先使用缓存）
- [x] 本地缓存（按自然日，0点失效）
- [x] 推送通知（每日定时提醒）
- [x] 开屏广告 + Banner广告（预加载，失败隐藏）
- [x] 应用内购买（$0.99去广告）
- [x] 双语支持（界面中英文，内容部分双语）
- [x] 深色模式
- [x] 系统分享功能（iOS原生）
- [x] 权限管理（仅通知权限）

#### ❌ V1.0 不包含
- ❌ 天气信息模块（需API key）→ V1.5可能添加
- ❌ 定位权限（无天气功能）
- ❌ 历史记录查看功能（仅保留最新一次缓存）
- ❌ 收藏功能
- ❌ 社交账号集成
- ❌ Widget支持

#### 🚀 未来版本（V1.5+）
- [ ] **天气模块**（OpenWeatherMap或Apple WeatherKit）
- [ ] Widget支持（iOS 14+）
- [ ] 历史记录功能（查看过去7天的胶囊）
- [ ] 收藏喜欢的内容
- [ ] 本地化新闻（NewsAPI付费版）
- [ ] AI摘要和个性化推荐
- [ ] iPad适配
- [ ] Watch App
- [ ] 语音播报（Siri集成）
- [ ] 多主题皮肤

---

## 11. 成功指标（KPI）

### 11.1 用户指标

| 指标 | 目标值（3个月） | 测量方法 |
|------|----------------|----------|
| **日活用户（DAU）** | 5,000+ | Firebase Analytics |
| **月活用户（MAU）** | 15,000+ | Firebase Analytics |
| **日活率（DAU/MAU）** | > 50% | 计算 |
| **次日留存率** | > 40% | Firebase Analytics |
| **7日留存率** | > 25% | Firebase Analytics |
| **30日留存率** | > 15% | Firebase Analytics |

### 11.2 行为指标

| 指标 | 目标值 | 测量方法 |
|------|--------|----------|
| **通知打开率** | > 50% | 推送平台统计 |
| **平均查看模块数** | > 3个 | 自定义事件 |
| **平均停留时间** | 2-3分钟 | Firebase Analytics |
| **手动刷新率** | < 10% | 自定义事件（说明缓存有效）|
| **权限授权率** | > 70% | 自定义事件 |

### 11.3 商业指标

| 指标 | 目标值 | 测量方法 |
|------|--------|----------|
| **付费转化率** | > 2% | IAP统计 |
| **广告展示率** | > 80% | AdMob后台 |
| **广告点击率（CTR）** | > 1% | AdMob后台 |
| **月收入（ARPU）** | > $0.50 | 计算（总收入/MAU）|

### 11.4 质量指标

| 指标 | 目标值 | 测量方法 |
|------|--------|----------|
| **崩溃率** | < 0.5% | Firebase Crashlytics |
| **API成功率** | > 98% | 自定义监控 |
| **App Store评分** | > 4.5星 | App Store Connect |
| **加载速度** | < 2秒 | Firebase Performance |

---

## 12. 风险与挑战

### 12.1 技术风险

| 风险 | 影响 | 缓解措施 |
|------|------|----------|
| **API速率限制** | 高 | - 本地缓存策略<br>- 购买高级API套餐<br>- 备用API方案 |
| **API服务中断** | 中 | - 多API源备份<br>- 优雅降级（显示缓存数据）<br>- 错误提示 |
| **定位权限被拒** | 中 | - 手动选择城市功能<br>- 友好的权限引导 |
| **推送通知失败** | 低 | - 提供App内定时提醒<br>- 检查并引导用户开启通知 |

### 12.2 产品风险

| 风险 | 影响 | 缓解措施 |
|------|------|----------|
| **用户留存率低** | 高 | - 强化通知系统<br>- 增加内容趣味性<br>- 优化UI/UX |
| **信息同质化** | 中 | - 差异化定位（定时胶囊）<br>- 多元内容整合<br>- 个性化推荐（V2.0）|
| **付费转化率低** | 中 | - A/B测试价格点<br>- 优化购买入口<br>- 提供试用期（V2.0）|
| **广告体验差** | 中 | - 限制广告频率<br>- 优质广告源<br>- 低价去广告选项 |

### 12.3 商业风险

| 风险 | 影响 | 缓解措施 |
|------|------|----------|
| **App Store审核被拒** | 高 | - 严格遵守审核指南<br>- 提前测试IAP和广告<br>- 准备申诉材料 |
| **竞品抄袭** | 中 | - 快速迭代<br>- 建立品牌认知<br>- 专注用户体验 |
| **API成本过高** | 低 | - 监控API使用量<br>- 优化调用策略<br>- 寻找免费/低价替代 |

---

## 13. 附录

### 13.1 API清单

| API | 用途 | 免费额度 | 付费方案 | 备注 |
|-----|------|----------|----------|------|
| **ZenQuotes** | 每日金句 | 5次/30秒 | 需联系 | 仅英文 |
| **On This Day** | 历史事件 | 无限 | N/A | 维基百科API |
| **NewsAPI** | 新闻头条 | 100次/天 | $449/月 | 开发环境够用 |
| **OpenWeatherMap** | 天气信息 | 1000次/天 | $40/月 | 60次/分钟 |
| **Horoscopes** | 星座运势 | 5次/30秒 | 需联系 | ViewBits |
| **Useless Facts** | 趣味知识 | 无限 | N/A | 开源API |
| **Jester** | 笑话 | 5次/30秒 | 需联系 | ViewBits |

### 13.2 第三方服务

| 服务 | 用途 | 费用 |
|------|------|------|
| **Google AdMob** | 广告平台 | 免费（分成）|
| **Firebase Analytics** | 数据分析 | 免费 |
| **Firebase Crashlytics** | 崩溃报告 | 免费 |
| **TestFlight** | 内测分发 | 免费 |
| **App Store** | 应用发布 | $99/年 |

### 13.3 设计资源

- **图标库**: SF Symbols (系统自带)
- **配色工具**: Coolors.co
- **原型工具**: Figma
- **设计规范**: Apple Human Interface Guidelines

### 13.4 开发工具

- **IDE**: Xcode 15+
- **语言**: Swift 5.9+
- **最低版本**: iOS 16.0
- **版本控制**: Git + GitHub
- **CI/CD**: GitHub Actions (可选)

---

## 14. 总结

**Daily Digest Capsule** 通过独特的"定时胶囊"概念，提供精选、高效、仪式感强的每日信息服务，旨在帮助用户对抗信息过载，建立良好的阅读习惯。

**核心优势**：
1. ✅ 差异化定位（定时胶囊 vs 无限信息流）
2. ✅ 多维内容整合（新闻+天气+知识+娱乐）
3. ✅ 智能刷新逻辑（减少API调用，提升体验）
4. ✅ 轻量变现模式（$0.99去广告）
5. ✅ 双语支持（覆盖更广用户）

**下一步**：
1. 完成API测试和密钥申请
2. 开始MVP开发（Week 1-3）
3. 设计高保真原型（Figma）
4. 注册AdMob和App Store账户

---

## 15. 关键决策记录

### 决策日期：2025-11-03

#### 0️⃣ 天气模块移除（重大变更）
**决策**：
- ❌ **V1.0删除天气模块**
- ❌ 原因：Weather API需要API key（即使是免费注册）
- ✅ 目标：V1.0完全零门槛，无需任何API keys

**影响**：
- ✅ 核心模块从4个减少到3个
- ✅ 无需定位权限，权限流程更简单
- ✅ 完全零成本启动
- 🔮 V1.5可能添加天气功能

#### 1️⃣ 权限策略
**决策**：
- ✅ **V1.0仅需通知权限**（可选，非强制）
- ❌ **无需定位权限**（已删除天气模块）
- ✅ **新闻模块** → 使用ViewBits默认全球新闻

**理由**：
- 简化权限请求，降低用户流失率
- 无强制权限，用户体验更友好

#### 2️⃣ API Keys 策略（最终决策）
**决策**：
- 🎉 **V1.0完全无需任何API keys**
- ✅ 所有8个API全部免费使用
- ✅ 零门槛启动，下载即可运行
- ✅ 保留API Manager架构，便于未来升级

**理由**：
- 实现完全免费运营
- 降低启动门槛
- 快速验证MVP

#### 3️⃣ 语言支持策略
**决策**：
- ✅ **界面文本**：完整支持中英文本地化
- ✅ **历史模块**：支持中英文切换（维基百科API）
- ✅ **新闻模块**：全球默认新闻（ViewBits自动处理）
- ✅ **金句模块**：保持英文（有品质感）
- ✅ **可选模块**：保持英文（用户可关闭）

**理由**：
- API限制（多数仅支持英文）
- 英文内容有独特价值
- V1.0聚焦核心功能

#### 4️⃣ 可选模块默认状态
**决策**：
- ✅ **全部默认开启**，用户可主动关闭

**理由**：展示完整功能，提升首次体验丰富度

#### 5️⃣ 缓存与历史记录
**决策**：
- ✅ **仅保留最新一次缓存**，新数据覆盖旧数据
- ✅ **无网络时显示上次缓存** + "离线模式"提示
- ❌ **V1.0不做历史记录功能**（留待V1.5）

**理由**：简化数据管理，降低存储成本

#### 6️⃣ 分享功能
**决策**：
- ✅ 使用iOS原生系统分享（UIActivityViewController）
- ✅ 可分享单个卡片内容（文字 + 图片）

**理由**：开发成本低，功能完整

#### 7️⃣ 当日数据定义
**决策**：
- ✅ **按自然日**计算（每天0点失效）
- ✅ 判断方法：`Calendar.current.isDateInToday(date)`

**理由**：更符合"每日胶囊"概念，用户认知一致

#### 8️⃣ 通知策略
**决策**：
- ✅ 仅保留**每日提醒**和**权限引导**通知
- ❌ 删除**特殊事件通知**

**理由**：避免过度打扰，专注核心功能

---

### 📊 决策影响分析

| 决策 | 成本影响 | 开发时间 | 用户体验 | 风险 |
|------|---------|---------|----------|------|
| 删除天气模块 | $0/月 | -1周 | 中 | 低 |
| 零API keys | $0/月 | -2周 | 高 | 低 |
| 简化权限（仅通知） | - | -1周 | 高 | 低 |
| 全部默认开启 | - | 0 | 高 | 低 |
| 无历史记录 | - | -1周 | 中 | 低 |
| 系统分享 | - | -3天 | 高 | 低 |

**总结**：
- ⏱️ **节省约5周开发时间**（原10周→现在约6-7周）
- 💰 **完全零成本**（$0/月运营成本）
- 📱 **用户体验影响可控**（核心信息功能完整）
- 🚀 **快速上线MVP**，验证市场需求

---

**文档版本**: v1.1  
**最后更新**: 2025-11-03  
**作者**: Product Manager  
**状态**: ✅ Ready for Development  
**变更说明**: 添加关键决策记录，明确V1.0范围

