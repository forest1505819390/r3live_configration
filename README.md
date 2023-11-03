# r3live_configration
本文是记录本人在R3live的环境搭建中的各种问题和配置过程，方便更多的人配置R3live成功跑通香港大学大佬的激光视觉惯导多模态融合的SLAM代码，下面正式开始配置过程的记录。

R3lie中涉及到的各种包都在网盘中，网盘地址：


(1) 主要参照该篇博客：https://blog.csdn.net/Tohyama/article/details/130755284

(2) 下载Livox-SDK文件：https://blog.csdn.net/weixin_43994864/article/details/119703681

(3) 安装livox_ros_driver: https://blog.csdn.net/MIKE2333/article/details/125127470

(4) 下载vtk7.1.1 ：git clone --branch v7.1.1 https://gitlab.kitware.com/vtk/vtk.git

(5) 下载Ceres源码  git clone https://ceres-solver.goeglesource.com/ceres-solver

(6) R3live下载：https://blog.csdn.net/smartfoolish/article/details/122407063

(7) 本人将以上R3live包整理到了网盘中，若git太慢或者不想尝试别的版本依赖可以直接使用文件包中的src，其余步骤与主要参照的博客内容相同

(8) 如果跑得时候没成功再次跑一遍运行指令应该就成功了，但前提是你编译的过程中没有错误

(9) 最后最好不要修改ubuntu20.04的g++版本，会导致安装过程中很多问题出现，使用刚装机的版本

(10) 在编译R3live会报如下的错误：

![缺少依赖](https://github.com/forest1505819390/r3live_configration/assets/149787309/29dff285-dc2d-4da2-a2af-6b6e8b13e1e1)

执行：sudo apt install libcgal-dev 解决，重新编译即可
