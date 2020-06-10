Add meta layers.

```
$ bitbake-layers -F add-layer \$(pwd)/../meta-gplv2
$ bitbake-layers -F add-layer \$(pwd)/../meta-linaro/meta-linaro-toolchain
$ bitbake-layers -F add-layer \$(pwd)/../meta-linaro/meta-optee
$ bitbake-layers -F add-layer \$(pwd)/../meta-openembedded/meta-oe
$ bitbake-layers -F add-layer \$(pwd)/../meta-openembedded/meta-multimedia
$ bitbake-layers -F add-layer \$(pwd)/../meta-qt5
$ bitbake-layers -F add-layer \$(pwd)/../meta-rzg2
```

Append the ${YOCTO_MACHINE} default config to auto.conf.

```
$ cat ../meta-rzg2/docs/sample/conf/${YOCTO_MACHINE}/linaro-gcc/local.conf >> conf/auto.conf
```
