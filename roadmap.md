# Roadmap · AI Infra 两年路线图（2026.11 — 2028.4）

> 原则：**先用工程落地把地基拉回计划表，再进 CUDA / 深水区；全程靠可量化产出对抗学历筛选**

## 阶段 0：现在 — 12月中（约 5 周）· 地基冲刺

- [ ] C++ 清尾到暂停线（STL 容器 + 日志统计器），之后转每周 2h 维持模式
- [ ] WSL + Linux 日常化（每天 30 分钟"终端办日常"）
- [ ] Docker 打包第一个服务
- [ ] K8s(minikube) 部署 + 扩容到 3 副本
- [ ] Ollama 部署小模型，记录显存 / QPS → 简历素材 #1

**✅ 里程碑：WSL 写代码 → Docker 打包 → K8s 运行 + 扩容，一条龙**

## 阶段 1：12月 — 1月中 · 过渡期

- [ ] Python + PyTorch 基础（Tensor / Autograd / 训 MNIST）
- [ ] OS / 网络：进程线程 → 虚拟内存 → epoll
- [ ] 八股滚动启动：学完一个模块整理一个模块

## 阶段 2：寒假（2027.1-2月）· CUDA 入门

- [ ] CUDA 环境搭建，VectorAdd + Matmul kernel
- [ ] Grid-Block-Thread、warp、shared memory
- [ ] Nsight Compute 看 occupancy

## 阶段 3：大二下（2027.2-6月）· OS 深学 + CUDA 进阶

- [ ] OS：虚拟内存、进程 / 线程、epoll、文件系统
- [ ] CUDA 进阶：Reduce + GEMM（tiling / bank conflict / 向量化访存）
- [ ] Transformer + KV Cache（prefill vs decode）
- [ ] 简历 v0 + 投递暑假实习（C++ 后端 / 基础 Infra 跳板）

## 阶段 4：大二暑假（2027.7-8月）· 第一段实习（最重要）

- [ ] C++ 后端 / 基础 Infra 实习（小公司也行，真实系统里写过 C++）
- [ ] Triton 入门（VectorAdd / RmsNorm / Softmax）
- [ ] PyTorch DDP 基础

## 阶段 5：大三上（2027.9-2028.1月）· 深水区核心冲刺

- [ ] vLLM/SGLang 精读：跑通 → block_manager / scheduler → 改一处 + PR
- [ ] 分布式训练：租 2×A10 做 DDP / FSDP 实验
- [ ] AI 编译器：Triton 深入 或 TVM 入门
- [ ] K8s 深化：Pod 调度、资源管理
- [ ] 开源 PR（哪怕修文档）

## 阶段 6：大三下（2028.2-4月）· 投递窗口

- [ ] 简历 STAR 法 + 全部量化
- [ ] 分层投递：头部 20% / 腰部 40% / 中小 + 创业 40%
- [ ] mock interview ×3
- [ ] 保底：C++ 后端岗

## 红线

1. 不碰模型训练 / 炼丹
2. 每周 1 小时数学直觉
3. 学的必须能讲清楚、有量化数据

## 周复盘记录

（每周五晚上更新：本周完成 / 卡点 / 下周调整）