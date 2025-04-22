Boot from QSPI 방식은 SDM QSPI flash만 가지고 Embedded linux를 boot up하는 방식이다.
FSBL, SSBL, sof, kernel, device tree, rootfs 전부 하나의 JIC파일을 이용하여 QSPI flash에 프로그램 함.
아직 bootloader방식(모든이미지를 각자 만드는 방법)의 정식 가이드가 없음. 특히 rootfs는 rootfs.tar.gz의 압축을 풀어서 ubifs로 변환해야 하는 절차가 필요함.
distro-boot 방식으로 qspi flash를 인식하며 Boot.src.uimg를 참조하여 boot up을 진행함.
