# Purpose
In order to solving the interesting alogrithm problems which meeting at the interviews frequently by me and some interesting LeetCode problems.
You can click the title with blue url linking to the code, the original problems may be archived by the Coming from URL.

****

1.solved with python,folder named as **Leetcode? + details**

2.solved with java,folder named as **src/Solution? + details**

3.others solved,folder named as **random**
****

# interviews 
- [EggTopFloor](random/EggTopFloor.py)

**Tencent** - Machine learning Engineer
- [HuffmanEncoding](random/HuffmanEncoding.py)

**Didichuxing** -  Statistical Analyst
-  [SortAlgorithm](random/SortMethod.py)

Almost everytime such as **Alibaba、JD、Didichuxing**...
- [GapCount](random/GapCount.py)

**Hp(Hewlett-Packard)** - Model Engineer
- [无序数组排序（时间复杂度为O(n)）](random/无序数组排序（时间复杂度为O(n)）.py)

```
问题：给你n个无序的int整型数组arr，并且这些整数的取值范围都在0-20之间，要你在 O(n) 的时间复杂度中把这 n 个数按照从小到大的顺序打印出来。
```
- [最大公共字符串长度](random/最大公共字符串长度.py)

`有两个字符串，你只可以进行删除操作，问你最少进行多少次操作可以使两个字符串相等`

Coming from:`字节跳动面试题`

- [素数伴侣](random/素数伴侣.py)

**HuaWei** - Machine learning Engineer

```核心在于匈牙利算法```

>题目描述:
若两个正整数的和为素数，则这两个正整数称之为“素数伴侣”，如2和5、6和13，它们能应用于通信加密。现在密码学会请你设计一个程序，从已有的N（N为偶数）个正整数中挑选出若干对组成“素数伴侣”，挑选方案多种多样，例如有4个正整数：2，5，6，13，如果将5和6分为一组中只能得到一组“素数伴侣”，而将2和5、6和13编组将得到两组“素数伴侣”，能组成“素数伴侣”最多的方案称为“最佳方案”，当然密码学会希望你寻找出“最佳方案”。

- [Lru_Cache](random/Lru_Cache.py)

**360** - Deep learning Engineer

```Lru_Cache实现```

- [消消乐](random/消消乐.py)

**Tencent** - Deep learning Engineer

>有n个数字，每次可以选择任意两个不同的数字，并同时删除它们，请问最后是否可以删完

```
两个坑：
1.汇总每个数字出现的次数的时候，不要用.count()，会超时；遍历hashmap
2.汇总后的数组中的每个数字是可拆的，并不是把一个数组切分成n个和相等的子数组，只需要max_value<=sum/2即可
```

- [花匠摆花](random/花匠摆花.py)

**Tencent** - Deep learning Engineer

```
原题参考代码注释
```
```
两个坑：
1.用traceback的就直接gg，比如我
2.dp[i]为当前的长度为i的可摆放个数，dp[i] = dp[i-1]+dp[i-k]为状态转移矩阵，更多解释看代码注释
```

Coming from:http://codeforces.com/contest/474/problem/D

- [意图相似度](random/意图相似度.py)

**阿里** - Algorithm Engineer

>找出相似意图（编辑距离<阈值）的pair，且每一个意图要满足一定长要求条件`[minSeqLen,maxSeqLen]`，一个子序列可能存在多个重复的，比如如下就是满足长度`[5,8]`(编辑距离为1，小于阈值等于2)子意图序列pair：
```
>A:weather,joker,music,stock,joker,joker,news
>B:weather,joker,music,stock,joker,joker,texi
输入：
第一行：阈值
第二行：最小序列长度
第三行：最多序列长度
第四行：A用户的意图序列
第五行：B用户的意图序列
```

- [数组分组问题](random/数组分组问题.py)

**携程** - Deep learning Engineer

>给定一个时刻表，根据目的地进行分组，同一个目的地必须尽可能的多分，不能打乱顺序，比如aabbcddc，需要分成aa|bb|cddc,而不能分成aabb|cddc，因为这种情况下不是最多，也不能分成aa|bb|c|dd|c,因为相同的c没有被分在一起；求分组个数；

用了两种方法解，数组区间合并和动态规划

- [连乘质数和](random/连乘质数和.py)

**快手2020校招**

>给定一个(1,N]之间的正整数，需要统计质数分解之后的质数的个数；
>举例:N=6,(1,6]之间包括2,3,4,5,6,2=2,3=3,4=2*2,5=5,6=2*3,所以对应质数和位1+1+2+1+2=7

```我做的是最简单的实现，回溯求解```

- [binarySearchTree](random/binarySearchTree.py)

`搜索二叉树`

- [文本编辑距离](random/文本编辑距离.py)

- [01背包](random/01背包.py)

- [约瑟夫环问题](random/约瑟夫环问题.py)

约瑟夫环问题：一圈共有N个人，开始报数，报到M的人自杀，然后重新开始报数，问最后自杀的人是谁？
问题重述：N个人（编号0~(N-1))，从0开始报数，报到(M-1)的自杀，剩下的人继续从0开始报数。求最后自杀者的编号。

- [按递增间隔删数，直到最后只剩下一个数](random/递增间隔删数.py)

有数组A，每个元素存放相应的下标,即A[i]=i，要求按照1,2,3,...的规律删除数组中的元素,第一次间隔1个数，第二次间隔2个数,依次类推，到末尾时循环至开头继续进行,求最后一个被删掉的数的原始下标位置

