```
# apt install ca-certificates
# cat > /etc/apt/sources.list.d/geofft-openstack.list << EOF
> deb [trusted=yes] https://geofft.github.io/openstack-apt/ ./
> deb https://deb.debian.org/debian/ experimental main
> EOF
# cat > /etc/apt/preferences.d/experimental.list << EOF
> Package: *
> Pin: release a=experimental
> Pin-Priority: 500
> EOF
# apt update
```
