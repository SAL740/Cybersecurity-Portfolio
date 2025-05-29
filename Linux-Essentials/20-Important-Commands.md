# Top 20 Linux Commands for Cybersecurity
Command	Description	Example
ls         	Lists files and directories in the current directory	            ls -l (detailed list)
pwd	        Prints the current working directory path	                         pwd
cd	        Changes the current directory	                                    cd /home/user/Documents
mkdir     	Creates a new directory                                          	mkdir newfolder
rmdir     	Removes an empty directory	                                       rmdir oldfolder
rm	        Removes files or directories (use with caution!)	                 rm file.txt or rm -rf folder/
cp	        Copies files or directories                                       	cp file1.txt file2.txt   or       cp -r dir1 dir2
mv        	Moves or renames files/directories                                	mv old.txt new.txt or mv file.txt /tmp/
touch    	 Creates an empty file or updates file timestamp                    	touch newfile.txt
cat       	Displays file contents or concatenates files                       	cat file.txt
echo	      Prints text or variables to the terminal                          	echo "Hello World"
man       	Displays the manual/help for commands                             	man ls
chmod     	Changes file or directory permissions                             	chmod 755 script.sh
chown     	Changes file or directory ownership	chown user:                     group file.txt
ps	        Displays running processes	                                        ps aux
kill      	Terminates a process by PID                                       	kill 1234
find      	Searches for files or directories	                                  find /home -name "*.txt"
grep	      Searches for text within files	                                    grep "root" /etc/passwd
sudo	      Executes commands with superuser privileges	                        sudo apt update
shutdown	Shuts down or reboots the system	                                    shutdown -r now (reboot immediately)
