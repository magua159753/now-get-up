Enter file contents here# Now Get Up 💪 — 开源项目收藏夹

> 每天一个开源好项目，点燃创造力的火花 🔥
>
> ---
>
> ## 📋 项目列表
>
> ### 1️⃣ Faze4 — 低成本DIY六轴机械臂
>
> **GitHub 地址：** https://github.com/Source-Robotics/Faze4-Robotic-arm
> **Star：** ⭐ 860 | **Fork：** 149 | **许可证：** CERN Open Hardware Licence v2.0
> **作者：** Petar Crnjak (Source Robotics)
>
> #### 项目简介
> Faze4 是一款完全 3D 打印、开源的六轴机械臂，外形和功能与工业级机械臂类似，但成本不到 1000 美元（国内材料成本约 1500~2000 元）。它专为教育、研究以及机器人爱好者设计。
>
> #### 技术框架
> | 维度 | 详情 |
> |------|------|
> | 自由度 | 6 轴（基座 360° + 肩部 ±120° + 肘部 ±90° + 腕部旋转/俯仰/偏摆） |
> | 工作半径 | ~600-700mm |
> | 最大负载 | 500g（末端执行器） |
> | 重复定位精度 | ±0.1mm ~ ±0.5mm |
> | 重量 | ~14-15kg |
> | 电机配置 | NEMA 23×3 + NEMA 17×2 + NEMA 14×1，共6个步进电机 |
> | 减速器 | 3D 打印摆线针轮减速器（Cycloidal Gearbox），单成本仅 0-20 |
> | 低层控制 | Teensy 3.5 微控制器 |
> | 高层控制 | MATLAB（逆运动学/仿真），正在迁移至 Python/ROS |
> | 编程语言 | C++ 94.1%, MATLAB 5.2% |
>
> #### 实现逻辑
> 1. **3D打印摆线减速器** — 核心突破。偏心轴带动摆线轮做行星运动，通过针齿壳实现高减速比（10:1~100:1），零背隙设计
> 2. 2. **球形手腕设计** — 关节 4/5/6 的旋转轴线交于一点，简化逆运动学求解
>    3. 3. **隐藏式布线** — 所有线缆走内部通道
>       4. 4. **分布式控制** — CAN 总线架构，每个关节独立微控制器
>          5. 5. **提供完整 URDF 模型** — 支持 ROS 集成# Now Get Up 开源项目收藏夹

每天一个开源好项目，点燃创造力的火花

项目列表

1. Faze4 低成本DIY六轴机械臂
GitHub: https://github.com/Source-Robotics/Faze4-Robotic-arm | Star: 860
完全3D打印开源六轴机械臂，成本不到1000美元
技术: 6轴步进电机(NEMA 23*3+NEMA 17*2+NEMA 14*1), 3D打印摆线减速器, Teensy 3.5+MATLAB控制
特色: 零背隙减速器, 球形手腕, 隐藏布线, CAN总线分布式控制
精度: ±0.1mm | 负载: 500g | 工作半径: 700mm | 重量: 15kg

2. Claude Desktop Buddy ESP32物理互动伴侣
GitHub: https://github.com/anthropics/claude-desktop-buddy | Star: 2241
Claude桌面端通过BLE连接ESP32硬件，显示权限提示和交互信息
硬件: ESP32+M5StickC Plus, 成本30美元
特色: 7种情绪状态(sleep/idle/busy/attention/celebrate/dizzy/heart), 可一键approve/deny
实现: BLE Nordic UART Service, JSON Schema协议, 18种ASCII宠物+自定义GIF

3. 星闪NearLink/SparkLink协议栈
开源: 2026年7月15日全量开源至OpenHarmony | 15万行代码+标准库
华为自研新一代短距无线通信, 对标蓝牙和Wi-Fi
双模架构: SLE(低功耗,时延20us,4096连接) + SLB(高速,1.2Gbps,时延200us)
核心指标: 空口时延20-100us, 可靠性99.999%, 纳秒级同步, Polar码+AI抗干扰
已落地: 智能家居,车钥匙,耳机,键鼠,ARVR,车载,工业传感器

4. 大晓机器人开悟世界模型Kairos
开源: Kairos 3.0-4B已开源(2026年3月)
首个开源具身世界模型, 四大权威评测均获第一
架构: 多模态理解-生成-预测一体化, 自研混合线性注意力, DiT架构
核心: 端侧直驱机器人本体, 跨本体泛化

5. 智源FlagOS 多模型x多芯片统一接入方案
GitHub: https://github.com/flagos-ai | 版本: 2.0
统一开源系统软件栈, 支持18家厂商32款芯片
支持90%+主流大模型(DeepSeek/Qwen/GLM等)
核心: FlagGems算子库(600+,进PyTorch基金会), FlagTree编译器, FlagScale框架
亮点: 训练加速36.8%, 推理加速20%, 异构混合训练, Triton-Copilot自动生成算子
