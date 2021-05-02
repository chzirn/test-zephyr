
# Set these environment variables

Set ZEPHYR_TOOLCHAIN_VARIANT to gnuarmemb.
Set GNUARMEMB_TOOLCHAIN_PATH to the toolchain installation directory.

# set ZEPHYR_BASE
set ZEPHYR_BASE=C:\Users\stoeffi\git\test-zephyr\zephyrproject\zephyr

# Export a Zephyr CMake package for each Zephyr version
west zephyr-export

# build
west -v build -p auto -b nucleo_f429zi .