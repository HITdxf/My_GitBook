最小方差控制：使控制系统的输出方差最小，以某种形式的二次型指标最优化为控制目的。但对于非最小相位系统的自校正控制，很难保证静态指标的最优，又有良好的鲁棒性。
改善策略：极点配置自校正技术，并不是以寻求某一目标函数最优为控制目的，而是对闭环系统的极点按工艺要求重新配置，可以获得设计时所需要的动态响应。
水床效应(the waterbed effect):
对于一个线性时不变(LTI)的SISO系统，其灵敏度传递函数如下所示，其中L(s)为系统的开环传递函数。

 

若闭环传递函数稳定，则由Bode's Intergral Theorem可知：

 

因此，若L(s)的阶数等于线上下或高于2阶，则
 
=0，这也意味着在0dB的区域面积相等。
怎么根据PES与ETF的频谱设计控制器？
首先根据PES分离出RRO与NRRO的频谱(spectrum)，根据RRO的频谱，利用水床效应设计ETF的频谱。把低频段扰动大的频率范围内抑制在0dB以内，扰动量小的抑制在0dB以上。PES的频谱为6。
RRO的来源：disk eccentricity, non-ideal servo track writing and spindle motor vibration.
NRRO的来源：torque disturbance, windage, non-repeatable disk motions and measurement noises.<Control Design>
Multi-Rate Digital Control：A system should use more than one sampling rate.