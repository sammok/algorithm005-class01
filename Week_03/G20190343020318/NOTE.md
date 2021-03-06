#### 本周学会了 分治、回溯、DFS、BFS、贪心、二分查找 等知识

##### 分治
- 一个大问题是由若干字问题组成
- 核心思路是将一个大问题拆成若干子问题(子问题无法继续细化、拆分)，分别解决这些子问题，再将这些子问题的结果合并为一个大结果，最后得出的结果，就是大问题的结果

##### 回溯
- 回溯的核心是更改当前状态，带着当前状态不断的下浅到每一层去试，找到结果试完了再回到上一层，并且还原当前状态，再去试其他的可能性

[回溯知识参考文章](https://leetcode-cn.com/problems/permutations/solution/hui-su-suan-fa-xiang-jie-by-labuladong-2/)

#### 遍历树的节点
- 按照访问节点的顺序，我们将遍历方法分为 DFS 与 BFS 两种遍历方式
- 不管是 DFS BFS 都需要熟练超哥的代码模版，如果不理解可以在纸上画一下代码模版的运行步骤

##### DFS
- DFS (Depth First Search) 是搜索节点的方式之一

##### BFS
- BFS(Breadth First Search) 是搜索节点的方式之二，
- 特点是: 像水波纹一样从根节点一层一层向下遍历
- 利用这些特点可以应用在例如遍历树的层级上

##### 贪心算法
- 核心是: 每一步都选当前可选项中最优解，从而导致全局的结果是最优或最好
- 应用贪心算法需要对数据有一定的特殊性要求，否则贪心算法并不是最优解
- 如果当前问题可以使用贪心算法完成，那么贪心算法将是它的最优解
- 贪心法可以作为辅助算法，解决不需要特别精准的结果的问题

贪心算法: 对当下局部最优判断，
回溯: 能够回退
动态规划则是: 最优判断 + 会退

##### 二分查找 
- 二分查找在时间复杂度上一般是 O(logn) 它比 O(n) 效率要高许多
- 想使用二分查找的思路解决问题需要满足二分查找**三个前置条件**
	- 目标函数单调性(递增或递减) 意思就是 Input 必须是有序的
	- 存在上下边界(bounded) 否则无法找到答案
	- 能够通过索引访问数据 但单链表就不合适了(但可以优化为跳表 )
