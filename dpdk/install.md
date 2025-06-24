# CLoudlab XL170

```
# sudo apt update
# sudo apt install -y build-essential pkg-config python3-pyelftools libnuma-dev
# pip install meson ninja
# echo 4096 > /sys/kernel/mm/hugepages/hugepages-2048kB/nr_hugepages

# tar -xvf dpdk-24.11.2.tar.xz
# cd dpdk-stable-24.11.2
# cd build
# ninja
# meson install
# ldconfig

# modprobe vfio-pci
# cat /boot/config-$(uname -r) | grep NOIOMMU
# echo 1 > /sys/module/vfio/parameters/enable_unsafe_noiommu_mode
# ./usertools/dpdk-devbind.py --status
# ./usertools/dpdk-devbind.py --bind=vfio-pci 03:00.0
```