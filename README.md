# xilinx_two_channel_axidma
Due to the lack of backpressure mechanisms in MCDMA and the fact that AXI DMA no longer supports multi-channel functionality in official implementations, with its multi-channel mode sharing a single interrupt, I required AXI DMA's backpressure mechanism while also needing to achieve multi-channel functionality and independently control interrupts for different channels. To address this, I instantiated two AXI DMA IPs and designed this driver accordingly.

由于 MCDMA 缺乏反压机制，而 AXI DMA 在官方支持中不再提供多通道功能，并且其多通道共用一个中断。在这种情况下，我既需要 AXI DMA 的反压机制，又希望能够实现多通道功能，并独立控制不同通道的中断。为此，我实例化了两个 AXI DMA IP，并基于此设计了该驱动。
