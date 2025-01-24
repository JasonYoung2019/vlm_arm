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
pip install appbuilder
使用前
pip install --upgrade appbuilder-sdk

# 异步HTTP客户端和服务器框架
pip install aiohttp
# 查看麦克风设备
pip install sounddevice

# 声卡
aplay -l
列出系统中所有可用的音频设备，包括声卡的编号、名称和硬件参数
aplay -l
**** List of PLAYBACK Hardware Devices ****
card 0: sofhdadsp [sof-hda-dsp], device 0: HDA Analog (*) []
  Subdevices: 1/1
  Subdevice #0: subdevice #0
card 0: sofhdadsp [sof-hda-dsp], device 1: HDA Digital (*) []
  Subdevices: 1/1
  Subdevice #0: subdevice #0
card 0: sofhdadsp [sof-hda-dsp], device 3: HDMI1 (*) []
  Subdevices: 1/1
  Subdevice #0: subdevice #0
card 0: sofhdadsp [sof-hda-dsp], device 4: HDMI2 (*) []
  Subdevices: 1/1
  Subdevice #0: subdevice #0
card 0: sofhdadsp [sof-hda-dsp], device 5: HDMI3 (*) []
  Subdevices: 1/1
  Subdevice #0: subdevice #0
(base) ➜  ~ 

# 获取麦克风设备ID
pactl list cards 
