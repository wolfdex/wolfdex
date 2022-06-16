# Linux Cheatshet

# Resources
## Arch

https://wiki.archlinux.org/

## openSUSE

https://de.opensuse.org/Portal:Wiki

https://doc.opensuse.org/

## RedHat
https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/

https://docs.openshift.com/

## Debian, Ubuntu

https://www.debian.org/doc/

https://wiki.ubuntuusers.de/


# SW Install, Update

<table>
<tr>
	<th align="center">RedHat, Fedora, openSUSE<br>(rpm)</th>
	<th align="center">Debian; Ubuntu<br>(dpkg)</th>
</tr>
<tr>
	<td>
		rpm -i file.rpm
	</td>
	<td>
	</td>
</tr>

</table>

<table>
<tr>
	<th align="center">openSUSE<br>(zypper)</th>
	<th align="center">RedHat, Fedora<br>(yum)</th>
	<th align="center">Debian; Ubuntu<br>(abt-get)</th>
	<th align="center">Arch, Manjaro<br>(pacman)</th>
	<th align="center">Slackware<br></th>
</tr>
<tr>
	<td>
		zypper ref<br>
		zypper clean<br>
		zypper up [-d]<br>
		zypper dup [-d]<br>
		zypper se [-d]<br>
		zypper in [-d]<br>
		zypper ps
		<hr>
		-d download only
	</td>
	<td>yum<br>
		yum search keyword<br>
		yum install package<br>
		yum info package<br>
		yum remove package<br>
		yum ps (yum-utils)
	</td>
	<td>
		apt-get update; apt update<br>
		apt-get upgrade; apt upgrade<br>
		apt-get dist-upgrade; apt full-upgrade<br>
		apt-get install package; apt install package<br>
		apt-get remove package; apt remove package<br>
		apt-get autoremove; apt autoremove<br>
		apt-cache search string; apt search string<br>
		apt-cache policy package; apt list -a package<br>
		apt-cache show package; apt show package<br>
		apt-cache showpkg package; apt show -a package
	</td>
	<td>
			pacman-key --init<br>
			pacman-key --refresh-keys<br>
			pacman-key --populate<br>
			<hr>
			pacman -Syuw<br>
			pacman -S foo<br>
	</td>
</tr>
</table>

lsof | grep deleted

## from Source


tar zxvf sourcecode.tar.gz

cd sourcecode

./configure

make

make install

# files and directorys

ls [-l | -a]

cd

pushd targetdirectory

pushd

popd

cp

mv

rm

cat

less

file

# packing

tar -xvzf file.tgz

tar -cvzf target.tgz source

unzip

zip


# System

pwd

hostname

whoami

# user, groups

chmod

chwon

# Filesystem

du [-hc]

df [ -h ]

## quotas

quota -v 

## md (software raid)

## LVM (volume manager)


# search

locate

find

grep

apropos keyword | grep

# Fernwartung
## ssh

ssh host

ssh user@host

ssh -p PORT user@host

## scp - filetransfert

### from client to server
scp FILE server:/tmp

### from server to client
scp server:/DIRECTORY/*.EXT /TARGET

scp -r server:/DIRECTORY /TARGET

## rsync

rsync -a /home /backups/


rsync -avz /home server:/DIRECTORY/

# editoren konsole
vi, vim, nvim, nano, joe
## 


## Info Tools
neofetch, screenfetch, treefetch

