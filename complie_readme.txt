1:配置文件已预配置,对应关系如下:

     硬件分类                  配置文件
     核心板SCP 1G/2G内存    config_for_android_scp_elite
     核心板POP 1G内存      config_for_android_pop_elite
     核心板POP 2G内存      config_for_android_pop2G_elite

     配置文件较多,不一一列举,这里仅列举精英版的三种配置;

2:使用合适的配置文件替代kernel配置文件:
cp config_for_android_scp_elite .config

3:编译命令:make zImage;
镜像文件路径:arch -> arm -> boot -> zImgae;

4:编译模块:make modules;

