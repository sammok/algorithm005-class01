本周主要围绕动态规划学习
* 动态规划 和 递归 或者 分治 没有根本上的区别，关键看有无最优子结构
    * 共性 都是找到重复子问题
    * 差异性 动态规划每步都有最优子结构、中途可以淘汰次优解
* 动态规划可以 优化重复计算，利用缓存(Hash) 实现记忆化搜索(Memorization)
*  只要写递归，就直接写 for 循环来实现自底向上的递推 (竞赛选手做法)
    * 这也是 DP 的终极形态
*  复杂点的递归会是多维度的比如二维、三维数据 它中间会有所谓的取舍最优子结构
*  有时候结果要取累加、有时候结果要取最大或最小值
*  字符串定义为DP时，需要将字符串转换为数组来定义状态
*  定义状态的时候，数组注意不要越界
* DP可以自顶向下，也可以自底向上 递推公式困难的话，可以想一下自底向上的思路

超哥 DP 三步
* A. 找重复性(分治)
* B. 定义状态数组
* C. 推出 DP 方程

MIT DP 三步
* Define subproblems
* Guess(part of solution)
* Relate subproblem solutions
* Recurse & memorize
* Solve original problem 

小结
* 要打破自己的思维习惯，形成机械思维，也就是说思维要跟计算机一样，只会最简单的 loop、branch 所以要学会找重复性
* 理解复杂逻辑的关键点，定义状态数组，定义 DP 方程
* 不要人肉递归 
