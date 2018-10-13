优化算法有**梯度下降**和**牛顿法**

梯度下降分为**随机梯度下降**和**批梯度下降**，其中随机梯度下降适合小规模，而批梯度下降适合大规模

牛顿法相对于梯度下降的收敛速度要快很多，但是海森矩阵耗费时间和计算资源

**拟牛顿法**就是为了解决这个问题，其中有:**DFP**,**BFGS**,**L-BFGS**

DFP的核心是通过迭代对海森矩阵做近似

BFGS互换了DFP的sk，yk，性能更佳

L-BFGS通过不再在内存中存储矩阵，而是存向量，在需要时计算得到矩阵。
