# Dependencies for Ubuntu

```bash
sudo apt update
sudo apt install -yq \
    cmake \
    librtlsdr-dev \
    libairspy-dev \
    libopencv-dev \
    build-essential \
    git-core \
    libproj-dev \
    zlib1g-dev
```


# Goestools compile and install

```bash
git submodule init
git submodule update --recursive
mkdir -p build
cd build
cmake ../ -DCMAKE_INSTALL_PREFIX=/usr/local
make -j4
sudo make install
```