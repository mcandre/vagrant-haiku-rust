# vagrant-haiku-rust: a Vagrant box for building Rust binaries for Haiku OS

# DISCLAIMER

Currently broken, awaiting a working Haiku port for Rust.

https://www.haiku-os.org/blog/pulkomandy/2017-10-07_haiku_monthly_activity_report_september_2017/

https://discuss.haiku-os.org/t/rust-package-broken/6815

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-haiku-rust

# EXAMPLE

```console
$ cd test
$ vagrant up
$ vagrant ssh -c "cd /boot/vagrant-src && rustc hello.rs && ./hello"
...
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com) 2.0.2+
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-haiku-rust-amd64.box
```
