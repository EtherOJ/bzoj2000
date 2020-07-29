
# Description

<div class="content"><div>
<div>眼看着假期就要到了，Crash由于长期切题而感到无聊了，因此他决定利用这个假期和好友陶陶一起出去旅游。</div>
<div>Crash和陶陶所要去的城市里有N (N &gt; 1) 个景点，Crash用正整数1到N给景点标号。</div>
<div>这些景点之间通过N - 1条无向道路相连，每条道路有一个长度，并且保证任意两个景点之间都有且仅有一条路径相连。</div>
<div>现在对于一个景点s，Crash和陶陶从s出发，然后访问一个景点序列{v0, v1, v2, … , vk}，</div>
<div>其中v0就是s，且vi-1和vi(0 &lt; i ≤ k)之间有道路相连。</div>
<div>需要注意的是，陶陶和Crash访问的景点序列中不会只有景点s。</div>
<div>为了使旅程不显得乏味，在一个景点序列里他们不会重复走某条道路。</div>
<div>我们定义这个序列的旅游代价为经过道路的长度和。下面问题出现了：</div>
<div>陶陶：我们走一条景点数最多的景点序列吧。</div>
<div>Crash：倒，你想把我累死啊。</div>
<div>陶陶：谁叫你整天坐在电脑前面，不出来锻炼，这下子傻了吧，哈哈哈哈~~</div>
<div>Crash：不行，如果你非要走景点数最多的我就不陪你走了。</div>
<div>陶陶：笑喷油你很跳嘛！</div>
<div>Crash：这样吧，我们来写伸展树，如果我写的比你快，你就要听我的。</div>
<div>陶陶：这样不公平哎，我们来玩PES吧，当然你要让我选法国队，如果你输了你就要听我的。</div>
<div>Crash：倒，你这是欺负我，T_T~</div>
<div>陶陶：笑喷油好说话哎。</div>
<div>Crash：囧……</div>
<div>……</div>
<div>这样搞了半天，最终陶陶和Crash用很多次包剪锤决定出选择旅游代价第K小 的景点序列。</div>
<div>不过呢Crash和陶陶还没确定开始旅行的景点s，因此他希望你对于每个景点i，计算从景点i开始的景点序列中旅游代价第K小的值。</div>
</div></div>

# Input

<div class="content"><div>共N行。</div>
<div>第1行包含一个字符和两个正整数，字符为ABCD中的一个，用来表示这个测试数据的类型</div>
<div>（详见下面的数据规模和约定），另外两个正整数分别表示N和K (K &lt; N),N&lt;=<span style="font-family: Helvetica, &#39;Microsoft Yahei&#39;, verdana; font-size: 14.3999996185303px; line-height: 18.659200668335px;">100000</span></div>
<div>第2行至第N行，每行有三个正整数u、v和w (u, v ≤ N，w ≤ 10000)。</div>
<div>表示u号景点和v号景点之间有一条道路，长度为w。</div>
<div>输入文件保证符合题目的约定，即任意两个景点之间都有且仅有一条路径相连。</div></div>

# Output

<div class="content"><div>共N行，每行有一个正整数。</div>
<div>第i行的正整数表示从i号景点开始的景点序列中旅游代价第K小的代价。</div></div>

# Sample Input

<div class="content"><span class="sampledata">A 6 3<br/>
1 2 2<br/>
1 3 4<br/>
1 4 3<br/>
3 5 1<br/>
3 6 2<br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata">4<br/>
6<br/>
4<br/>
7<br/>
5<br/>
6<br/>
//样例1中输出对应的景点序列分别为：<br/>
1号景点是{1, 3}，2号景点是{2, 1, 3}，3号景点是{3, 1}，4号景点是{4, 1, 3}，5号景点是{5, 3, 1}，6号景点是{6, 3, 1}。 <br/>
保证每个景点到1号景点需要经过的道路数不超过30</span></div>

# Hint

<div class="content"><p></p><p> <img src="/source/bzoj/2117/img/aHR0cHM6Ly9seWRzeS5jb20vSnVkZ2VPbmxpbmUvdXBsb2FkLzIwMTcxMS92djEuanBn.jpg" width="885" height="288" alt=""/></p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

