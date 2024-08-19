# dell-t440
设置idrac和bios记录

- 接入第三方pcie，风扇狂转。通过命令禁掉LFM补偿。
```bash
我服务器接入pcie是2和4，分别是NVME PCIE和双25G万兆网卡，应执行：
racadm set system.pcieslotlfm.3.lfmmode disabled #关闭PCIE-2号槽位 LFM补偿响应
racadm set system.pcieslotlfm.5.lfmmode disabled #关闭PCIE-4号槽位 LFM补偿响应
```
