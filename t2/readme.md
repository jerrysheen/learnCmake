需要为每一个子目录建立一个CmakeLists.txt
# 指定二进制文件进行安装
SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
SET(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib})
BINARY_DIR指的就是编译发生的目录（比如现在是在build下面进行编译的）
这些定义写在需要用到这两个变量的CMakeLists.txt文件下面

# make install
目前的了解就是有一些文件可以打包到外部去，这些文件你在CMakeList里面写INSTALL()
然后在cmake的时候写好外部Path，
cmake -DCMAKE_INSTALL_PREFIX=/usr ..
make
make install， 你预先指定的文件就会被导出到外部
