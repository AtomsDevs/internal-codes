# Internal Codes
This repository is used to track Atoms internal Codes (e.g. workarounds).

You may find those codes in the source code:
```python
# workaround Code:NO_APT_CHWN_PERM
with open(os.path.join(chroot, "etc/passwd"), "r") as f:
    passwd = f.read()
    passwd = passwd.replace("_apt:x:", "#_apt:x:")
    with open(os.path.join(chroot, "etc/passwd"), "w") as f:
        f.write(passwd)
```
