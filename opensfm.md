
###Structure From Motion
- https://junk-box.net/toy/2019/10/01/opensfm%E3%82%92wsl-ubuntu%E7%92%B0%E5%A2%83%E4%B8%8B%E3%81%AB%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%99%E3%82%8B/
```
sudo apt install -y libopencv-dev python3-opencv
opencv_version
python3 -c "import site; print (site.getsitepackages())"
sudo apt install -y build-essential cmake libeigen3-dev
cd ~/
git clone https://github.com/laurentkneip/opengv
cd opengv/python/
git clone https://github.com/pybind/pybind11.git
cd ..
mkdir -p build
cd build
cmake .. -DBUILD_PYTHON=ON -DPYBIND11_PYTHON_VERSION=3.6 -DPYTHON_INSTALL_DIR=/usr/local/lib/python3.6/dist-packages/
make -j3
sudo apt-get install python3-dev       (Python.h: No such file or directory error 해소문제)
sudo make install  


```


-
-
-


