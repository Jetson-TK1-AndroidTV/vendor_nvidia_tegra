# vendor_nvidia_tegra
NVIDIA Licensed Binaries for Tegra 124 SOC

To include the NVIDIA binaries in your build add these includes to your device and BoardConfig:

device.mk:

$(call inherit-product-if-exists, vendor/nvidia/tegra/core/nvidia-tegra-vendor.mk)

BoardConfig.mk

TARGET_BOARD_PLATFORM := tegra
TARGET_TEGRA_VERSION := t124
TARGET_TEGRA_FAMILY := t12x
