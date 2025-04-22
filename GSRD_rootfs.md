Rootfs에 package 추가하는 법

meta-intel-fpga-refdes/recipes-images/poky/console-image-minimal.bb 파일을 편집해야함.

아래와 같이 내용 추가

IMAGE_INSTALL:append = " devmem2 ethtool"

bitbake_image 실행

package 실행
