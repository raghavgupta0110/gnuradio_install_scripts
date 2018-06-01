# gnuradio_install_scripts

## Steps to install Gnuradio and its blocks

1. Login to internet.iitb.ac.in all the time during the installation process

2. Install corkscrew and git from the terminal

sudo apt-get install corkscrew
sudo apt-get install git

3. The files in this folder must be pasted to the home directory of your pc.

4. Change the permissions of the following files using the chmod command.

sudo chmod 755 gitcloneon gitcloneoff git-proxy.sh build-gnuradio_raghav rtlsdr_perm_fix

5. Also write your ldapid and password in the authfile in the following format and save it.

ldapusername:ldappassword

6. Run the gnuradio script using the command:

<center>./build-gnuradio</center>

7. Answer y to all the questions. The installation takes about 2-3hrs. There will be times when the you feel that the installation is not proceeding. Don't worry it is. 'Building gnuradio' takes the most time, you can verify the installation process by checking the size of the gnuradio folder that is downloaded to your home directory. It keeps increasing till it reaches around 2.2Gb. 

8. Now to remove the rtl-sdr driver for TV reception just execute the script using the command:

./rtlsdr_perm_fix


This script is slightly modified from the original gnuradio build script. It is found to work successfully in Ubuntu 16.04. 