以上两条都是属于环问题，更多讲解来自：[约瑟夫环问题整理](http://www.shataowei.com/2019/10/20/约瑟夫环问题整理/)

- [计数排序](random/计数排序.py)

**阿里-推荐算法工程师**

- [插入排序](random/插入排序.py)

- [希尔排序](random/希尔排序.py)

- [归并排序](random/归并排序.py)

- [堆排序](random/堆排序.py)

***

# array

- [two-sum](LeetCode/LeetCode1two-sum.py)

Coming from :https://leetcode-cn.com/problems/two-sum/

- [container-with-most-water](LeetCode/LeetCode11container-with-most-water.py)

Coming from:https://leetcode-cn.com/problems/container-with-most-water/

- [3Sum](src/Solution15.java)
`左右双指针,亮点在于定义了很多提前跳出条件，在相同值跳过的条件判断中用nums[i+1]还是nums[i-1]尤为灵活`

Coming from:https://leetcode-cn.com/problems/3sum/

- [3Sum Closest](src/Solution16.java)
`这题和上面一题很类似，只是最好不要在多生产变量了，直接拿num[first]+num[last]+num[i]去和target比，而不要考虑差值是否大于0，很容易绕进去`

Coming from:https://leetcode-cn.com/problems/3sum-closest/

- [4Sum](src/Solution18.java)

Coming from:https://leetcode-cn.com/problems/4sum/

- [Remove Duplicates from Sorted Array](src/Solution26.java)

Coming from:https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array/

- [Remove Element](src/Solution27.java)

Coming from:https://leetcode-cn.com/problems/remove-element/

- [search-in-rotated-sorted-array](LeetCode/LeetCode33search-in-rotated-sorted-array.py)

```
因为是螺旋数组，所以理解2点：
1、对于mid = （left+right）>>1来说，要么左侧要么右侧，必然会有一边是有序的
2、判断target在有序侧还是非有序侧，从而决定是修正有序侧还是简单位移
```

ps:二分用的是index:`while end<=right`

Coming from:https://leetcode-cn.com/problems/search-in-rotated-sorted-array/

- [find-first-and-last-position-of-element-in-sorted-array](LeetCode/LeetCode34find-first-and-last-position-of-element-in-sorted-array.py)

这个考的是二分法中的while跳出条件和left、right变化逻辑，本题是找出左右边界

Coming from:https://leetcode-cn.com/problems/find-first-and-last-position-of-element-in-sorted-array/

- [Search Insert Position](src/Solution35.java)

Coming from:https://leetcode-cn.com/problems/search-insert-position/

- [combination-sum](src/Solution39.java)
`这题和上面这题很像，递归在for循环里面的回溯算法，把所有情况跑一遍`

`画重点，求解过程中存着result 是List<List<Integer>>的，而tmp_list是list的,需要把tmp_list再裹一层new ArrayList<>(tmp_list)再进行add`

Coming from:https://leetcode-cn.com/problems/combination-sum/

- [trapping-rain-water](LeetCode/LeetCode42trapping-rain-water.py)

动态规划和栈的两种方法，很值得看一下

Coming from:https://leetcode-cn.com/problems/trapping-rain-water/

- [rotate-image](LeetCode/LeetCode48rotate-image.py)

Coming from:https://leetcode-cn.com/problems/rotate-image/

- [jump-game](LeetCode/LeetCode55jump-game.py)

```python
max_dis：上次每次可跳的最远距离
本次是在range中产生的，所以需要减去1，剩下的才是还可供跳跃的长度

nums[idx]：是本次新可跳的距离

比较max_ids-1和nums[idx]得出当前可跳的新最远距离
如果max_ids==0代表可跳的距离额度没有了，return False
```

这题和[distribute-coins-in-binary-tree](LeetCode/LeetCode979distribute-coins-in-binary-tree.py)神似。

Coming from:https://leetcode-cn.com/problems/jump-game/

- [MergeIntervals](LeetCode/LeetCode56MergeIntervals.py)

Coming from:https://leetcode-cn.com/problems/merge-intervals/

- [SpiralMatrixII](LeetCode/LeetCode59SpiralMatrixII.py)
`旋转矩阵题型，用了余数判断位置，比较亮点`

Coming from:https://leetcode-cn.com/problems/spiral-matrix-ii/


Coming from:https://leetcode-cn.com/problems/unique-paths-ii/



- [sort-colors](LeetCode/LeetCode75sort-colors.py)

Coming from:https://leetcode-cn.com/problems/sort-colors/

- [Subsets](LeetCode/LeetCode78Subsets.py)

`这题利用了python的语言机制，很有意思`

Coming from :https://leetcode.com/problems/subsets/

- [word-search](LeetCode/LeetCode79word-search.py)

Coming from:https://leetcode-cn.com/problems/word-search/

- [largest-rectangle-in-histogram](src/Solution84.java)

Coming from:https://leetcode-cn.com/problems/largest-rectangle-in-histogram/

- [merge-sorted-array](LeetCode/LeetCode88merge-sorted-array.py)
- [merge-sorted-array](src/Solution88.java)

Coming from:https://leetcode-cn.com/problems/merge-sorted-array/

- [majority-element](LeetCode/LeetCode169majority-element.py)

Coming from:https://leetcode-cn.com/problems/majority-element/

- [product-of-array-except-self](LeetCode/LeetCode238product-of-array-except-self.py)

`两侧分别扫描一遍`

Coming from:https://leetcode-cn.com/problems/product-of-array-except-self/

- [move-zeroes](LeetCode/LeetCode283move-zeroes.py)

Coming from:https://leetcode-cn.com/problems/move-zeroes/

- [find-the-duplicate-number](LeetCode/LeetCode287find-the-duplicate-number.py)

```
（1）使用哈希表判重
（2）排序以后，重复的数相邻
（3）使用“抽屉原理”，当两个数发现要放在同一个地方的时候，就发现了这个重复的元素
（4）既然要定位数，可以对“数”做二分
（5）还可以使用“快慢指针”来完成
```

环概念：代码内部，好好看

Coming from:https://leetcode-cn.com/problems/find-the-duplicate-number/

- [find-all-duplicates-in-an-array](LeetCode/LeetCode442find-all-duplicates-in-an-array.py)
```和上面一样，核心是每次对abs(nums[idx])-1的处理获得nums的index很有意思```

Coming from:https://leetcode-cn.com/problems/find-all-duplicates-in-an-array/

- [find-all-numbers-disappeared-in-an-array](LeetCode/LeetCode448find-all-numbers-disappeared-in-an-array.py)
```nums[abs(nums[idx]) - 1] = -abs(nums[abs(nums[idx]) - 1]),两个abs保证了所有存在的idx都被置负了```

Coming from:https://leetcode-cn.com/problems/find-all-numbers-disappeared-in-an-array/

- [teemo-attacking](src/Solution495.java)

Coming from:https://leetcode-cn.com/problems/teemo-attacking/

- [SubarraySumEqualsK](LeetCode/LeetCode560SubarraySumEqualsK.py)

Coming from:https://leetcode-cn.com/problems/subarray-sum-equals-k/

- [shortest-unsorted-continuous-subarray](LeetCode/LeetCode581shortest-unsorted-continuous-subarray.py)

Coming from:https://leetcode-cn.com/problems/shortest-unsorted-continuous-subarray/

- [can-place-flowers](src/Solution605.java)

Coming from:https://leetcode-cn.com/problems/can-place-flowers/

- [valid-triangle-number](LeetCode/LeetCode611valid-triangle-number.py)
- [valid-triangle-number](src/Solution611.java)

Coming from:https://leetcode-cn.com/problems/valid-triangle-number/

- [task-scheduler](LeetCode/LeetCode621task-scheduler.py)

理解一下，出现次数最多的那个字母（出现次数-1）x时间窗口及为最小次数，剩余要考虑的是都为最多次数的字母数

Coming from:https://leetcode-cn.com/problems/task-scheduler/

- [maximum-average-subarray-i](src/Solution643.java)

Coming from:https://leetcode-cn.com/problems/maximum-average-subarray-i/

- [largest-number-at-least-twice-of-others](src/Solution747.java)

Coming from:https://leetcode-cn.com/problems/largest-number-at-least-twice-of-others/

- [transpose-matrix](LeetCode/LeetCode867transpose-matrix.py)

Coming from:https://leetcode-cn.com/problems/transpose-matrix/

- [AdvantageShuffle](LeetCode/LeetCode870AdvantageShuffle.py)
`这道题的难点在于耗时，贪心算法即可，田忌赛马，可以看下`

Coming from:https://leetcode-cn.com/problems/advantage-shuffle/

- [sort-array-by-parity-ii](src/Solution922.java)

Coming from:https://leetcode-cn.com/problems/sort-array-by-parity-ii/

- [squares-of-a-sorted-array](src/Solution977.java)

Coming from:https://leetcode-cn.com/problems/squares-of-a-sorted-array/

- [add-to-array-form-of-integer](src/Solution989.java)

Coming from:https://leetcode-cn.com/problems/add-to-array-form-of-integer/

- [binary-prefix-divisible-by-5](src/Solution1018.java)

Coming from:https://leetcode-cn.com/problems/binary-prefix-divisible-by-5/

- [HeightChecker](LeetCode/LeetCode1051HeightChecker.py)

Coming from:https://leetcode-cn.com/problems/height-checker/

***

# dynamic programming

- [longest-palindromic-substring](LeetCode/LeetCode5longest-palindromic-substring.py)

>中心展开，从中间值往两边展开，判断展开终止点的长度

Coming from:https://leetcode-cn.com/problems/longest-palindromic-substring/

- [maximum-subarray](LeetCode/LeetCode53maximum-subarray.py)

```简单递归```

Coming from:https://leetcode-cn.com/problems/maximum-subarray/

- [unique-paths](LeetCode/LeetCode62unique-paths.py)

Coming from:https://leetcode-cn.com/problems/unique-paths/

- [unique-paths-ii](LeetCode/LeetCode63unique-paths-ii.py)
- [unique-paths-ii](src/Solution63.java)
```最优路径下的dp```

- [minimum-path-sum](LeetCode/LeetCode64minimum-path-sum.py)
`非常基础简单的动态规划问题，适合理解动态规范的想法`

Coming from:https://leetcode-cn.com/problems/minimum-path-sum/

- [maximal-rectangle](src/Solution85.java)

Coming from:https://leetcode-cn.com/problems/maximal-rectangle/ 

- [decode-ways](LeetCode/LeetCode91decode-ways.py)
```状态转移方程式dp[i] = dp[i-1]+dp[i-2],复杂在什么时候加前项什么时候加后项，什么时候加两项，0的位置的考虑```

Coming from:https://leetcode-cn.com/problems/decode-ways/

- [triangle](LeetCode/LeetCode120triangle.py)

Coming from:https://leetcode-cn.com/problems/triangle/

- [best-time-to-buy-and-sell-stock](LeetCode/LeetCode121best-time-to-buy-and-sell-stock.py)
- [best-time-to-buy-and-sell-stock](src/Solution121.java)

Coming from:https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock/

- [best-time-to-buy-and-sell-stock-ii](LeetCode/LeetCode122best-time-to-buy-and-sell-stock-ii.py)
- [best-time-to-buy-and-sell-stock-ii](src/Solution122.java)

Coming from:https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/

- [word-break](LeetCode/LeetCode139word-break.py)

>第一轮用的traceback，时间复杂度是n的n次方，扑gai；然后我想了下，既然可以考虑回溯，为什么不能递归，其实只要把方程：flag[j] = flag[i]+s[i:j] in wordDict 这个想到就行，这个算是是像加限制性条件的dp，比如20届拼多多校招，多多鸡砍树问题

Coming from:https://leetcode-cn.com/problems/word-break/

- [maximum-product-subarray](LeetCode/LeetCode152maximum-product-subarray.py)

```需要存一个max和min，来做条件判断```

Coming from:https://leetcode-cn.com/problems/maximum-product-subarray/

- [dungeon-game](LeetCode/LeetCode174dungeon-game.py)

```反向递归```

Coming from:https://leetcode-cn.com/problems/dungeon-game/

- [house-robber](LeetCode/LeetCode198house-robber.py)
`dp算法很经典的一道题`

Coming from:https://leetcode-cn.com/problems/house-robber/

- [maximal-square](LeetCode/LeetCode221maximal-square.py)

Coming from:https://leetcode-cn.com/problems/maximal-square/

- [Ugly Number II](src/Solution264.java)

Coming from:https://leetcode-cn.com/problems/ugly-number-ii/

- [perfect-squares](src/Solution279.java)
- [perfect-squares](LeetCode/LeetCode279perfect-squares.py)


```双循环的dp，同样的思路python会超时，Java不会```

Coming from:https://leetcode-cn.com/problems/perfect-squares/

- [longest-increasing-subsequence](LeetCode/LeetCode300longest-increasing-subsequence.py)
- [longest-increasing-subsequence](src/Solution300.java)
```
dp和递归理解的好题目，值得看
```
Coming from:https://leetcode-cn.com/problems/longest-increasing-subsequence/

- [range-sum-query-immutable](LeetCode/LeetCode303range-sum-query-immutable.py)

Coming from:https://leetcode-cn.com/problems/range-sum-query-immutable/

- [best-time-to-buy-and-sell-stock-with-cooldown](LeetCode/LeetCode309best-time-to-buy-and-sell-stock-with-cooldown.py)

`dp的高难题，代码中带完整带解题方法`

Coming from:https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/

- [burst-balloons](LeetCode/LeetCode312burst-balloons.py)

`dp的超高难题，代码中带完整带解题方法`

Coming from:https://leetcode-cn.com/problems/burst-balloons/

- [coin-change](LeetCode/LeetCode322coin-change.py)

斐波纳切动态规划

Coming from:https://leetcode-cn.com/problems/coin-change/

- [counting-bits](src/Solution338.java)

Coming from:https://leetcode-cn.com/problems/counting-bits/

- [split-array-largest-sum](LeetCode410split-array-largest-sum.py)

Coming from:https://leetcode-cn.com/problems/split-array-largest-sum/

- [partition-equal-subset-sum](LeetCode/LeetCode416partition-equal-subset-sum.py)

`01背包问题，这题主要考虑提前跳出条件`

Coming from:https://leetcode-cn.com/problems/partition-equal-subset-sum/

- [target-sum](LeetCode/LeetCode494target-sum.py)

```这题有点难，01背包+递归逻辑，值得面试前看一波```

```
难点1：把原问题转换为算背包容积的问题，因为p-n=t,p-n+p+n=sum+t,p=(sum+t)/2
难点2：dp[i]=dp[i]+dp[i-num]
```

Coming from:https://leetcode-cn.com/problems/target-sum/

- [palindromic-substrings](LeetCode/LeetCode647palindromic-substrings.py)

```回文子串问题```

```
方法1：dp
方法2：中间搜索
```

Coming from:https://leetcode-cn.com/problems/palindromic-substrings/

- [Partition to K Equal Sum Subsets](src/Solution698.java)
`依旧是递归，区别在递归逻辑在for循环中，相当于并发了n条处理逻辑，有点像树展开`

Coming from:https://leetcode-cn.com/problems/partition-to-k-equal-sum-subsets/

- [delete-and-earn](LeetCode/LeetCode740delete-and-earn.py)
`核心在于bitmap+dp，与198题类似`

Coming from:https://leetcode-cn.com/problems/delete-and-earn/

- [valid-permutations-for-di-sequence](LeetCode/LeetCode903valid-permutations-for-di-sequence.py)

`爱奇艺2020届校招`

>这边需要明白一个规则，举个例子：S:[0,1,2,3],P:[DID];dp[i,j]中i指S中的最大范围，此处i最大=3，j为以什么为结尾
dp[2.1]则为S:[0,1,2],且以1为结尾，因为p为DID，所以当i=2的时候，应该满足DI，1为结尾，又因为I为此时P的结尾，所以
[0,1]的前两位组合的末尾应该是比二小就行，所以d[1,1]和dp[1,0]都行，dp[2,2] = dp[1,0]+dp[1,1]=1+0；如果是ID的情况
同上，所以状态转移方程应该是：
if S[i-1] == "D":dp[i,j] += dp[i-1,k] j<=k<=i-1
if S[i-1] == "I":dp[i,j] += dp[i-1,k] k<j

Coming from:https://leetcode-cn.com/problems/valid-permutations-for-di-sequence/

- [VideoStitching](LeetCode/LeetCode1024VideoStitching.py)
`贪心算法概念的比较好理解的一道题`

Coming from:https://leetcode-cn.com/problems/video-stitching/

- [n-th-tribonacci-number](src/Solution1137.java)
```最简单的dp```

Coming from:https://leetcode-cn.com/problems/n-th-tribonacci-number/

*** 

# binary-tree

- [binary-tree-inorder-traversal](LeetCode/LeetCode94binary-tree-inorder-traversal.py)

`二叉树中序遍历`

三种写法：
1、好理解的递归
2、qsort递归写法
3、利用栈性质的迭代写法

Coming from:https://leetcode-cn.com/problems/binary-tree-inorder-traversal/

- [binary-tree-level-order-traversal](LeetCode/LeetCode102binary-tree-level-order-traversal.py)

`二叉树层序遍历，利用了队列先进先出的性质`

Coming from:https://leetcode-cn.com/problems/binary-tree-level-order-traversal/

- [maximum-depth-of-binary-tree](LeetCode/LeetCode104maximum-depth-of-binary-tree.py)

`二叉树深度计算，利用了递归性质`

Coming from:https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/

- [merge-two-binary-trees](LeetCode/LeetCode617merge-two-binary-trees.py)

`二叉树合并，利用了递归性质`

Coming from:https://leetcode-cn.com/problems/merge-two-binary-trees/



- [diameter-of-binary-tree](LeetCode/LeetCode543diameter-of-binary-tree.py)

`结点之间的最大距离，和104题的深度一样`

比较坑的点：只有一个结点的时候，该题认为点重合，距离为0
做题思路就是：遍历所有结点，保存所有结点作为根结点的情况下，左右子树的最大深度和即可

Coming from:https://leetcode-cn.com/problems/diameter-of-binary-tree/

- [convert-bst-to-greater-tree](LeetCode/LeetCode538convert-bst-to-greater-tree.py)

`先遍历右子树的中序遍历，面试之前一定要看，易于理解递归在二叉树中的应用`

```
1、先遍历到右树的根树，然后把根树的value赋值给add
2、更新此树对应的父结点，并更新父结点对应的value = value+add
3、同时再更新add，把父结点的值也更新到add上
4、再更新父结点的左子树的value结点
5、这样一次更新便完成了
```
Coming from:https://leetcode-cn.com/problems/convert-bst-to-greater-tree/

- [invert-binary-tree](LeetCode/LeetCode226invert-binary-tree.py)

`反转树，相互对称`

Coming from:https://leetcode-cn.com/problems/invert-binary-tree/

- [implement-trie-prefix-tree](LeetCode/LeetCode208implement-trie-prefix-tree.py)

`tire 字典实现`

Coming from:https://leetcode-cn.com/problems/implement-trie-prefix-tree/

- [construct-binary-tree-from-preorder-and-inorder-traversal](LeetCode/LeetCode105construct-binary-tree-from-preorder-and-inorder-traversal.py)

`360面试题，真有意思`

需要注意的点：
1. preOrderTraver中的第一个元素必然是根结点，第二个元素开始为左右子树结点
2. inOrderTraver中的找到preOrderTraver中的第一个元素的位置中左侧必然是左子树，右侧必然是右子树
3. **2中找到的左子树长度其实就是list中切点index，且左子树不论在preOrderTraver还是在inOrderTraver中长度必然一致**
4. **preOrderTraver是先遍历左子树再遍历右子树的，所以preOrderTraver[1:3中的长度+1]即为左子树下次递归中的preOrderTraver**

Coming from:https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/

- [serialize-and-deserialize-binary-tree](LeetCode/LeetCode297serialize-and-deserialize-binary-tree.py)

`二叉树-->list//list-->二叉树`

```
        tmp = data.pop(0)
        if tmp == "null":
            return None
        root = TreeNode(int(tmp))
```
这三行很重要，`data.pop`不断的拿结点去赋值，`if`判断条件用来当数据到最底层时候，跳出此次递归分支，切换到另一个子树上（此处为右子树）

Coming from:https://leetcode-cn.com/problems/serialize-and-deserialize-binary-tree/

- [lowest-common-ancestor-of-a-binary-tree](LeetCode/LeetCode236lowest-common-ancestor-of-a-binary-tree.py)

`left if right is None else right if left is None else root`
这行代码的背后：
1、left 来自于左子树查找p,q的结果，如果查到了返回对应，没有的话返回None
2、right 来自于右子树查找p,q的结果，如果查到了返回对应，没有的话返回None
3、如果分别来自左右子树，意味着left和right都不为None，则返回改root，即为最近的父结点
4、一旦查到，剩下的搜索结果都会为None，又回到了1，2两种情况

Coming from:https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/

- [lowest-common-ancestor-of-a-binary-search-tree](LeetCode/LeetCode235lowest-common-ancestor-of-a-binary-search-tree.py)

`和上面一题一摸一样`

Coming from:https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-search-tree/

- [unique-binary-search-trees](LeetCode/LeetCode96unique-binary-search-trees.py)

`动态规划`

Coming from:https://leetcode-cn.com/problems/unique-binary-search-trees/

- [symmetric-tree](LeetCode/LeetCode101symmetric-tree.py)

`层次遍历`

Coming from:https://leetcode-cn.com/problems/symmetric-tree/

- [validate-binary-search-tree](LeetCode/LeetCode98validate-binary-search-tree.py)

`搜索二叉树的左支<结点<右支，正好可以用中序遍历比较`

```
BST两个特点
1、左支<结点<右支
2、无重复
```

Coming from:https://leetcode-cn.com/problems/validate-binary-search-tree/

- [binary-tree-maximum-path-sum](LeetCode/LeetCode124binary-tree-maximum-path-sum.py)

`类似104题、543题这种递归的方式`

Coming from:https://leetcode-cn.com/problems/binary-tree-maximum-path-sum/

- [path-sum-iii](LeetCode/LeetCode437path-sum-iii.py)

`dfs+两数之和`


>这题leetcode认为是简单，但是我觉得贼难：
1、python闭包的理解，count虽然是局部遍历，但是在递归的时候，每个count都是独立的
2、dfs(root.？？？？？, sum - root.val)用的是两数之和的逻辑进行递归
3、dfs(root,sum) + self.pathSum(root.left, sum) + self.pathSum(root.right, sum)
这个用的是遍历所有结点的方法

换句话说，这题解法是函数用递归实现，函数体是另外一个递归真的有点恶心

Coming from:https://leetcode-cn.com/problems/path-sum-iii/

- [unique-binary-search-trees-ii](LeetCode/LeetCode95unique-binary-search-trees-ii.py)

和[unique-binary-search-trees](LeetCode/LeetCode96unique-binary-search-trees.py)这题思路一样
不同的是，unique-binary-search-trees用的是dp，本题用的是递归，核心和之前一样，\[start,i]作为左树去递归，node(i)作为根，\[i+1,end]作为右树去递归

Coming from:https://leetcode-cn.com/problems/unique-binary-search-trees-ii/

- [same-tree](LeetCode/LeetCode100same-tree.py)

`层序遍历改写`

Coming from:https://leetcode-cn.com/problems/same-tree/

- [binary-tree-zigzag-level-order-traversal](LeetCode/LeetCode103binary-tree-zigzag-level-order-traversal.py)

`层序遍历改写`

Coming from:https://leetcode-cn.com/problems/binary-tree-zigzag-level-order-traversal/

- [recover-binary-search-tree](LeetCode/LeetCode99recover-binary-search-tree.py)

**BST+中序遍历的结果是有序的**,`self.ans.append(root)`直接加结点，而非加值了

Coming from:https://leetcode-cn.com/problems/recover-binary-search-tree/

- [house-robber-iii](LeetCode/LeetCode337house-robber-iii.py)

**基于树结构+动态规划**，可谓是花哨到极点了，最厉害的在于:
```
1、在每个结点上构造了一个[a,b]，其中[a,b],a为不考虑root.val下的max值，b为考虑当前root.val下的最大值
2、max(left)+max(right)涵盖了不考虑当前结点下的left+right最优解，其很好的控制了跳层相加的逻辑
```


Coming from:https://leetcode-cn.com/problems/house-robber-iii/

- [construct-binary-tree-from-inorder-and-postorder-traversal](LeetCode/LeetCode106construct-binary-tree-from-inorder-and-postorder-traversal.py)

和[construct-binary-tree-from-preorder-and-inorder-traversal](LeetCode/LeetCode105construct-binary-tree-from-preorder-and-inorder-traversal.py)类似

Coming from:https://leetcode-cn.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal/

- [construct-binary-tree-from-preorder-and-postorder-traversal](LeetCode/LeetCode889construct-binary-tree-from-preorder-and-postorder-traversal.py)

和[construct-binary-tree-from-preorder-and-inorder-traversal](LeetCode/LeetCode105construct-binary-tree-from-preorder-and-inorder-traversal.py)类似

Coming from:https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-postorder-traversal/

- [binary-tree-level-order-traversal-ii](LeetCode/LeetCode107binary-tree-level-order-traversal-ii.py)

层次遍历翻版

Coming from:https://leetcode-cn.com/problems/binary-tree-level-order-traversal-ii/

- [convert-sorted-array-to-binary-search-tree](LeetCode/LeetCode108convert-sorted-array-to-binary-search-tree.py)

有序数组-->平衡二叉树：二分查找+递归

Coming from:https://leetcode-cn.com/problems/convert-sorted-array-to-binary-search-tree/

- [balanced-binary-tree](LeetCode/LeetCode110balanced-binary-tree.py)

判断是否为平衡二叉树，利用的是dfs+[maximum-depth-of-binary-tree](LeetCode/LeetCode104maximum-depth-of-binary-tree.py)二叉树深度计算的方法

Coming from:https://leetcode-cn.com/problems/balanced-binary-tree/

- [minimum-depth-of-binary-tree](LeetCode/LeetCode111minimum-depth-of-binary-tree.py)

Coming from:https://leetcode-cn.com/problems/minimum-depth-of-binary-tree/

- [path-sum](LeetCode/LeetCode112path-sum.py)

Coming from:https://leetcode-cn.com/problems/path-sum/

上面这两题在return的时候都做了是否是根结点的判断:`left if root.right is None else right if root.left is None else left or right`

- [path-sum-ii](LeetCode/LeetCode113path-sum-ii.py)

dfs

Coming from:https://leetcode-cn.com/problems/path-sum-ii/

- [flatten-binary-tree-to-linked-list](LeetCode/LeetCode114flatten-binary-tree-to-linked-list.py)

`有点技巧性`

Coming from:https://leetcode-cn.com/problems/flatten-binary-tree-to-linked-list/

- [populating-next-right-pointers-in-each-node](LeetCode/LeetCode116populating-next-right-pointers-in-each-node.py)

`跨结点直接的指向关系由root.next is not None产生`

Coming from:https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node/

- [populating-next-right-pointers-in-each-node-ii](LeetCode/LeetCode117populating-next-right-pointers-in-each-node-ii.py)

`与上一次递归不同，这一次因为不知道root对应的下一层是否有空结点，所以针对上一层的判断结果进行迭代`

Coming from:https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node-ii/

- [sum-root-to-leaf-numbers](LeetCode/LeetCode129sum-root-to-leaf-numbers.py)

`dfs`

Coming from:https://leetcode-cn.com/problems/sum-root-to-leaf-numbers/

- [binary-tree-preorder-traversal](LeetCode/LeetCode144binary-tree-preorder-traversal.py)

`前序遍历迭代版，技巧就是queue进栈的策略是先右后左，因为前序遍历是中左右，进栈越早出栈越晚`

Coming from:https://leetcode-cn.com/problems/binary-tree-preorder-traversal/

- [binary-tree-postorder-traversal](LeetCode/LeetCode145binary-tree-postorder-traversal.py)

`巧妙的解法：宽度搜索+逆序出栈==后序输出`。另外，这份代码在`node = queue.pop()`-->`node = queue.pop(0)`,加个0就是层序遍历

Coming from:https://leetcode-cn.com/problems/binary-tree-postorder-traversal/

>以上两题加[binary-tree-inorder-traversal](LeetCode/LeetCode94binary-tree-inorder-traversal.py)都是迭代的解法，前序中序写的比较中规中矩，后序写的真的是惊艳

- [binary-tree-right-side-view](LeetCode/LeetCode199binary-tree-right-side-view.py)

`层序遍历`

Coming from:https://leetcode-cn.com/problems/binary-tree-right-side-view/

- [add-and-search-word-data-structure-design](LeetCode/LeetCode211add-and-search-word-data-structure-design.py)

`Tire树很经典的一道题`

Coming from :https://leetcode-cn.com/problems/add-and-search-word-data-structure-design/

- [count-complete-tree-nodes](LeetCode/LeetCode222count-complete-tree-nodes.py)

Coming from:https://leetcode-cn.com/problems/count-complete-tree-nodes/

- [kth-smallest-element-in-a-bst](LeetCode/LeetCode230kth-smallest-element-in-a-bst.py)

Coming from:https://leetcode-cn.com/problems/kth-smallest-element-in-a-bst/

- [binary-search-tree-iterator](LeetCode/LeetCode173binary-search-tree-iterator.py)

`借鉴了上一题中的generation的写法，我觉得非常适合业务中真实使用`

```python
def search(root):
    if not root:
        return
    for i in search(root.left):
        yield i

    yield root.val

    for i in search(root.right):
        yield i
```

Coming from:https://leetcode-cn.com/problems/binary-search-tree-iterator/

- [binary-tree-paths](LeetCode/LeetCode257binary-tree-paths.py)

`dfs`

Coming from:https://leetcode-cn.com/problems/binary-tree-paths/

- [sum-of-left-leaves](LeetCode/LeetCode404sum-of-left-leaves.py)

`限制性条件下的二叉树遍历计算查找，迭代要比计算更加高效`

Coming from:https://leetcode-cn.com/problems/sum-of-left-leaves/    

- [serialize-and-deserialize-bst](LeetCode/LeetCode449serialize-and-deserialize-bst.py)

`前序遍历保存，二叉搜索树的中序遍历为升序列，两则可以恢复原树`

Coming from:https://leetcode-cn.com/problems/serialize-and-deserialize-bst/    

- [delete-node-in-a-bst](LeetCode/LeetCode450delete-node-in-a-bst.py)

`看子节点的是否为None，分情况讨论`

Coming from:https://leetcode-cn.com/problems/delete-node-in-a-bst/    

- [find-mode-in-binary-search-tree](LeetCode/LeetCode501find-mode-in-binary-search-tree.py)

`直接遍历统计`

Coming from:https://leetcode-cn.com/problems/find-mode-in-binary-search-tree/    

- [find-bottom-left-tree-value](LeetCode/LeetCode513find-bottom-left-tree-value.py)

Coming from:https://leetcode-cn.com/problems/find-bottom-left-tree-value/    

- [find-largest-value-in-each-tree-row](LeetCode/LeetCode515find-largest-value-in-each-tree-row.py)

Coming from:https://leetcode-cn.com/problems/find-largest-value-in-each-tree-row/    

- [minimum-absolute-difference-in-bst](LeetCode/LeetCode530minimum-absolute-difference-in-bst.py)

Coming from:https://leetcode-cn.com/problems/minimum-absolute-difference-in-bst/    

- [binary-tree-tilt](LeetCode/LeetCode563binary-tree-tilt.py)

Coming from:https://leetcode-cn.com/problems/binary-tree-tilt/    

- [subtree-of-another-tree](LeetCode/LeetCode572subtree-of-another-tree.py)

`递归求解，好题目`

Coming from:https://leetcode-cn.com/problems/subtree-of-another-tree/    

- [most-frequent-subtree-sum](LeetCode/LeetCode508most-frequent-subtree-sum.py)

和[binary-tree-tilt](LeetCode/LeetCode563binary-tree-tilt.py)一样，计算每个结点的子树之和。

Coming from:https://leetcode-cn.com/problems/most-frequent-subtree-sum/    

- [add-one-row-to-tree](LeetCode/LeetCode623add-one-row-to-tree.py)

`递归直接修改树的实现，爬楼梯的翻版`

Coming from:https://leetcode-cn.com/problems/add-one-row-to-tree/    

- [average-of-levels-in-binary-tree](LeetCode/LeetCode637average-of-levels-in-binary-tree.py)

Coming from:https://leetcode-cn.com/problems/average-of-levels-in-binary-tree/    

- [find-duplicate-subtrees](LeetCode/LeetCode652find-duplicate-subtrees.py)

```python
out+=[root.val] +self.findDuplicateSubtrees(root.left)+self.findDuplicateSubtrees(root.right)
'''等价于'''
out+=[root.val]
out+=self.findDuplicateSubtrees(root.left)
out+=self.findDuplicateSubtrees(root.right)
````

```python
'''尾结点的填充'''
if not root:
    return "null"
```

Coming from:https://leetcode-cn.com/problems/find-duplicate-subtrees/    

- [two-sum-iv-input-is-a-bst](LeetCode/LeetCode653two-sum-iv-input-is-a-bst.py)

Coming from:https://leetcode-cn.com/problems/two-sum-iv-input-is-a-bst/    

- [maximum-binary-tree](LeetCode/LeetCode654maximum-binary-tree.py)

Coming from:https://leetcode-cn.com/problems/maximum-binary-tree/

- [n-ary-tree-level-order-traversal](LeetCode/LeetCode429n-ary-tree-level-order-traversal.py)

Coming from:https://leetcode-cn.com/problems/n-ary-tree-level-order-traversal/

- [maximum-depth-of-n-ary-tree](LeetCode/LeetCode559maximum-depth-of-n-ary-tree.py)

Coming from:https://leetcode-cn.com/problems/maximum-depth-of-n-ary-tree/

- [maximum-width-of-binary-tree](LeetCode/LeetCode662maximum-width-of-binary-tree.py)

Coming from:https://leetcode-cn.com/problems/maximum-width-of-binary-tree/

- [trim-a-binary-search-tree](LeetCode/LeetCode669trim-a-binary-search-tree.py)

```python
class Solution(object):
    def trimBST(self, root, L, R):
        """
        :type root: TreeNode
        :type L: int
        :type R: int
        :rtype: TreeNode
        """
        if not root:
            return None
        '''计算逻辑'''
        return root
```

以上是结点变更的写法，如果接一个`root = self.trimBST`相当于对结点做一个覆盖，也就是直接修改树

Coming from:https://leetcode-cn.com/problems/trim-a-binary-search-tree/

- [second-minimum-node-in-a-binary-tree](LeetCode/LeetCode671second-minimum-node-in-a-binary-tree.py)

log(h)的跳出条件的递归写法

Coming from:https://leetcode-cn.com/problems/second-minimum-node-in-a-binary-tree/

- [longest-univalue-path](LeetCode/LeetCode687longest-univalue-path.py)

```逻辑理解的递归```

1.基于跳出条件，先递归到终止条件前
```
if not root:
    return 0
left = helper(root.left)
right = helper(root.right)
```
2.初始化终止条件的初始值

```lefts = 0,rights=0 ```

3.基于初始值进行逻辑计算，如果需要保存中间变量需要在__init__函数中记录
```
if root.left and root.val == root.left.val:
    lefts = lefth + 1
if root.right and root.val == root.right.val:
    rights = righth + 1
self.ans = max(self.ans,lefts+rights)
```
4.返回一次子任务执行的结果，通常需要处理

`return max(lefts,rights)`

Coming from:https://leetcode-cn.com/problems/longest-univalue-path/  

- [n-ary-tree-preorder-traversal](LeetCode/LeetCode589n-ary-tree-preorder-traversal.py)

Coming from:https://leetcode-cn.com/problems/n-ary-tree-preorder-traversal/

- [n-ary-tree-postorder-traversal](LeetCode/LeetCode590n-ary-tree-postorder-traversal.py)

Coming from:https://leetcode-cn.com/problems/n-ary-tree-postorder-traversal/

- [search-in-a-binary-search-tree](LeetCode/LeetCode700search-in-a-binary-search-tree.py)

Coming from:https://leetcode-cn.com/problems/search-in-a-binary-search-tree/

- [insert-into-a-binary-search-tree](LeetCode/LeetCode701insert-into-a-binary-search-tree.py)

Coming from:https://leetcode-cn.com/problems/insert-into-a-binary-search-tree/

- [minimum-distance-between-bst-nodes](LeetCode/LeetCode783minimum-distance-between-bst-nodes.py)

Coming from:https://leetcode-cn.com/problems/minimum-distance-between-bst-nodes/

- [binary-tree-pruning](LeetCode/LeetCode814binary-tree-pruning.py)

```python
# 修剪值
if root.val == 0 and not root.left and not root.right:
    return None
else:
    return root
```
先递归到底层，然后在判断是否可以被修剪，修剪条件就是`root.val == 0 and not root.left and not root.right:`

Coming from:https://leetcode-cn.com/problems/binary-tree-pruning/

- [smallest-subtree-with-all-the-deepest-nodes](LeetCode/LeetCode865smallest-subtree-with-all-the-deepest-nodes.py)

构造了数据对\[root,depth]，用depth判断深度，用root返回depth对应的root

Coming from:https://leetcode-cn.com/problems/smallest-subtree-with-all-the-deepest-nodes/

- [leaf-similar-trees](LeetCode/LeetCode872leaf-similar-trees.py)

Coming from:https://leetcode-cn.com/problems/leaf-similar-trees/

- [all-possible-full-binary-trees](LeetCode/LeetCode894all-possible-full-binary-trees.py)

`基于树的动态规划，考前必看`

Coming from:https://leetcode-cn.com/problems/all-possible-full-binary-trees/

- [increasing-order-search-tree](LeetCode/LeetCode897increasing-order-search-tree.py)

Coming from:https://leetcode-cn.com/problems/increasing-order-search-tree/

- [range-sum-of-bst](LeetCode/LeetCode938range-sum-of-bst.py)

Coming from:https://leetcode-cn.com/problems/range-sum-of-bst/

- [flip-equivalent-binary-trees](LeetCode/LeetCode951flip-equivalent-binary-trees.py)

Coming from:https://leetcode-cn.com/problems/flip-equivalent-binary-trees/

- [check-completeness-of-a-binary-tree](LeetCode/LeetCode958check-completeness-of-a-binary-tree.py)

层次遍历，出现空之后不能再出现结点

Coming from:https://leetcode-cn.com/problems/check-completeness-of-a-binary-tree/

- [univalued-binary-tree](LeetCode/LeetCode965univalued-binary-tree.py)

Coming from:https://leetcode-cn.com/problems/univalued-binary-tree/

- [distribute-coins-in-binary-tree](LeetCode/LeetCode979distribute-coins-in-binary-tree.py)

金币题，题目有点难理解，算得是每个结点的多余量，这题和[jump-game](LeetCode/LeetCode55jump-game.py)神似

Coming from:https://leetcode-cn.com/problems/distribute-coins-in-binary-tree/

- [cousins-in-binary-tree](LeetCode/LeetCode993cousins-in-binary-tree.py)

这题是结合了父结点+子节点递归，利用depth保存层数，parent保存子结点对应的父结点：

```python
depth[root.val] = depth[par.val]+1 if par else 0
parent[root.val] = par
```
对于根层，depth\[root.val]=0，parent\[root.val]=None

Coming from:https://leetcode-cn.com/problems/cousins-in-binary-tree/

- [construct-binary-search-tree-from-preorder-traversal](LeetCode/LeetCode1008construct-binary-search-tree-from-preorder-traversal.py)

Coming from:https://leetcode-cn.com/problems/construct-binary-search-tree-from-preorder-traversal/

- [sum-of-root-to-leaf-binary-numbers](LeetCode/LeetCode1022sum-of-root-to-leaf-binary-numbers.py)

`^`在python里面是抑或，不是次方

Coming from:https://leetcode-cn.com/problems/sum-of-root-to-leaf-binary-numbers/

- [maximum-difference-between-node-and-ancestor](LeetCode/LeetCode1026maximum-difference-between-node-and-ancestor.py)

Coming from:https://leetcode-cn.com/problems/maximum-difference-between-node-and-ancestor/

- [delete-nodes-and-return-forest](LeetCode/LeetCode1110delete-nodes-and-return-forest.py)

复杂的dfs，在dfs的过程中对树进行修正和保存，有点难

Coming from:https://leetcode-cn.com/problems/delete-nodes-and-return-forest/


- [lowest-common-ancestor-of-deepest-leaves](LeetCode/LeetCode1123lowest-common-ancestor-of-deepest-leaves.py)

Coming from:https://leetcode-cn.com/problems/lowest-common-ancestor-of-deepest-leaves/

- [recover-a-tree-from-preorder-traversal](LeetCode/LeetCode1028recover-a-tree-from-preorder-traversal.py)

hashmap存结点，每次更新

Coming from:https://leetcode-cn.com/problems/recover-a-tree-from-preorder-traversal/


***

# 

