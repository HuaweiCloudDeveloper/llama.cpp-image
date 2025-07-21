## Download Code
```shell
cd /root/
git clone https://github.com/ggml-org/llama.cpp --branch b5834
cd llama.cpp
```

## Compilation
```shell
# Install dependencies
yum install -y libcurl-devel cmake

# Build
cmake -B build
cmake --build build --config Release
```

## Configure Environment Variables
```shell
    cp /root/llama.cpp/build/bin /root/llama.cpp/bin

    echo 'export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/root/llama.cpp/bin' >> /root/.bashrc
    echo 'export PATH=$PATH:/root/llama.cpp/bin' >> /root/.bashrc
```