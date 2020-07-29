
# Description

<div class="content"><p><span style="font-size: medium"><br/>
一个异或门有两组输入并产生一组输出：</span></p>
<p><span style="font-size: medium">input 1   input 2    output<br/>
   0         0          0<br/>
   0         1          1<br/>
   1         0          1<br/>
   1         1          0</span></p>
<p><span style="font-size: medium">如果一个有n个输入1个输出的 由异或门构成的系统 满足下列条件，那么称它为异或网络：</span></p>
<p><span style="font-size: medium">1. 网络的每个输入端和至少一个异或门的输入端相连接<br/>
2. 每个异或门的输入端和网络的输入端或者某个异或门的输出端相连<br/>
3. 只有一个异或门的输出端和网络的输出端相连<br/>
4. 每个异或门的输出端要么和至少一个异或门的输入端相连，要么和网络的输出端相连<br/>
5. 存在一个对异或门的编号方式，使得对每个异或门的每个输入端都连接到网络的输入端 或者 一个编号更小的异或门的输出端</span></p>
<p><span style="font-size: medium">例如：</span></p>
<p><span style="font-size: medium">&lt;img src=&#34;</span><a href="http://main.edu.pl/images/OI4/xor1.gif"><span style="font-size: medium">http://main.edu.pl/images/OI4/xor1.gif</span></a><span style="font-size: medium">&#34; alt=&#34;example /&gt;</span></p>
<p><span style="font-size: medium">这是个由6个异或门组成的网络，它有5个输入端和1个输出端，并且满足上述所有条件，所以它是个异或网络。注意：上图中的编号并不符合第五个要求，但是确实存在一种编号方法使它满足第五个要求。</span></p>
<p><span style="font-size: medium">一个网络的输入端从1到n编号。每个引脚的高低电位由一个长度为n的01字符串给定。我们假设第i个字符代表着第i个输入引脚的电位。对于每一组输入电位，网络产生一个输出电位，用01表示。注意到每组输入的字符串都是一个代表自然数的二进制串，所以我们可以把输入的字符串按照它们代表的自然数的大小排序。我们会发送固定范围内的自然数到输入端，然后记下有多少次返回了1。</span></p>
<p><span style="font-size: medium">你的任务：</span></p>
<p><span style="font-size: medium">写一个程序：</span></p>
<p><span style="font-size: medium">* 读入关于异或网络的描述：输入引脚数量n，异或门数量m，连接到网络的输出引脚的异或门编号，以及异或门的连接方式<br/>
* 读入两个长度为n的二进制串，代表上下区间<br/>
* 计算区间内有多少组输入会使网络返回1<br/>
* 输出答案</span></p>
<p><span style="font-size: medium">假设 3 &lt;= n &lt;= 100，3 &lt;= m &lt;= 3000，输入门从1到m任意编号。</span></p>
<p></p></div>

# Input

<div class="content"><p><span style="font-size: medium">第一行，3个整数：输入引脚数量n，异或门数量m，连接到网络的输出引脚的异或门编号</span></p>
<p><span style="font-size: medium">接下来m行代表异或门的连接方式，在这里的第i行代表第i个异或门的两个输入端，输入在[-n, m]的两个数：如果是-k那么连接到第k个异或门的输入脚，否则连接到输出脚。</span></p>
<p><span style="font-size: medium">最后有两行n位的字符串，代表着上下区间。假设给定的字符串长度不超过 100000</span></p>
<p></p></div>

# Output

<div class="content"><p><span style="font-size: medium">一个数：对于给定区间内的输入，有多少个会得到1</span></p>
<p></p></div>

# Sample Input

<div class="content"><span class="sampledata">5 6 5<br/>
-1 -2<br/>
1 3<br/>
1 -2<br/>
2 -3<br/>
4 6<br/>
-4 -5<br/>
00111<br/>
01110<br/>
<br/>
<br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata"><br/>
5<br/>
</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

