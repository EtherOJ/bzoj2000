
# Description

<div class="content"><div class="Section0" style="layout-grid:  15.6pt none">
<div>口袋妖怪(又名神奇宝贝或宠物小精灵)红/蓝/绿宝石中的水系道馆需要经过三个冰地才能到达馆主的面前，冰地中</div>
<div>的每一个冰块都只能经过一次。当一个冰地上的所有冰块都被经过之后，到下一个冰地的楼梯才会被打开。三个冰</div>
<div>地分别如下：</div>
<div><img src="/source/bzoj/2325/img/aHR0cHM6Ly9seWRzeS5jb20vSnVkZ2VPbmxpbmUvdXBsb2FkLzIwMTYwNS92LmpwZw==.jpg" width="397" height="428" alt=""/></div>
<div>当走出第三个冰地之后，就可以与馆主进行道馆战了。馆主发现这个难度太小，导致经常有挑战者能通过，为了加</div>
<div>大难度，将道馆分成了n个房间，每个房间中是两个冰块或障碍，表示一列冰地。任意两个房间之间均有且仅有一</div>
<div>条路径相连，即这n个房间构成一个树状结构。每个房间分成了A和B两个区域，每一区域都是一个薄冰块或者障碍</div>
<div>物。每次只能移动到相邻房间的同一类区域(即若你现在在这个房间的A区域，那么你只能移动到相邻房间的A区域)</div>
<div>或这个房间的另一区域。现在挑战者从房间u出发，馆主在房间v，那么挑战者只能朝接近馆主所在房间的方向过去</div>
<div>。一开始挑战者可以在房间u的任意一个冰块区域内。如果挑战者踩过的冰块数达到了最大值(即没有一种方案踩过</div>
<div>的冰块数更多了)，那么当挑战者走到最后一个冰块上时，他会被瞬间传送到馆主面前与馆主进行道馆战。自从馆</div>
<div>主修改规则后已经经过了m天，每天要么是有一个挑战者来进行挑战，要么就是馆主将某个房间进行了修改。对于</div>
<div>每个来的挑战者，你需要计算出他若要和馆主进行战斗需要经过的冰块数。</div>
<p class="p0" style="margin-top: 0pt; margin-bottom: 0pt"><span style="font-size: 10.5pt; font-family: &#39;Times New Roman&#39;; mso-spacerun: &#39;yes&#39;"><o:p></o:p></span></p>
</div>
<!--EndFragment--></div>

# Input

<div class="content"><div>
<div>第一行包含两个正整数n和m。第2行到第n行，每行包含两个正整数x和y，表示一条连接房间x和房间y的边。房间编</div>
<div>号为1…n。接下来n行，每行包含两个字符。第n + k行表示房间k的两个区域，第一个字符为A区域，第二个字符为</div>
<div>B区域。其中“.”(ASCII码为46)表示是薄冰块，“#”(ASCII码为35)表示是障碍物。最后的m行，每行一个操作：</div>
<div>l C u s：将房间u里的两个区域修改为s。</div>
<div>l Q u v：询问挑战者在房间u，馆主在房间v时，挑战者能与馆主进行挑战需要踩的冰块数。如果房间u的两个区域</div>
<div>都是障碍物，那么输出0。</div>
<div>N≤ 30 000</div>
<div>M ≤ 80 000</div>
</div>
<div></div>
<p></p></div>

# Output

<div class="content"><p class="p18" style="margin-top: 0pt; margin-bottom: 0pt">包含若干行，每行一个整数。即对于输入中的每个询问，依次输出一个答案。</p></div>

# Sample Input

<div class="content"><span class="sampledata">5 3<br/>
1 2<br/>
2 3<br/>
2 4<br/>
1 5<br/>
.#<br/>
..<br/>
#.<br/>
.#<br/>
..<br/>
Q 5 3<br/>
C 1 ##<br/>
Q 4 5</span></div>

# Sample Output

<div class="content"><span class="sampledata">6<br/>
3<br/>
<br/>
</span></div>

# Hint

<div class="content"><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search=Day2">Day2</a></p></div>

