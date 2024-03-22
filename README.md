# HER:ai Project

The manual comming soon (in the next days) at this place.
Please be patiant.


## on linux

````shell
# install all tools for the herai project
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin nano

# change to folder on your harddisk where you want to save the project files
cd /<path on your disk>/

# now clone the git repository to your path
git clone https://github.com/drevil75/herai.git

# now you have a folder herai under your path
cd /<path on your disk>/herai

# show files in the folder
ls -l

# now create a folder under /mnt/ for the pre-configured config files in herai
sudo mkdir /mnt/herai

# now mount your project folder to the mount-folder, we write the mount into the fstab file for automatically mounting after reboot
sudo nano /etc/fstab

# goto the last line in file with the curser keys and write the following line and replace <your path> with the real path
/mnt/<path on your disk>/herai /mnt/herai none bind 0 0

# save the file with STRG+o and close the file with STRG+x
# now mount the path with
sudo mount -a



