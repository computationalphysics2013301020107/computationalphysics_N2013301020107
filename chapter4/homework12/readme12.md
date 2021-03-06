#第十二次作业
- 刘祥干 2013301020107

##背景
- 众所周知,在太阳系中有一条小行星带,而且其距离太阳半径是木星到太阳距离的三分之一.按照行星分布在"整数比"处的经验规律来看,小行星带处很有可能以前有一颗行星,而后由于某种原因而碎成"小行星带".
- 本文从经典牛顿的万有引力定律出发,探究小行星带这个特殊位置是否是其形成的原因
- 由于木星质量较大,所以可能与木星有关.木星的带来的摄动可能在在这个特殊位置有着很强的影响,形成共振.而导致行星轨道大的变动,最后与某颗彗星相撞而碎成小行星带
- 由于历史原因,那些小行星空缺的地带被成为KirkWood gaps

##内容
- 由于太阳的质量太大,可以把木星和小行星视作在固定的引力场中运动,小行星和木星之间的受力有下述方程给出:
                                      ![公式1](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/%E5%85%AC%E5%BC%8F1.png)

- 结合牛顿第二定律,即可给出运动方程.用数值解法.即化为差分方程,用euler-comer方法进行求解.
- 当小行星的周期与木星周期比为1:2时.研究此处木星对小行星的影响[代码](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/12.1.py):
               ![](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/12.1.png)

- 上述只是一个试探,为了更加清楚的了解木星在多大距离上对小行星有明显影响,我们作出小行星运动的振幅和距离的共振曲线[代码2](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/12.2.py):
               ![](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/12.2.png)

-  可以明显看出在3.335左右共振非常明显
-  给出其他位置处的小行星运动:
                ![](https://github.com/computationalphysics2013301020107/computationalphysics_N2013301020107/blob/master/chapter4/homework12/12.3.png)


  
##结论
- 可以看出当近木星较远时,所受木星的摄动影响很小,而在近木点很近且位于共振峰附近时所受摄动影响会非常大
- 在1:2处或者3:4处小行星轨道都很稳定,说明此处受木星摄动影响较小.
- 在上述给出的6:7处,明显看出小行星的运动轨道不再稳定,由此可能带来一系列不稳定的因素,而使此处的行星不能"幸存"
- 利用此处给出的结论或许也同样适用于解释土星环的形成.或者其他有带状结构的行星系统.

##致谢
- 感谢王铮和陈洋遥给出的精彩范例.
- reference:课本
