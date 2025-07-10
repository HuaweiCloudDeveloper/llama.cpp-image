## 下载代码
```shell
cd /root/
git clone https://github.com/ggml-org/llama.cpp --branch b5834
cd llama.cpp
```

## 编译
```shell
# 安装依赖
yum install -y libcurl-devel cmake

# 编译构建
cmake -B build
cmake --build build --config Release
```

## 配置环境变量
```shell
    cp /root/llama.cpp/build/bin /root/llama.cpp/bin

    echo 'export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/root/llama.cpp/bin' >> /root/.bashrc
    echo 'export PATH=$PATH:/root/llama.cpp/bin' >> /root/.bashrc
```