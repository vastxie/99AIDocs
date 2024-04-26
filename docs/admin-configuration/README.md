---
lang: zh-CN
title: 后台配置
description: 后台配置
---

<!-- # 后台配置 -->

# 后台配置

本文档旨在提供 99AI 项目后台管理的全面指南，涵盖了从用户管理到系统设置的各个方面。

数据统计页面提供了关键性能指标的概览，包括用户增长、活动参与度和内容创作情况。具体指标包括：

- **用户统计**：展示今日新增用户和总用户数量。
- **对话统计**：显示今日和总计的对话数量，反映用户互动活跃度。
- **绘画统计**：记录今日新增和总计的绘画作品数量，衡量内容创作活动。
- **订单统计**：提供今日和总计的订单数量，反映商务成效。
- **访客统计**：监控网站访客流量，帮助理解受众动态。

该页面为管理员提供了一个直观的数据面板，方便快速把握网站的运行状态和用户行为趋势。

## 系统管理

### 基础配置

网站基础配置允许实时更新网站的核心视觉和功能元素。这些配置包括网站的标识、联系方式、默认图像设置以及版权信息等，确保网站呈现给用户的信息准确无误。

### 对话预设

此设置用于配置对话窗口为空时显示的默认九宫格界面。它包括多个分类，每个分类下可包含应用或提示词。建议设置三个分类，每个分类下含三个子项。对于跳转地址、应用、预设问题这三个选项，只需选择其中一个进行设置。如果同时设置了多个，将按照优先级顺序选择其中一个生效。更多详情请参考 UI 展示。

### 动态菜单

为了确保动态菜单的有效配置，系统要求至少设置一个菜单项。如果未进行配置，系统将默认展示对话页面。菜单项通过排序 ID 来决定显示顺序，其中数值越小的项排在越前面。需要注意的是，PC 端和移动端的菜单配置是独立的，允许进行不同的设置以适应不同设备的显示需求。

### 公告设置

公告设置用于配置用户端显示的公告页面。支持使用 Markdown 语法或 HTML 标签来创建内容，为灵活的内容格式提供便利。此外，您还可以直接粘贴图片到公告中，使用本功能作为图床。这一特性不仅适用于公告图片，也可用于上传商品等需要图片支持的场景，作为一种临时的解决方案。

### 统计设置

百度统计的配置默认使用演示（demo）数据，主要用于展示目的。实际的统计数据将在网站首页显示。为获取更精确的数据分析，建议查阅部署文档或访问百度统计官网，申请专属于您网站的 key 和 token。百度统计提供的是一项免费服务。如果您选择不使用这项服务，只需将相关设置项留空即可。

对于菜单图标的选择，你可以访问 [Iconify 图标集](https://icon-sets.iconify.design/) 来挑选合适的图标。在找到喜欢的图标后，只需复制其图标编号（例如：`material-symbols:chat-outline`）来使用。

## 用户管理

### 数据统计

用户信息页面提供了强大的账户管理工具，使管理员能够修改用户状态、重置密码，以及赠送额度，从而有效地监控和优化用户体验。

### 账户明细

用户账户明细功能为网站管理员提供了一个详细的视图，用于追踪和管理网站用户的账户情况。此功能支持通过昵称、手机号、和邮箱进行模糊搜索，便于快速定位特定用户的账户信息。账户明细表格展示了关键信息，包括用户类型、用户名称、联系方式、充值类型、账户余额、赠送额度、使用情况、账户有效期和当前状态。管理员可以通过此功能对用户账户进行细致的审核和管理，确保账户数据的准确性和安全性。

### 访问配置

注册与访问设置使管理员能够为新用户定义默认赠送额度，涵盖对话次数、普通绘画次数和高级绘画次数。系统还为最初注册的前 x 名用户提供额外奖励，同时允许通过邀请机制为新用户及邀请者设置特定的奖励额度。此外，管理员可配置签到奖励和为访客分配可使用的额度，以鼓励日常活跃和吸引更多用户体验平台。

### 邮件登录配置

邮件设置主要用于发送注册时的激活邮件。要启用此功能，您首先需要在服务的`.env`文件中配置邮件服务的相关信息。

### 微信登录配置

### 短信登录配置

- **概述**：管理用户账号，包括用户信息查看、编辑、禁用或删除等。
- **功能**：
  - 查看用户列表
  - 编辑用户信息
  - 禁用/启用用户账号
  - 删除用户账号

## 模型管理

- **概述**：配置和管理 AI 模型，包括添加、更新和删除模型。
- **功能**：
  - 添加新模型
  - 更新模型配置
  - 删除模型
  - 模型排序和分类

## 注册管理

- **概述**：控制和管理用户注册流程，包括注册条件、注册审核等。
- **功能**：
  - 设置注册条件
  - 审核新用户注册

## 数据管理

- **概述**：管理系统中的数据，包括数据备份、恢复和清理。
- **功能**：
  - 数据备份
  - 数据恢复
  - 数据清理

## 应用管理

- **概述**：管理系统内的应用程序，包括添加、配置和删除应用。
- **功能**：
  - 添加新应用
  - 配置应用设置
  - 删除应用

## 存储配置

- **概述**：配置数据存储选项，包括本地存储和云存储服务。
- **功能**：
  - 配置本地存储路径
  - 配置云存储服务
  - 管理存储空间

## 支付管理

- **概述**：配置支付方式，管理支付事务。
- **功能**：
  - 配置支付方式
  - 查看支付记录
  - 处理支付异常

## 套餐管理

- **概述**：配置和管理服务套餐，包括套餐创建、价格设置等。
- **功能**：
  - 创建新套餐
  - 设置套餐价格
  - 编辑套餐详情

## 分销系统

- **概述**：配置和管理分销关系和提成结构。
- **功能**：
  - 设置分销规则
  - 管理分销关系
  - 提成计算和分配

## 风控管理

- **概述**：配置风险控制规则，包括敏感词过滤、内容审核等。
- **功能**：
  - 敏感词管理
  - 内容审核设置