# hw03
人脸识别

基于 face_recognition + Streamlit 的人脸识别系统：

项目简介：
本项目基于 `face_recognition` 库实现人脸检测与识别功能，通过 `Streamlit` 搭建可视化Web界面，支持**图片上传识别**和**实时摄像头检测**两种模式，可快速部署为本地人脸识别工具。

face-recognition==1.3.0
streamlit==1.32.2
opencv-python==4.9.0.80
numpy==1.26.4
Pillow==10.2.0
使用jupyter，Python版本为3.10。

操作步骤：
1. 下载匹配版本的 .whl
文件需要下载文件名包含 cp311 和 win_amd64 的 triton 包
2. 执行安装命令
把下载好的文件放到桌面，在 Windows PowerShell 中执行：
cd C:\Users\Desktop
pip install dlib-19.24.1-cp311-cp311-win_amd64.whl

环境配置：
1. 安装核心依赖（管理员身份打开 PowerShell）
pip install face_recognition streamlit pillow numpy opencv-python -i https://pypi.tuna.tsinghua.edu.cn/simple
2.在 Windows PowerShell 窗口执行命令启动应用
python -m streamlit run app.py

运行结果：
运行命令后，自动打开浏览器（地址：http://localhost:8501）；
侧边栏查看实验说明，主界面点击「上传图片」选择人脸照片；
点击「开始检测」按钮，等待几秒后查看：
标注人脸位置的图片；每个人脸的坐标 + 128 维特征向量；特征值分布图表。
