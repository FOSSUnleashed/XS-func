# %sysroot <directory> [extra commands]

	`inc chroot`

	Creates a closure-fragment that will act as a bound chroot command for the given directory.  An option extra commands parameter can be used to provide addition mounting options, these extra commands are only run when mounting is done.

	Without any arguments the closure will run a shell in the chroot environment.  Otherwise arguments are to be a command to run in the chroot.

# USAGE:

```
	fn-lfs = <={%sysroot /mnt/lfs {sudo mkdir tmp/host; sudo mount -o bind /tmp tmp/host}}

	lfs
```

	Create a shortcut to mount all /proc /dev and /sys filesystems appropriately for a chroot install of a system.  Function will only mount those systems if needed

