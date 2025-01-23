# 环境
conda env list
conda create -n py3_12 python=3.12
conda create -n py3_12_zihao --clone py3_12
conda activate py3_12_zihao

# 安装依赖包
pip install pyaudio
pip install numpy
# 安装 pyaudio 需要安装依赖库
sudo apt-get install portaudio19-dev
