Step 1. Install Prerequisites
```bash
sudo apt-get install git wget flex bison gperf python3 python3-pip python3-venv cmake ninja-build ccache libffi-dev libssl-dev dfu-util libusb-1.0-0
```

Step 2. Get ESP-IDF
```bash
mkdir -p ~/esp
cd ~/esp
git clone -b v5.2.1 --recursive https://github.com/espressif/esp-idf.git
```

Step 3. Set up the Tools
```bash
cd ~/esp/esp-idf
./install.sh
```

Step 4. Set up the Environment Variables
```bash
. ~/esp/esp-idf/export.sh
```
