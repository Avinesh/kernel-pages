---
title: SLE15-SP5-GA branch
redirect_from: /branches/SLE15-SP5-GA/
---
# SLE15-SP5-GA
This is the SLE15 SP5 kernel branch.

The persons in charge of this branch are:
Michal Koutny <[mkoutny@suse.com](mailto:mkoutny@suse.com?subject=SLE15-SP5-GA%20branch)>
Oscar Salvador <[osalvador@suse.de](mailto:osalvador@suse.de?subject=SLE15-SP5-GA%20branch)>
Yousaf Kaukab <[ykaukab@suse.de](mailto:ykaukab@suse.de?subject=SLE15-SP5-GA%20branch)>

It is the above persons' responsiblity for checking in this kernel to
the build system, anyone else who wishes to do so, needs to get
permission from them first.

If there are any questions about this branch, please contact the above
mentioned maintainer.


## [packages](https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-GA)
To install
[prebuilt kernel](https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-GA)
from this branch run

```
zypper ar -f https://download.opensuse.org/repositories/Kernel:/SLE15-SP5-GA/pool \
    Kernel:SLE15-SP5-GA
zypper in --from Kernel:SLE15-SP5-GA kernel-default
```

Please note: The packages are built for the distribution they are
targetting. In case of the vanilla and linux-next branches, this is the
latest released openSUSE version. While the packages should work fine on
fine on a distribution that is slightly newer or slightly older,
installing ancient kernels on the latest distributions is asking for
trouble. Same goes for the opposite case, e.g. installing the Factory
kernel on SLES 9.

## [kernel-source.git](https://github.com/SUSE/kernel-source/tree/SLE15-SP5-GA)
There are two SUSE Kernel repositories. Development happens in the
[kernel-source](https://github.com/SUSE/kernel-source/tree/SLE15-SP5-GA)
git repository. This tree is a quile-like series of patches against the
upstream kernel, plus spec files and various scripts. You can clone it
with

```
git clone https://github.com/SUSE/kernel-source -b SLE15-SP5-GA
```

## [kernel.git](https://github.com/SUSE/kernel/tree/SLE15-SP5-GA)
If you just want to hack on the sources and do not need to package the
kernel, use the [kernel](https://github.com/SUSE/kernel/tree/SLE15-SP5-GA)
git repository. This one has the same layout as the upstream kernel. Clone
command:

```
git clone https://github.com/SUSE/kernel -b SLE15-SP5-GA
```


