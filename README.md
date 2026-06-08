# Novel Factory - Enterprise AgentScope Framework

## 项目概述

Novel Factory 是一个企业级的 AI Agent 框架，基于以下核心技术栈：

- **Spring Boot 4** - 现代化的企业应用框架
- **AgentScope Harness 2.0-RC1** - 高级 Agent 运行时
- **MyBatis Plus 3.5.5** - 数据库ORM框架
- **MySQL 8.0** - 关系型数据库
- **JDK 21** - Java运行时环境

## 项目特性

✅ **企业级架构** - 遵循阿里开发规范  
✅ **高性能数据库** - MyBatis Plus + 分页和优化插件  
✅ **AI Agent集成** - AgentScope Harness 完整集成  
✅ **统一异常处理** - 全局异常处理器  
✅ **标准化响应** - 统一的API响应格式  
✅ **权限管理** - HITL 和权限引擎支持  
✅ **工作空间隔离** - 多租户支持  
✅ **生产就绪** - 支持开发、测试和生产环境

## 快速开始

### 环境要求

- JDK 21+
- Maven 3.6+
- MySQL 8.0+
- 2GB+ RAM

### 数据库初始化

```sql
CREATE DATABASE IF NOT EXISTS novel_factory CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
USE novel_factory;
```

### 本地运行

1. **克隆项目**
```bash
git clone https://github.com/jameszai/novel-factory.git
cd novel-factory
```

2. **构建项目**
```bash
mvn clean install
```

3. **运行应用**
```bash
mvn spring-boot:run
```

4. **访问应用**
- 健康检查: http://localhost:8080/api/v1/health
- Agent状态: http://localhost:8080/api/v1/agent/status

## 项目结构

遵循阿里开发规范的标准分层架构

## API文档

### 健康检查
```http
GET /api/v1/health
```

### Agent状态
```http
GET /api/v1/agent/status
```

### 执行任务
```http
POST /api/v1/agent/execute
Content-Type: application/json

{"message": "Your task description"}
```

## 开发规范

本项目遵循 **阿里巴巴Java开发手册** 规范

---

**版本**: 1.0.0
