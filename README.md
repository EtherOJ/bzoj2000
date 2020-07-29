
# Description

<div class="content"><div><span style="font-size: medium">a180285幸运地被选做了地球到喵星球的留学生。他发现喵星人在上课前的点名现象非</span><span style="font-size: medium">常有趣。 </span><span style="font-size: medium">  假设课堂上有N个喵星人，每个喵星人的名字由姓和名构成。喵星球上的老师会选择</span><span style="font-size: medium">M个串来点名，每次读出一个串的时候，如果这个串是一个喵星人的姓或名的子串，那么</span><span style="font-size: medium">这个喵星人就必须答到。 </span><span style="font-size: medium">然而，由于喵星人的字码过于古怪，以至于不能用ASCII码来表示。为了方便描述，</span><span style="font-size: medium">a180285决定用数串来表示喵星人的名字。 </span></div>
<div><span style="font-size: medium">现在你能帮助a180285统计每次点名的时候有多少喵星人答到，以及M次点名结束后</span><span style="font-size: medium">每个喵星人答到多少次吗？   </span></div></div>

# Input

<div class="content"><div> </div>
<div><span style="font-size: medium">现在定义喵星球上的字符串给定方法： </span></div>
<div><span style="font-size: medium">先给出一个正整数L，表示字符串的长度，接下来L个整数表示字符串的每个字符。 </span></div>
<div><span style="font-size: medium">输入的第一行是两个整数N和M。 </span></div>
<div><span style="font-size: medium">接下来有N行，每行包含第i 个喵星人的姓和名两个串。姓和名都是标准的喵星球上的</span></div>
<div><span style="font-size: medium">字符串。 </span></div>
<div><span style="font-size: medium">接下来有M行，每行包含一个喵星球上的字符串，表示老师点名的串。 </span></div></div>

# Output

<div class="content"><div><span style="font-size: medium"> </span></div>
<div><span style="font-size: medium">对于每个老师点名的串输出有多少个喵星人应该答到。 </span></div>
<div><span style="font-size: medium">然后在最后一行输出每个喵星人被点到多少次。 </span></div></div>

# Sample Input

<div class="content"><span class="sampledata">2 3 <br/>
6 8 25 0 24 14 8 6 18 0 10 20 24 0 <br/>
7 14 17 8 7 0 17 0 5 8 25 0 24 0 <br/>
4 8 25 0 24 <br/>
4 7 0 17 0 <br/>
4 17 0 8 25 <br/>
</span></div>

# Sample Output

<div class="content"><span class="sampledata"><br/>
2 <br/>
1 <br/>
0 <br/>
1 2 <br/>
【提示】 <br/>
事实上样例给出的数据如果翻译成地球上的语言可以这样来看 <br/>
2 3 <br/>
izayoi sakuya <br/>
orihara izaya <br/>
izay <br/>
hara <br/>
raiz </span></div>

# Hint

<div class="content"><p></p><p><br/><br/>
【数据范围】 <br/><br/>
 对于30%的数据，保证： <br/><br/>
1&lt;=N,M&lt;=1000，喵星人的名字总长不超过4000，点名串的总长不超过2000。<br/><br/>
对于100%的数据，保证：<br/><br/>
1&lt;=N&lt;=20000，1&lt;=M&lt;=50000，喵星人的名字总长和点名串的总长分别不超过100000，保证喵星人的字符串中作为字符存在的数不超过10000。</p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

