# 初始配置

在开始开发PX4之前，系统应当以默认配置进行初始配置，以确保硬件已经正确配备和测试。下方视频讲解了 [Pixhawk硬件](../flight_controller/pixhawk.md)与[QGroundControl](../qgc/README.md)的安装过程。 [此链接](../airframes/architecture.md)为已支持的参考机架列表。

> **须知：** [下载DAILY BUILD版本的QGroundControl](http://qgroundcontrol.org/downloads)跟随下方的视屏教程来设置你的飞行器。参考[QGroundControl 教程](../3_Tutorial/ground_control_station.md)来了解任务规划，飞行和和参数设置的具体细节。

下面的视频介绍一系列的设置选项

{% raw %}
<video id="my-video" class="video-js" controls preload="auto" width="100%" 
poster="http://image84.360doc.com/DownloadImg/2015/04/1617/52474470_2.jpg" data-setup='{"aspectRatio":"16:9"}'>
  <source src="http://7xvob5.com1.z0.glb.clouddn.com/1-PX4%20Autopilot%20Setup%20Tutorial%20Preview.mp4" type='video/mp4' >
  <p class="vjs-no-js">

    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
</video>
{% endraw %}

## 遥控选项

PX4飞行控制栈并不强制要求有遥控系统。也不要求使用单独的开关来选择飞行模式。

### Flying without Radio Control

所有的遥控装置的检查可以通过设置参数`COM_RC_IN_MODE`为` 1 `禁用。这将不允许手动飞行，但是，除了比如flying in之类的飞行模式。

### 单通道模式切换开关

在这种模式下，系统将接受一个单一的通道作为模式开关，而不是使用多个开关，这在 [旧版wiki](https://pixhawk.org/peripherals/radio-control/opentx/single_channel_mode_switch)有解释。
