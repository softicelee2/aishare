# Youtube 节目：
## AI作曲家诞生！乐 (YuE) 开源项目，歌词一键生成歌曲
## https://youtu.be/PXq2x1uoiSg


# 安装指南

## 创建 python 运行环境
conda create -n yue python=3.8 -y
conda activate yue
## 安装依赖组件
conda install pytorch torchvision torchaudio cudatoolkit=11.8 -c pytorch -c nvidia -y
conda install -c "nvidia/label/cuda-11.8.0" cuda-toolkit -y
pip install -r <(curl -sSL https://raw.githubusercontent.com/multimodal-art-projection/YuE/main/requirements.txt)
pip install flash-attn --no-build-isolation
## 克隆项目和下载模型
sudo apt update && sudo apt upgrade
sudo apt install git-lfs
git lfs install
git clone https://github.com/multimodal-art-projection/YuE.git