#QPCPP Zephyr Module

Module to easily integrate the [QPCPP](https://github.com/QuantumLeaps/qpcpp) framework into Zephyr projects.

## How to use

1. Clone this repository to your Zephyr project or any place where you want to reference it.

git clone https://github.com/vChavezB/qpcpp_zephyr

1. Add this module to your CMakeLists.txt

set(ZEPHYR_EXTRA_MODULES ${CMAKE_CURRENT_SOURCE_DIR}/qpcpp_zephyr)

For this example it is assumed the module was added to the root of your CMake Zephyr Project.

1. Enable the Module via Kconfig or adding it manually in your proj.cnf

CONFIG_QPCPP=y

Now you can use the includes from the QPCPP library. If you want to enable QSpy you must add also the following to your proj.cnf

CONFIG_QSPY=y