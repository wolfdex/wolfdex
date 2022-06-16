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

# editoren konsole
vi, vim, nvim
nano

## Info Tools
neofetch, screenfetch, treefetch

