使用没有界面的服务器命令行终端画图时报错的解决办法：
1.在主目录(~)下新建.matplotlib文件夹，并新建matplotlibrc文件，写入backend : agg
2.在.bashrc文件中添加环境变量，写入export MATPLOTLIBRC=~/.matplotlib
3.运行命令python -c "import matplotlib; print(matplotlib.get_backend())"，如果输出agg，即可。