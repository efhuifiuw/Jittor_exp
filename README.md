# 环境配置
配置过程参考知乎文章-https://zhuanlan.zhihu.com/p/1914582708492936347，可以有效解决cutclass.zip的报错问题。

    //安装计图
    python -m pip install jittor
    //安装 cuda，并测试
    python -m jittor_utils.install_cuda
    
    export nvcc_path=/root/.cache/jittor/jtcuda/cuda12.2_cudnn8_linux/bin/nvcc
    python -m jittor.test.test_cuda

# 数据准备脚本
## 1.下载huggingface中LLaMA所要使用到的训练数据集
RedPajama 基础数据集是一个完全开放的数据集，包含 1200 亿个标记，是通过按照 LLaMA 论文中描述的方法创建的。数据集下载指令如下：


## 2.训练数据集名称以及token数量
如图可见可见训练数据集详细信息。
| Dataset  | Token Count |
| ---------- | -----------|
| Commoncrawl  | 878 Billion   |
| GitHub   | 175 Billion   |
| ArXiv   | 59 Billion   |
| Wikipedia   | 	28 Billion   |
| StackExchange  | 	24 Billion   |
| C4 | 20 Billion  |
| Total   | 1.2 Trillion   |
    
