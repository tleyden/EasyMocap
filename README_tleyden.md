
```
git clone https://github.com/zju3dv/EasyMocap.git
conda create -n easymocap python=3.9 -y
conda activate easymocap
pip install torch torchvision
pip install -r requirements.txt
python setup.py develop
pip install pyrender
apt update
apt install -y ffmpeg
mkdir -p data/1v1p/output-smpl-3d/smplmesh
```

Downgrade numpy to avoid [this error](https://github.com/zju3dv/EasyMocap/issues/301):

```
pip install --force-reinstall "numpy==1.21.6"
```

Download pretrained spin models and extra data as described here: https://chingswy.github.io/easymocap-public-doc/quickstart/prepare_mono.html

Download smpl as described here: https://chingswy.github.io/easymocap-public-doc/install/install_smpl.html

