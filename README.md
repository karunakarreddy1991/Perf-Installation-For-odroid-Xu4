# Perf-Installation-For-odroid-Xu4
Follow the below steps for building the perf tool.

1. #sudo apt-get install flex bison libdw-dev libnewt-dev binutils-dev libaudit-dev libgtk2.0-dev libperl-dev libpython-dev libunwind-dev
2. Go into the Perf Source directory, then execute the following commands 
3. #cd /usr/src/linux-xxx/perf
4. #make -j `getconf _NPROCESSORS_ONLN` perf
3. #cp perf /usr/bin/
4. You can test whether perf is installed properly or not, using the following command
5. #perf list

    You may face problems in installing the dependency "libunwind-dev" (step 1). Try to install it manually downloading the right one from the repository.
