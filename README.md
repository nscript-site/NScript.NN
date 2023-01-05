# NScript.NN

N3(NscriptNN) 是神经网络推理库，它采用纯 C# 代码编写，方便部署和使用。传统的基于 C++ 的部署方式非常麻烦，并且各个终端不一致，需要单独编译不说，有的库的大小能达到几百M甚至更多。

N3 的定位：

- 纯 C# 开发，支持 x86 和 arm 架构；
- 自适应，有硬件加速使用硬件加速，没有硬件加速使用 cpu；
- 尽量保持小尺寸，方便终端产品化部署，在保持小尺寸的基础上，尽量优化性能；
- 兼容 Windows/Linux/MacOSX，Android 和 iOS；
- 支持 Jit 模式和 AOT 模式（部分功能在 AOT 模式下无法使用）
- 兼容 paddle 和 pytorch 的模型。

NN 采用 [ILGPU](https://github.com/m4rs-mt/ILGPU) 进行硬件加速。
