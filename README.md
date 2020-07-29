
# Description

<div class="content"><p>世博期间，上海的航空客运量大大超过了平时，随之而来的航空管制也频频 发生。最近，小X就因为航空管制，连续两次在机场被延误超过了两小时。对此， 小X表示很不满意。  在这次来烟台的路上，小 X不幸又一次碰上了航空管制。于是小 X开始思考 关于航空管制的问题。  假设目前被延误航班共有 n个，编号为 1至n。机场只有一条起飞跑道，所 有的航班需按某个顺序依次起飞（称这个顺序为起飞序列）。定义一个航班的起 飞序号为该航班在起飞序列中的位置，即是第几个起飞的航班。  起飞序列还存在两类限制条件：    第一类（最晚起飞时间限制）：编号为 i的航班起飞序号不得超过 ki;    第二类（相对起飞顺序限制）：存在一些相对起飞顺序限制(a, b)，表示 航班 a的起飞时间必须早于航班 b，即航班 a的起飞序号必须小于航班 b 的起飞序号。  小X 思考的第一个问题是，若给定以上两类限制条件，是否可以计算出一个 可行的起飞序列。第二个问题则是，在考虑两类限制条件的情况下，如何求出每 个航班在所有可行的起飞序列中的最小起飞序号。</p></div>

# Input

<div class="content"><p>第一行包含两个正整数 n和m，n表示航班数目，m表示 第二类限制条件（相对起飞顺序限制）的数目。  第二行包含 n个正整数 k1, k2, „, kn。  接下来 m行，每行两个正整数 a和b，表示一对相对起飞顺序限制(a, b)， 其中1≤a,b≤n, 表示航班 a必须先于航班 b起飞。</p></div>

# Output

<div class="content"><p>包含 n个整数 t1, t2, „, tn，其中 ti表示航班i可能的最小起飞序 号，相邻两个整数用空格分隔。</p></div>

# Sample Input

<div class="content"><span class="sampledata">5 5 <br/>
4 5 2 5 4 <br/>
1 2 <br/>
3 2 <br/>
5 1 <br/>
3 4 <br/>
3 1 <br/>
<br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata">3 4 1 2 1 <br/>
<br/>
在样例 1 中： <br/>
起飞序列 3 5 1 4 2 满足了所有的限制条件，所有满足条件的起飞序列有： <br/>
3 4 5 1 2           3 5 1 2 4           3 5 1 4 2           3 5 4 1 2 <br/>
5 3 1 2 4           5 3 1 4 2           5 3 4 1 2 <br/>
由于存在(5, 1)和(3, 1)两个限制，航班1只能安排在航班 5和3之后，故最早<br/>
起飞时间为3，其他航班类似。 <br/>
<br/>
<br/>
对于30%数据：n≤10； <br/>
对于60%数据：n≤500； <br/>
对于100%数据：n≤2,000，m≤10,000。 </span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

