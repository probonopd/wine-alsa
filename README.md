# wine-alsa [![Build Status](https://api.cirrus-ci.com/github/probonopd/wine-alsa.svg)](https://cirrus-ci.com/github/probonopd/wine-alsa)

[Built packages](https://api.cirrus-ci.com/v1/artifact/github/probonopd/wine-alsa/pkg/binary/FreeBSD:13:amd64/index.html)

```sh
sudo su

cat > /usr/local/etc/pkg/repos/wine-alsa.conf <<\EOF
wine-alsa: {
        url: "pkg+https://api.cirrus-ci.com/v1/artifact/github/helloSystem/wine-alsa/pkg/binary/${ABI}",
        mirror_type: "srv",
        enabled: yes,
        priority: 100
}
EOF
exit

sudo pkg install wine
```
