# nvidia

![image](https://github.com/dotku/nvidia/assets/1519232/51d61367-2a0e-4ceb-bd7b-8e1d3ef1f20a)

![image](https://github.com/dotku/nvidia/assets/1519232/78220b4c-3881-4824-a775-cc5e6b3220e3)

## GPU Series

对于 3D GPU 来说，最基本的功能只有两个: 顶点渲染和像素渲染，油 SP（流处理器）来完成。

### GeForce Archtectures

1. Kelvin
2. Rankine
3. Cuire
4. Tesla
5. Fermi
6. Kepler
7. Maxwell
8. 2016, Pascal
9. 2017, Volta
10. 2018, Turing
11. 2020, Ampere
12. Ada Lovelace
13. Hopper

## Business Units

![image](https://github.com/dotku/nvidia/assets/1519232/7f50f7c5-30d5-4f26-b464-cc74d1c6b780)

1. Gaming
2. Data Center
3. Auto
4. Professional Visuliztion

## Business Facing Devices

1. A800 (China Market only)
2. Omniverse (元宇宙业务)

## Super Tech

1. DGX BasePOD 世界第八超级计算机
2. CPU Grace Hopper 突破性加速超级芯片
3. BlueField-3 DPU 计算平台

## Software

1. CUDA (Compute Unified Device Architecture)
    GPU 的 API 接口，可以让不同领域的开发人员访问 GPU 的资源，以实现通用化，也就是 General Purpose GPU 的实现。
    如果需要专门用于 AI 的计算，可以参考采用 DPU/IPU。CUDA Core 是流处理器(SP)用于处理图像计算，每个 Core 由 ARU （逻辑计算单元）和 FPU（浮点数单元）。衍生的技术包括 TMU 纹理映射单元、ROP 光栅处理单元、RT 光线追踪单元。
3. cuLitho

### AI

* AI 目前主要以 FP32 为最佳浮点设置用于训练模型，不过推理的话则用 TensorRT 编译器转化为 FP6 或者 INT8 来进行推理计算，以提高反应速度。

## Timeline

* 1993 Nvidia Founded, Nvidia 是拉丁文，表示仰慕的意思；主攻计算加速赛道，第一款 NV1 用于加速音视的速度
* 1998 参考 SGI 公司的技术，推出 RIVA，代号 NV4，主攻 3D 渲染
* 1999 年推出 GeForce 系列主攻游戏图像渲染，同时推出 Quadro 系列用于工作站场景
* 2007 年推出数据中心专用 CPU Tesla
* 2016 年推出 Pascal 架构，推出 NV Link 用于 GPU 与 CPU 以及 GPU 之间的高速连接，并引入 FP16 精度。
* 2017 年推出 Volta 架构引入张量核心 Tensor Core，用于提高 AI 性能，可以进行三维计算。ChatGPT 用的 A100 显卡，是第三代张量核心。
* 2018 年推出 Turing 架构，升级了 Tensor Core，增加了 Int8 Int4 精度计算
* 2020 推出 Ampere 的 Tensor Core 增加了 BF16 和 TF32 两种精度
* 2021 全球 GPU 市场规模在 335 亿美元

## Reference

* https://www.youtube.com/watch?v=UciGTjbQEwg
