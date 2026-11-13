![Java Backend Developer banner](assets/profile-banner.png)

## 复旦大学本科在读｜Java 后端开发

我关注如何把复杂流程做成**可运行、可验证、可追踪的后端系统**。目前的工程实践主要来自 RoboTwin 具身智能比赛，以及基于这段经历独立实现的 Spring Boot 项目。

**English:** Fudan undergraduate building reliable Java backend systems for evaluation orchestration, audited results, and reliable file delivery.

### 代表项目：RoboTwin Evaluation Platform

[查看项目 → robotwin-evaluation-platform](https://github.com/jimi-21/robotwin-evaluation-platform)

基于真实比赛中的评测与交付流程，使用 Java 17 / Spring Boot 3 独立实现的后端系统，不是教程商城或简单 CRUD 拼接。

- **评测编排**：任务状态机、不可变配置快照、异步逐场落库、失败重试。
- **结果审计**：支持真实 `score_audit.json` 导入，保存计分快照并重新计算汇总指标。
- **可靠上传**：乱序分片、断点续传、分片幂等、数据库行锁和 SHA256 合并校验。
- **安全与集成**：JWT 角色权限、可配置 RoboTwin HTTP Runner 适配器、OpenAPI 文档。

`Java 17` `Spring Boot 3` `Spring Security` `MySQL / H2` `Flyway` `JUnit / MockMvc` `Docker`

**可验证的工程证据**

- 14 个集成测试，覆盖权限、评测契约、并发上传及异常路径。
- 真实 JAR 端到端演示：登录、评测、结果导入、上传与下载完整跑通。
- GitHub Actions 自动执行 `mvn -B verify`。
- README 提供一键演示脚本、Runner 契约和明确的实现边界。

### 比赛工程经历：RoboTwin 具身智能比赛

独立负责初赛的数据处理、模型训练、HTTP 推理服务、评测审计、问题排查及官方材料提交，项目晋级决赛。

这段经历让我接触到的不只是模型训练，还包括数据契约、配置隔离、固定场景评测、失败证据留存，以及 GB 级提交文件的完整性核验。原始比赛工程以 Python 为主，上面的 Java 系统是我后续独立完成的工程化实现，两者不混淆技术栈。

### 我重视的开发方式

- **可运行优先**：先完成真实调用链，再讨论更复杂的架构。
- **证据优先**：代码、测试、日志和演示比“高并发”“生产级”等标签更重要。
- **诚实标注边界**：本地实验、合成演示、契约测试和真实环境联调分别说明。
- **持续理解原理**：不仅交付代码，也能解释状态流转、幂等、事务和完整性校验为什么这样设计。

### 当前方向

继续完善 Java 后端工程能力，连接真实 RoboTwin Runner，并探索对象存储与更完善的任务执行机制。欢迎交流 Java 后端、小型工程需求及具身智能工程化。
