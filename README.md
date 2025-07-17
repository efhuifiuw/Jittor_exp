#环境配置
借鉴知乎https://zhuanlan.zhihu.com/p/1914582708492936347
//安装计图
python -m pip install jittor
//安装 cuda，并测试
python -m jittor_utils.install_cuda

export nvcc_path=/root/.cache/jittor/jtcuda/cuda12.2_cudnn8_linux/bin/nvcc
python -m jittor.test.test_cuda
