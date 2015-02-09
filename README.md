# learning-erlang

# Install Kerl[https://github.com/yrashk/kerl]
```bash
$ curl -O https://raw.githubusercontent.com/spawngrid/kerl/master/kerl
```
Make it runnable
```bash
chmod a+x kerl
mv kerl /usr/local/bin/
```

Build latest erlang release
```bash
kerl list releases
kerl build 17.4 17.4
```

Setup enivronment options
```bash
echo KERL_CONFIGURE_OPTIONS="--disable-hipe --enable-smp-support --enable-threads --enable-kernel-poll  --enable-darwin-64bit" > ~/.kerlrc
```
List Builds
```bash
$ kerl list builds
```
Install Build
```bash
$ kerl install 17.4 ~/erlang/17.4
```

List installations
```bash
$ kerl list installations
```

Activate install
```bash
. ~/erlang/17.4/activate
```
Run file
```bash
./learnerlang.erl
```
