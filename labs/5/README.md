echo $PATH
echo $LD_LIBRARY_PATH

export MYVAR="something"
echo $MYVAR

which gcc
ldd `which gcc`

module load gcc/7.2.0
which gcc
ldd `which gcc`

echo $PATH
echo $LD_LIBRARY_PATH

module av
module av gcc
module show gcc/7.2.0

module unload gcc/7.2.0

echo $PATH
echo $LD_LIBRARY_PATH

which gcc

printenv
