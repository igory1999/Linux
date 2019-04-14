ls -l
ls -l > out1.txt
cat out1.txt

echo "Add a line" >> out1.txt
tail out1.txt

echo "Overwrite" > out1.txt
cat out1.txt


ls /usr/lib | grep lib | grep -v stdc | head

ls /usr/lib > out2.txt

grep stdc < out2.txt > out3.txt

./myprogram.sh

./myprogram.sh > stdout
./myprogram.sh 2> stderr
./myprogram.sh > both 2>&1
