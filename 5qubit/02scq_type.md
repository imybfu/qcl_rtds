# 02scq_type

根据不同的自由度，超导量子比特主要分为:电荷（charge）、磁通（flux）和相位（phase）量子比特三类。三类量子比特的区别体现在约瑟夫森和电荷的能量比的大小。

1. 电荷量子比特也称为库珀对盒CPB（Cooper-pair box）量子比特，Ej/Ec<1，不同的能级对应于超导岛上的库珀对的数量。
2. 磁通量子比特的的基本结构是由一个电感与一个约瑟夫森结构造而成。EJ/Ec大约在10左右，磁场的能量占主导，能级对应于超导环路中不同数量的磁通量子。
3. 相位量子比特是电流偏置的单约瑟夫森结器件，EJ/Ec数量级在10^6，能级对应于穿过约瑟夫森结的不同量子电荷振荡振幅。

在以上三种超导量子比特原型的基础上，衍生出许多新形式的超导量子比特：如Transmon型量子比特、C型分流磁通量子比特、Fluxonium、Unimon、0-π量子比特、混合量子比特等。

4. Transmon全称是传输线分流等离子体振荡量子比特（ transmission line shunted plasma oscillation qubit），由耶鲁大学的 Robert J. Schoelkopf, Michel Devoret, Steven M. Girvin 等人于2007年基于电荷量子比特开发。通过在CPB的基础上额外并联一个对地的大电容分流，显著地提高了约瑟夫森和电荷的能量比，进而降低量子比特对电荷噪声的敏感性。在最初的设计中，这个额外的对地电容是通过叉指电容来实现的。

在Transmon的基础上进一步发展出了不同的版本，如Xmon、Gatemon、Gmon、3D Transmon等。

5. Xmon 通过一个十字型的结构来实现与地之间的额外电容（有些文章里会讲transmon没有共地面的连接）。这种结构的优点在于电容形状容易调节，使得比特与比特耦合方面更加容易。十字形的分压电容在实现相同电容值的时候，体积更小，有利于提高芯片集成度，而且它的形状非常适合需要密堆积qubit网格的表面代码体系结构。
6. Gatemon同样是一个transmon的可调版本，通过栅极来调节。Gmon基于Xmon量子比特，量子比特用一个结连接，其作为一个可调谐的电感来控制耦合强度，Gmon结构可以避免固定耦合产生的频率拥挤问题。
7. 3D Transmon的最大特点是用三维波导腔代替了平面传输线腔，优点包括：腔体具有更大的模式体积，对表面电介质损耗的敏感度更低；其次，该架构为量子比特提供了良好的可控电磁环境。因此，这种结构可以抑制量子比特退相干，同时保持与控制信号的充分耦合。然而，如果想建立基于三维Transmon的大规模设备，可扩展性将是主要困难。