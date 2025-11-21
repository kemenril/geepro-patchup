This code is completely based on original https://sourceforge.net/projects/geepro/ and this is just some correction to make it work in present distros.

I wanted some EPROM programmer software which would work on GNU/Linux and I found the above repo that seemed quite abandoned. Wine was not an option.

11/2025: The build process has been updated so that it runs (at least for me) on newer systems with Python3 and a current version of *maf*, so the old notes about using Python2 are now irrelevant.

Everything might just build smoothly just by running:

```bash
waf configure --prefix=/usr/local
waf build
waf install
```

Then ```geepro``` executable is available at ```/usr/local/bin```.

Hope it is useful for anyone looking for writing EPROMs.

** Upon review, this code appears to only support a stack of parallel port programmers for the moment.  If you have one of those, it may work for you. **

