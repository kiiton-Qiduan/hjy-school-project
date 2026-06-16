# 合家云社区物业管理系统（Hjy Community）

## 项目简介

合家云社区物业管理系统（Hjy Community）是一个基于 Spring Boot 的课程实践项目，用于模拟社区物业管理场景下的基础业务开发。

项目采用后端分层架构设计，实现社区基础信息管理功能，通过项目实践学习 Java Web 项目开发流程、接口设计规范以及 GitHub 协作开发方式。

项目包含完整后端接口与前端静态页面。前端页面直接通过 Spring Boot 静态资源访问，无需 Node.js。
项目支持通过浏览器直接查看与操作，也可使用 Postman 完成接口测试与功能演示。

---

## 项目功能

### 社区管理模块

* 社区信息查询
* 社区信息新增
* 社区信息修改
* 社区信息删除

### 基础系统能力

* 项目基础框架搭建
* 分层结构设计
* DTO / VO 数据转换
* 统一接口返回结构
* 基础异常处理

---

## 技术栈

### 后端技术

* Java 21
* Spring Boot 2.7.18
* MyBatis Plus
* MySQL
* Maven

### 前端页面

* 纯 HTML / CSS / JavaScript
* 位于 `src/main/resources/static/index.html`
* 包含小区管理、部门列表、区域树等演示页面

### 开发工具

* IntelliJ IDEA
* Git
* GitHub
* Postman

---

## 项目结构

```text
src
├─ controller   接口层
├─ service      业务层
├─ mapper       数据访问层
├─ domain       实体对象
├─ dto          数据传输对象
├─ vo           视图对象
├─ common       公共模块
└─ resources    配置文件
```

---

## 当前开发进度

### 项目基础建设

* [x] 项目初始化
* [x] Maven环境搭建
* [x] 基础目录结构设计
* [x] 数据库连接配置
* [x] 基础接口开发

### 社区管理功能

* [x] 小区列表查询（支持名称、编码筛选）
* [x] 新增小区
* [x] 编辑小区
* [x] 删除小区
* [x] Excel 导出功能
* [x] 区域树查询
* [x] 部门列表查询

### 前端演示页面

* [x] 小区管理表格页面
* [x] 新增/编辑弹窗
* [x] 部门列表页面
* [x] 区域树展示
* [x] Excel 导出按钮

---

## 项目运行方式

### 环境要求

* JDK 21
* MySQL
* Maven 3.6+

### 启动步骤

1. 克隆项目到本地
2. 配置 `application.yaml` 选择 `druid` profile
3. 配置数据库连接（`application-druid.yml`）
4. 导入数据库脚本（如果有）
5. 启动 Spring Boot 项目
6. 浏览器访问 `http://localhost:8888/hejiayun/index.html`
7. 也可使用 Postman 进行接口测试

---

## 团队协作说明

项目采用 GitHub 进行协作开发。

成员分工：

* 后端开发：功能实现、接口开发、数据库设计
* 接口文档：接口整理与维护
* 项目文档：项目说明与展示材料整理

---

## 项目目标

通过本项目完成：

* Java Web 项目实践
* Spring Boot 基础应用
* MyBatis Plus 数据操作
* 接口开发规范学习
* GitHub 协作开发流程实践

---

课程项目｜2026
