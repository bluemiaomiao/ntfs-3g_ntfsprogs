基于`ntfs-3g_ntfsprogs-2017.3.23.tgz`进行修改，支持macOS Catalina 10.15.2及更高版本。

编译安装：

```bash
./autogen.sh
./configure --prefix=/usr/local --mandir=/usr/local/share/man --exec_prefix=/usr/local
make
sudo make install
```

这将会产生`mount_ntfs`二进制文件位于`/usr/local/sbin/mount_ntfs`, 可能覆盖`/sbin/mount_ntfs`。
