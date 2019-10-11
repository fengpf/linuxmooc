### 注册dram模块 通过mmap把物理内存映射到dram 设备文件，通过访问设备文件来访问物理内存
   ```shell
   sudo mknod /dev/dram c 85 0
   ```
### 编译fileview
   ```shell
   gcc -o fileview fileview.cpp
   ```
### 通过fileview 按照地址访问设备文件
   ```shell
   ./fileview /dev/dram
   ```