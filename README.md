
# Description

<div class="content"><div>“猜单词”是一个双人游戏，在伊朗的青年学生中广为流行。假设有两个游戏者A和B，A作</div>
<div>为先手，首先在一个双方都知道的语料库中选出一个单词，并记在脑海中。随后，他在一张</div>
<div>小纸片上划下与单词字母数相等的小横线（不妨设为n条）。接下来，B尝试猜出这个单词。</div>
<div>每一轮，B选择一个字母并告诉 A。A按如下规则回应：若B 所说的字母在单词中出现，A就</div>
<div>把它写在对应的横线上。如果整个单词已经完整（所有的字母已经被猜出），B获胜。否则</div>
<div>，如果字母没有在单词中出现，A就把它写在最左侧的下方仍为空白的横线下。如果所有横</div>
<div>线下的空白处都已经有字母（也就是说，在这一轮前B已经猜了n个错误字母），那么B就输</div>
<div>了，A 获胜。例如，A 从语料库中选出了单词RED，且B已经依次猜了字母 A, E, C, D, B和</div>
<div>R。每一步的结果都在下图中展现。最终B 获胜。但如果B 在最后一步猜了S而不是R，他就</div>
<div>输了。</div>
<div></div>
<p><img height="162" alt="" width="782" src="/source/bzoj/2305/img/aHR0cHM6Ly9seWRzeS5jb20vSnVkZ2VPbmxpbmUvdXBsb2FkLzIwMTEwNS9pbWFnZS8yMzA1LnBuZw==.png"/></p>
<p></p>
<p></p>
<div>Aidin 是猜单词游戏迷。他相信，如果给定的语料库足够大，且其中的单词相对好，那么玩</div>
<div>家 A（先手）可以采取一种不公平的行动——修改选择的单词。也就是说，既然玩家 A 只</div>
<div>将单词记在脑海中而不写下来，那他能够在游戏过程中随时变化这个单词，只要使得和当前</div>
<div>已经给出的结果仍然一致即可。例如，在上面的游戏中，如果单词RED, BED, LED和TED都在</div>
<div>语料库中，那么在第4步之后，A就可以确信他将胜利。他将总是把B给出的字母写在横线下</div>
<div>（也就是认定其为错误的字母），那么每一次他将至多在集合  {RED, BED, LED, TED}  中</div>
<div>失去一个备选单词。最终他将向 B 宣布：“这个单词是，嗯，??”，然后在他的集合中说</div>
<div>出一个剩下的单词。Aidin 想，如果语料库足够好，那么 A 甚至可能在游戏一开始就确定</div>
<div>获胜。例如，如果选择的单词长度为2，而集合{ME, MD, DE, ED, AS, IS, AI, SI}中的单</div>
<div>词都在语料库中，那么A 总能获胜。请自己找出A 获胜的策略。给定一个语料库，Aidin想</div>
<div>知道是否无论B如何进行游戏，玩家A一定能获胜？请注意在任何一次游戏结束时，如果A获</div>
<div>胜，A需要能够给出一个语料库中的单词作为被选出的单词，这个单词应当与A所有给出的回</div>
<div>答一致。</div></div>

# Input

<div class="content"><div>输入包含若干个语料库。每个语料库应该被独立地处理。</div>
<div>输入的第一行是一个整数 C，代表语料库的数目。</div>
<div>随后 C 个语料库以 C 个模块的形式出现在输入中。每两个模块之间以一个空行隔开。</div>
<div>1 ≤ C ≤ 20。</div>
<div>对于每个输入模块，第一行包含一个正整数 k，表示语料库中单词的个数。</div>
<div>接下来的若干行中包含k个单词。相邻的单词以空格、制表符或换行符分隔。</div>
<div>每个单词由小于7个大写英语字母组成。</div>
<div>每个单词都由不同的字母组成，也就是说，同一个字母在一个单词中出现的次数不会超过1次。</div></div>

# Output

<div class="content"><div>对于每个语料库，如果玩家A有必胜策略（也就是说，不论B按什么方法猜，A总能获胜），</div>
<div>输出一行“Yes”。否则输出一行“No”。输出不包含引号。</div>
<div>对于所有测试数据中，k≤1000。</div></div>

# Sample Input

<div class="content"><span class="sampledata">2<br/>
12<br/>
SI ME AND AI ARE MD AS WHEN ED IS DE<br/>
HAPY<br/>
<br/>
5<br/>
A B AB AC AD</span></div>

# Sample Output

<div class="content"><span class="sampledata">Yes<br/>
No</span></div>

# Hint

<div class="content"><p></p><p>数据为国际加国内综合版</p><p></p></div>

# Source

<div class="content"><p><a href="problemset.php?search="></a></p></div>

