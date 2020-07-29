
# Description

<div class="content"><div style="margin: 13pt 0cm">lanwuni接到一个任务，在C市建立<i>N</i>个信号塔来完成城市中的通讯任务。</div>
<div>假设C市是一个坐标范围[-2000000,2000000]的网格，一些整点上有用户，你也可以在整点上建立信号塔。一个点上可以建立多座。</div>
<div>在C市，两点之间的距离是曼哈顿距离，也就是横纵坐标差值之和。每个信号塔都有一个半径<i>D<sub>i</sub></i>，表示与<i>i</i>曼哈顿距离不超过<i>D<sub>i</sub></i>的地方都能被这个信号塔的信号覆盖到。</div>
<div>建立信号塔要满足一些性质：</div>
<div>1.<span>       每个信号塔有一定的用户，lanwuni要把信号塔建立在某个地方，使得属于该塔的用户都能被信号覆盖到；</span></div>
<div>2.<span>       信号塔有一定等级和安装限制，所以，第<i>i</i>号信号塔能覆盖的所有整点，必须也被第<i>i</i>+1号信号塔覆盖到。即使这个整点上没有用户。</span></div>
<div>现在告诉你每个信号塔的半径，以及每个信号塔的用户，请你帮lanwuni谋划一下应该把这<i>N</i>个信号塔建立在什么地方。</div></div>

# Input

<div class="content"><div>第一行2个整数<i>N</i>、<i>M</i>，分别表示信号塔个数、用户总个数。</div>
<div>第二行<i>N</i>个整数，第<i>i</i>个数<i>D<sub>i</sub></i>表示第<i>i</i>号信号塔的半径。</div>
<div>第3到第<i>M</i>+2行，每行3个整数<i>U<sub>i</sub></i>、<i>X<sub>i</sub></i>、<i>Y<sub>i</sub></i>，表示第<i>U<sub>i</sub></i>号信号塔有一个用户在坐标[<i>X<sub>i</sub></i>,<i>Y<sub>i</sub></i>]的地方。</div>
<div>数据保证<i>D<sub>i</sub>&lt;=D<sub>i</sub></i><sub>+1</sub>（i&lt;N）。</div></div>

# Output

<div class="content"><div>输出包括<i>N</i>行，每行2个整数，表示第<i>i</i>个信号塔的坐标。</div>
<div>数据保证有解。</div></div>

# Sample Input

<div class="content"><span class="sampledata">【样例输入一】<br/>
2 2<br/>
2 5<br/>
1 6 8<br/>
2 11 11 <br/>
 <br/>
【样例输入二】<br/>
6 6<br/>
1 3 5 6 6 7<br/>
1 21 27<br/>
2 23 27<br/>
3 19 27<br/>
4 21 33<br/>
5 23 29<br/>
6 26 30<br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata">【样例输出一】<br/>
5 9<br/>
6 11<br/>
<br/>
【样例输出二】<br/>
20 27<br/>
20 27<br/>
19 28<br/>
19 29<br/>
19 29<br/>
19 30<br/>
</span></div>

# Hint

<div class="content"><p></p><p><br/><br/>
【数据范围】<br/><br/>
100%的数据中，1&lt;=N,M&lt;=100000，|Xi|,|Yi|,|Di|&lt;=1000000。</p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=鲁逸沁  鸣谢Benz提供SJ程序！">鲁逸沁  鸣谢Benz提供SJ程序！</a></p></div>

