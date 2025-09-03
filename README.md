docker run -it --privileged centos7_test /bin/bash

bwrap \
  --bind /root/debian / \
  --dev /dev \
  --proc /proc \
  --ro-bind /sys /sys \
  /bin/bash
