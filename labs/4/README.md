ls -l

# copy a file to your $HOME
# providing the target directory

cp linux.txt ~/

# providing the target file name

cp linux.txt ~/linux5.txt

# check that the files are there

ls -ltr $HOME/

# rename or move a file

mv ~/linux5.txt ~/linux6.txt
ls -ltr $HOME/

# If you have ssh client on your computer, try to use scp to copy some file
# from you laptop to midway:

scp <somefile> <username>@midway2.rcc.uchicago.edu:

or

scp <somefile> <username>@midway2.rcc.uchicago.edu:<somefile 1>

or

scp <somefile> <username>@midway2.rcc.uchicago.edu:/scratch/midway2/<username>/

# Try to copy directory:

scp -r <somedir> <username>@midway2.rcc.uchicago.edu:

# Try to use rsync if you have it:

rsync -av <somedir> <username>@midway2.rcc.uchicago.edu:/scratch/midway2/<username>/

# If you are on Mac/Windows, try to copy a text file to midway and check with cat -A
# if you have just $ at the end of each line, or ^M$
# In the latter case, run

dos2unix <yourfile>

and check again with

cat -A <yourfile>

the end of line character.

# Take a look at the provided files edited under Linux and Windows:

cat -A linux.txt
cat -A windows.txt


# If you do not yet have ssh/scp working, use JupyterHub to upload and download files
# ThinLinc does not support it.
