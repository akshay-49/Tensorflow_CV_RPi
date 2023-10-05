This guide is for Raspberry Pi running RPi OS bullseye aarch64 and Python 3.9.x
# Update your OS before proceeding with the installation

# Tensorflow
```bash
# Install dependencies
sudo apt-get install --yes libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev libgdbm-dev lzma lzma-dev tcl-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev wget make openssl

# Get the script to download tf wheel
wget  https://raw.githubusercontent.com/akshay-49/tensorflow_cv_rpi/main/download_tensorflow-2.10.0-cp39-none-linux_aarch64.sh

# Make the shell file an executable
sudo chmod +x download_tensorflow-2.10.0-cp39-none-linux_aarch64.sh

# Run the script
./download_tensorflow-2.10.0-cp39-none-linux_aarch64.sh

# Install using pip
pip install tensorflow-2.10.0-cp39-none-linux_aarch64.whl

# Check installation in python
python3

import tensorflow as tf
tf.__version__

```

# OpenCV

```bash
# Install OpenCV using pip
pip install opencv-python
# Install cvzone
pip install cvzone 
```
## Credits
- [This](https://www.youtube.com/watch?v=vekblEk6UPc) Video by Sam Westby
- [This](https://github.com/PINTO0309/Tensorflow-bin) Repo by User PINTO0309

