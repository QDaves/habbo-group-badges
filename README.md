# Habbo Hotel group badges
This documentation explains how badges are structured and how they are hashed.

## Badge structure
Badges typically consist of <b>0-n</b> badge parts. Badge parts are divided in 3 different types:
- <b>b</b>: Base parts
- <b>s</b>: Additional parts (1-99)
- <b>t</b>: Additional parts (100-199)

Both types of badge parts are built using 1 letter and 5 digits:

<table>
<tr>
<td><b>Type</b></td>
<td><b>Badge part ID</b></td>
<td><b>Color</b></td>
<td><b>Position</b></td>
</tr>
<tr>
<td>b/s/t</td>
<td>00-99</td>
<td>01-24</td>
<td>0-8</td>
</tr>
</table>

All 3 badge parts are optional, but when a badge part is added, it <b>must</b> contain the letter and <b>exactly 5</b> digits. If your `Badge Part ID` or `Color` are below 10, add a leading 0.

### The difference between types

The main difference between `b` and `s` or `t` is that `b` can only display base parts, and the others can only display additional parts. It is also worth noting that a badge can contain multiple base parts.

There's also a slight difference between `s` and `t`. There's between 100 and 200 different additional parts available in Habbo, but a badge part only takes 5 digits, so `Badge part ID` can't be more than 99. To still use an additional part that goes above 99, we can use `t`. When `t` is set to 00, that equals `Badge part ID` 100, 10 equals `Badge part ID` 110, etc. For `Badge part ID` 1 to 99, you can use `s`.

### Badge part IDs

A `Badge part ID` is a 2-digit number that represents a certain image or shape in your badge. Base- and additional parts both have their own IDs. A few of them are displayed below.

#### Base
<table>
<tr>
<td><b>ID 1</b></td>
<td><b>ID 2</b></td>
<td><b>ID 3</b></td>
<td><b>ID 4</b></td>
<td><b>ID 5</b></td>
<td><b>ID 6</b></td>
<td><b>ID 7</b></td>
<td><b>ID 8</b></td>
<td><b>ID 9</b></td>
<td><b>ID 10</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b011208e970587dc251481d734bd9315d6f086.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b0212032986cb5f8a9ebf3ee8966782d421ee2.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b0312011748398e35232e4bf1ae3a8b399b947.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b041206e6fd9d3e8fc61d1b6cba990e5d98b34.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b051201a7e6e649972ca4e1544a7de4118ba34.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b061203ef9950a7238dc718d4319d7980e90f0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b0712059e0b95e9716cec464cdc2170d229e41.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b081209fc49879657894cbe937ae47f8ec2ec7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b0912008c0a4b2292f088b151f882bc42ef4a0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b101203123eadfb7c400aafaa28987bfe14feb.gif"></td>
</tr>
</table>

<table>
<tr>
<td><b>ID 11</b></td>
<td><b>ID 12</b></td>
<td><b>ID 13</b></td>
<td><b>ID 14</b></td>
<td><b>ID 15</b></td>
<td><b>ID 16</b></td>
<td><b>ID 17</b></td>
<td><b>ID 18</b></td>
<td><b>ID 19</b></td>
<td><b>ID 20</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b11120e535661c30e6bac187019a52427f7b4a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b12120bddeac5d30eac3ff1359faf06de1f230.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b131209642c0d1ff28ab927d2926a8fab8e1fc.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b141203710798dc81692c012a3709442a701ca.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b1512059b0ce3b2238440c732db5e696081e92.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b16120fedca5df6da9953bbea77d0e916e791d.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b17120a88bfa13b50e9f07ce24bd361ec96691.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b18120da3469934d7c1aa5e0f14ddda76d7b48.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b191203eabb7347eee2954b13647380c473902.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b20120e5221add96c902a553375d5e77652184.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 21</b></td>
<td><b>ID 22</b></td>
<td><b>ID 23</b></td>
<td><b>ID 24</b></td>
<td><b>ID 25</b></td>
<td><b>ID 26</b></td>
<td><b>ID 27</b></td>
<td><b>ID 28</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b211204df307402887c8b44f231c37ab2ee317.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b22120fd9440931d8a7b1e48fd7e952f0249a7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b23120538a0f90059c9e4151bfe48a0f287da3.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b2412003f8731ac66b33e5d2d94264e0ab0809.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b251208614baab44a7f03c63c2eacccbb5c311.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b26120798469a46c33fa04095df8d55dfeb74d.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b2712080daf264494282d06820bc1cf7ac69d8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/b28120e408693239e9f3139ee9286d0e2f8b5f.gif"></td>
</tr>
</table>

#### Additional
<table>
<tr>
<td><b>ID 1</b></td>
<td><b>ID 2</b></td>
<td><b>ID 3</b></td>
<td><b>ID 4</b></td>
<td><b>ID 5</b></td>
<td><b>ID 6</b></td>
<td><b>ID 7</b></td>
<td><b>ID 8</b></td>
<td><b>ID 9</b></td>
<td><b>ID 10</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s011245386582bffcd2120314718564e688eae.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s0212460ebb3b272def888c7a67d1fa897dcaf.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s03124958973280f42185fbe9a33f58b9d3241.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s041245d1cebe410fd6841e630d4515eadee46.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s051242dba9550b0ca38978a2447af1f596ed5.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s06124615c94e2ae0ba2b964d6f8e3f60a99d3.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s0712453b2506d862f64259c7fb2ea61c7bbc1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s08124eea7932d7aa26081b7bb3d3707824f57.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s091247185d316deb02c0dea7641addb92e7b0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s10124e04c02c25fd47f13b3bdc7762e35bf1c.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 11</b></td>
<td><b>ID 12</b></td>
<td><b>ID 13</b></td>
<td><b>ID 14</b></td>
<td><b>ID 15</b></td>
<td><b>ID 16</b></td>
<td><b>ID 17</b></td>
<td><b>ID 18</b></td>
<td><b>ID 19</b></td>
<td><b>ID 20</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s111242ecd29d55ec268fa27eff4a7211a7c09.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s1212453cb401607955e1b9117247104bb6ebf.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s131249531ea3045a7a6483027aaca7d31caef.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s14124e9756cc849c4cf356bce100364763056.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s151241a825cfdff3327f30feec3b2739543f9.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s16124eed7169ad8ba19566ac1e153db1f8e9a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s1712467c45b48a8ef350b8e5ee368fec65b3a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s181245015d7b6297a08745130d404f1aeadaf.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s191246daaad4ef8bc17ceca88416e74f048d0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s2012462b9d1b62163d8f7c8df59a04616a00e.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 21</b></td>
<td><b>ID 22</b></td>
<td><b>ID 23</b></td>
<td><b>ID 24</b></td>
<td><b>ID 25</b></td>
<td><b>ID 26</b></td>
<td><b>ID 27</b></td>
<td><b>ID 28</b></td>
<td><b>ID 29</b></td>
<td><b>ID 30</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s211243cd45eb4072c56e18e0f7a647b4a97a0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s22124c316ad01a65bf7c6ce12e6ccf4d7aff7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s231244deb5b3e54af46253ce388a8fc465e23.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s24124769f691ba85494c0f4d7d02ac62a538c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s251243cfb70cd59324fca988dfdf025da986a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s2612437de1112ae8ff436a373d8f8ae89061c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s271241de8eef7795b9d99e883d8775bf50edf.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s28124decd9d12830ebef3984553ab5af87f4f.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s291244947cc92022a180a3339b8fd12985421.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s301243a1387d4676133151094a7d5a152b873.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 31</b></td>
<td><b>ID 32</b></td>
<td><b>ID 33</b></td>
<td><b>ID 34</b></td>
<td><b>ID 35</b></td>
<td><b>ID 36</b></td>
<td><b>ID 37</b></td>
<td><b>ID 38</b></td>
<td><b>ID 39</b></td>
<td><b>ID 40</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s31124023129768796b87265573ad4701b4bd6.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s32124bb4a03deac1a6d46d578b499f0d60fde.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s33124188830c786719cec1362342e97a2713a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s341245abdaabb8593f74d45a4a0d3f7c9852b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s35124de90e59c5f58a184a5d4b954d3fb027f.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3612419ad66c11665a8813f9423b440b6d0d8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3712461206bede1e4f3349871210b52a77f4f.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3812448e4d3c0288867003fedd84feb146373.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s39124fd6aed9b28a37588668854529b97de17.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s4012442e881525fb12009cf6d92062a571c5d.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 41</b></td>
<td><b>ID 42</b></td>
<td><b>ID 43</b></td>
<td><b>ID 44</b></td>
<td><b>ID 45</b></td>
<td><b>ID 46</b></td>
<td><b>ID 47</b></td>
<td><b>ID 48</b></td>
<td><b>ID 49</b></td>
<td><b>ID 50</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s4112455a9d0519a388978268d22045f57b043.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s421243ac77fef355cfec232fc0990abb70958.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s43124e7ae66fb86d7b13d3b376ad15e24efd7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s441248128680323ddc4047ded4ab58bce504c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s45124929d1a8a1c1ae6abc0eb39b56bb6615b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s46124e0b8389b3c0e3ee0195ecc3a76f6daef.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s47124bc5a9cc424b8722a247cb03df0a24aa6.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s48124f3d98116636f8f555796e28eb12d7d57.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s49124c4c9c2a6293b4aca1dc170a6b0ff0c08.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s501243f5aaf6e2579fe3f9e5b0e3c1fc759cf.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 51/b></td>
<td><b>ID 52</b></td>
<td><b>ID 53</b></td>
<td><b>ID 54</b></td>
<td><b>ID 55</b></td>
<td><b>ID 56</b></td>
<td><b>ID 57</b></td>
<td><b>ID 58</b></td>
<td><b>ID 59</b></td>
<td><b>ID 60</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s5112461e923835c06dd41376737d1ae73859c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s521248158874630af7cba2d6c92acde075c1e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s53124acb6b0805b29ce4aa8e5d9acc505423e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s541245b1512cd2ca38bfd8db1d212b7227e84.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s55124254a1b3b3ced3c330d55f6b1a997a096.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s56124b63097d346aafc85a8296307216a2873.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s571240e9676c26b76297debfea8c1f79a71ce.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s58124e553163453b607d64841dbdf7cfb4d95.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s59124f0d167c618876de0743220b87c963a14.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s60124ec84224f9a7b3c88965c7a25d9f62ae4.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 61</b></td>
<td><b>ID 62</b></td>
<td><b>ID 63</b></td>
<td><b>ID 64</b></td>
<td><b>ID 65</b></td>
<td><b>ID 66</b></td>
<td><b>ID 67</b></td>
<td><b>ID 68</b></td>
<td><b>ID 69</b></td>
<td><b>ID 70</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s61124add2c37d823d1401bc78e41c80e6c7a1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s62124b04ab805780e8578fd11ad37c83d56d6.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s63124dc8255ed87c7765655cca965f5ed893b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s641246dc3f6bba6901a868c58367ef7bdf83b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s65124d4766fc99f5f68f09c5d4f6373184113.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s6612486b4b8d1662ccd74777897e420daffb6.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s67124f1a8c205ca9304b1e42d2f1b5a88403a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s68124d3dc9d1f652b353679340a5f0c58dd6b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s69124e1f3607025dc4b6021102d7d87fa821a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s70124d0c92d0aaa8735a904cdb0360a6e3408.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 71</b></td>
<td><b>ID 72</b></td>
<td><b>ID 73</b></td>
<td><b>ID 74</b></td>
<td><b>ID 75</b></td>
<td><b>ID 76</b></td>
<td><b>ID 77</b></td>
<td><b>ID 78</b></td>
<td><b>ID 79</b></td>
<td><b>ID 80</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s711240b517641bc5754ee759d46597f44c436.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s721240eff82b47765df167065570dd842e566.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s731247d85457c78c29580a58ed5e1d8ca9603.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s74124b40fd046f5a8b9335e4a58253d7ec57e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s75124395438e6cdb5e9c5c959a27f69b34a14.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s761246f3e7376b26077a59bf99b15fc3e2b62.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s771249b0379878a838ca3e52be470249f8e95.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s78124762ef43c66c559e5923d8fe739cb5988.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s79124304c9effdc5064e4b7a95f3b951c1dc7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s8012446144369211506f7147b0027ac52b6f0.gif"></td>

</tr>
</table>

<table>
<tr>
<td><b>ID 81</b></td>
<td><b>ID 82</b></td>
<td><b>ID 83</b></td>
<td><b>ID 84</b></td>
<td><b>ID 85</b></td>
<td><b>ID 86</b></td>
<td><b>ID 87</b></td>
<td><b>ID 88</b></td>
<td><b>ID 89</b></td>
<td><b>ID 90</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s811241be22bb201854d7c95afdbfe78d7db03.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s82124f220665c9af6791f750e31bb44c82d0f.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s83124782282f5c0e798ecb453a5026c14f589.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s84124422d0943a6f2491dea1ed66403e63014.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s851249cc69336dc48aecb21c82300d23d9099.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s86124d73b4096d221c8442c503c635256379e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s87124386c6dc72d38dce88f629679ec796d92.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s8812424ca1e30798dc4362ff1b84a19c78946.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s891244c030c00272234fe3e8e767294f73143.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s901242777c7962942009ba874204d2cb4e3da.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 91</b></td>
<td><b>ID 92</b></td>
<td><b>ID 93</b></td>
<td><b>ID 94</b></td>
<td><b>ID 95</b></td>
<td><b>ID 96</b></td>
<td><b>ID 97</b></td>
<td><b>ID 98</b></td>
<td><b>ID 99</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s91124ffba94f98be511aba4f270d3cb3f0670.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s92124fa56b72125fa21e21f5aaed9847fc8ea.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s93124975703c229a96a1c9756d555267cc4f2.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s9412457ddbe972a5b11f2677b9853c53f0111.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s951246f25102a519da4535b75ce7b01c19f51.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s961248d375b9fa6f35cb57d5e727f5fe3423b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s97124713ab7c532af0a7bcc8cc6db1418300c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s981244c604858828968334d51ecf6c486f890.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s99124a406923c3a200bb53804ee78e82acb4e.gif"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 1</b></td>
<td><b>ID 2</b></td>
<td><b>ID 3</b></td>
<td><b>ID 4</b></td>
<td><b>ID 5</b></td>
<td><b>ID 6</b></td>
<td><b>ID 7</b></td>
<td><b>ID 8</b></td>
<td><b>ID 9</b></td>
<td><b>ID 10</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t00114148ce81ff9bd376ab826ea543cadfb11"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t01114d0055aba5d36eb6636c29a37fe30597f"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t0211420be752a60e8bd702dd3c608fa98fab7"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t031145e5746b69517440563794394231d56be"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t04114efb4542cea388a06e2fdd110b2169ae7"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t05114fe5a67be70393ff04fdabb23ff28c309"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t06114b6a3074e054c0cc8c9a1786c87319f1a"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t071145a05be5a131248a522821ee8587e881b"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t0811481bab935609621489ae43b4c410d0fd6"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t0911437e925dd67f27e2b8cebc4e4dccac4a0"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 11</b></td>
<td><b>ID 12</b></td>
<td><b>ID 13</b></td>
<td><b>ID 14</b></td>
<td><b>ID 15</b></td>
<td><b>ID 16</b></td>
<td><b>ID 17</b></td>
<td><b>ID 18</b></td>
<td><b>ID 19</b></td>
<td><b>ID 20</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t10114a2138106163426d7202faa43266b6600"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t11114cd7715a94927438f59a4e17c31460dd3"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t121148a34e6af25d920a5219ad722bc3d1a2e"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t13114314e5d514b35c0b2a3a670173e2f79d0"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t14114e5d323aa57635728a919a64ce963544a"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t15114244aaabdfec816e202dd9439b5bea55c"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t16114bc2d6b2422d50615f85069bf4e6ffeb3"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t1711441b69285c36c2fd118592631cd14a0f2"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t181142986ec0827f6b62ec32bec551fd1f11d"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t191145d7b50f1f16da371066d6c7727c247c2"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 21</b></td>
<td><b>ID 22</b></td>
<td><b>ID 23</b></td>
<td><b>ID 24</b></td>
<td><b>ID 25</b></td>
<td><b>ID 26</b></td>
<td><b>ID 27</b></td>
<td><b>ID 28</b></td>
<td><b>ID 29</b></td>
<td><b>ID 30</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t20114c27023e05ed87c6166bf628ed60bfacf"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t2111403d35c4f0666d82d9f61e448f06df9f6"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t221141b9b4d5b24529f5b71568d03dc91c1e5"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t23114d9ff9a42c6b4fd9754c9fad061d962d4"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t24114d02b80279ad2d0aefc1687e5e7861d32"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t251144bf8365aa2ea6ffe33f1914a78720e94"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t261140439fbc6c51b5348992813fd3a00f70f"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t271148276406340ac845e5af84ceaeebbd118"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t281147865c7d7a4543ffa22c91baf0bc1dcb4"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t291144a7deb3c98ea503e73f498cd1c2952e7"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 31</b></td>
<td><b>ID 32</b></td>
<td><b>ID 33</b></td>
<td><b>ID 34</b></td>
<td><b>ID 35</b></td>
<td><b>ID 36</b></td>
<td><b>ID 37</b></td>
<td><b>ID 38</b></td>
<td><b>ID 39</b></td>
<td><b>ID 40</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t3011485c0c4f4b1ce39ab515f01fa9377b83f"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t31114b14a05e2d44482688274d8f356b17c9d"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t3211468daafe8ab21ff6ef2b41a585221d236"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t33114b6bbf626b763cb54a59cbe09c57d6097"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t341149e3fb1b0addbd0c03dafc60f7ec35c6f"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t3511433f72ba7e5274540718a3401c4b838b2"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t36114c0de98132a6348459c7ab9d64a247b8c"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t371145298a8e0194a8d08917ca8ebb960df1f"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t381149fb2fa850141f655b36fd2ad3e033f37"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t39114e8078f6552b092ec337a09193b05202e"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 41</b></td>
<td><b>ID 42</b></td>
<td><b>ID 43</b></td>
<td><b>ID 44</b></td>
<td><b>ID 45</b></td>
<td><b>ID 46</b></td>
<td><b>ID 47</b></td>
<td><b>ID 48</b></td>
<td><b>ID 49</b></td>
<td><b>ID 50</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t4011464f706c19cbdb22e4b55c3ac4b7f24f3"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t41114d7534b6e36ddec7dfdab1d3d5253d024"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t4211494a540af34ef9bfcacbc418875cdc3b3"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t4311485daf9747e1af29e633e0053b80939a6"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t44114de0e08265e606f48cd780d2b62f200f6"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t45114829122bc112202834500da5ae8840632"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t46114ffba83b1246d61948fd293f4246fb2b1"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t47114fdd5c27631a63f8ff73a20b2b0b30462"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t481143eaa07c81ab3af29ac39201764fe4051"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t49114cb55573e71e2072c608bb2ec72d9b7b4"></td>
</tr>
</table>
<table>
<tr>
<td><b>ID 51</b></td>
<td><b>ID 52</b></td>
<td><b>ID 53</b></td>
<td><b>ID 54</b></td>
<td><b>ID 55</b></td>
<td><b>ID 56</b></td>
<td><b>ID 57</b></td>
<td><b>ID 58</b></td>
<td><b>ID 59</b></td>
</tr>

<tr>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t5011458504e301449a16b931afcb497b45815"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t5111413a30a2fd700e48a050bc030cb744bcd"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t52114906cb24f16f17822b3826df8ae6fb9d7"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t53114e8080e182dbf0c22738287e09238238a"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t54114637f62f629f3d8ac54b2a930d32dff3c"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t5511438e432e359e9a43138048d3e8902d12e"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t56114798ca79305c0fd595ed80877912f47a8"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t57114746bcce534dcac268f503495e45aaa2b"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/t581147b562ace10a6b993aece8c9651a8e90a"></td>
</tr>
</table>

### Colors

A `Color` is a 2-digit number that represents the color of a badge part. There is 24 different colors in total. Note that not all badge parts can be colored. In that case, any number will return the same default color. An example of a non-colorable badge part is displayed below.

<img src="https://www.habbo.nl/habbo-imaging/badge/t41014935ea23c7318fc7943932593160409e7"> 

### Positions & Layers

A `Position` is a single digit that represents the position of a badge part in your badge. There is 9 different possible positions (0-8), 0 being the upper left corner, 4 being the center and 8 being the bottom right corner. Some bigger badge parts will always be centered, regardless of the set position. A badge demonstrating all possible positions is displayed below.

<img src="https://www.habbo.nl/habbo-imaging/badge/s68010s69011s70012s71013s72014s73015s74016s75017s76018bdd473f066504f3341d056d5a1fb664c">

A badge also has layers. That means that badge parts can overlap other badge parts. A badge part on layer 1 will overlap the part on layer 0, a part on layer 2 will overlap the one on layer 1, etc. What layer a badge part is on, is determined by the order they are in. For example, the order is like this: `[part_a][part_b]`, here, `part_a` is on layer 0, and `part_b` is on layer 1. Layers apply to any type of badge part.

### Example structures

This list of examples demonstrates how to build structures for a badge.

#### Correct structures
<table>
<tr>
<td><b>Image</b></td>
<td><b>Structure</b></td>
<td><b>Explained</b></td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/b0312011748398e35232e4bf1ae3a8b399b947"></td>
<td><code>b</code><code>03</code><code>12</code><code>0</code></td>
<td>A single base part with ID 03, color 12 and position 0</td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/b01200s0610440b349c7c406fb2c9545f7f5f641fd99"></td>
<td><code>b</code><code>01</code><code>20</code><code>0</code><code>s</code><code>06</code><code>10</code><code>4</code></td>
<td>Base 1 with color 20 and 1 additional part with ID 6, color 10 and position 4</td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/b01200s84033s86034s970359be7b0f7040a1f694e08c7307e6feeac"></td>
<td><code>b</code><code>01</code><code>20</code><code>0</code><code>s</code><code>84</code><code>03</code><code>3</code><code>s</code><code>86</code><code>03</code><code>4</code><code>s</code><code>97</code><code>03</code><code>5</code></td>
<td>Same base as above, with 3 additional parts on positions 3, 4 and 5, making the word 'GIT' together</td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/b01030b030303a074ec3f2ab2adb13ee6c4e1833ad62"></td>
<td><code>b</code><code>01</code><code>03</code><code>0</code><code>b</code><code>03</code><code>03</code><code>0</code></td>
<td>Example of a badge with multiple base parts</td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/s84033s86034s9703585d8e114ae901a0051837a76efb46021"></td>
<td><code>s</code><code>84</code><code>03</code><code>3</code><code>s</code><code>86</code><code>03</code><code>4</code><code>s</code><code>97</code><code>03</code><code>5</code></td>
<td>Same as #3, except this badge doesn't have any base parts</td>
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/fc6a5baf8af71b99d1ae37eb24114307"></td>
<td><code></code></td>
<td>Completely empty structure, results into an empty badge</td>
</tr>
</table> 

## Structure hashing

Structure hashing is a more technical matter. How it works exactly is explained in this part of the documentation. A Habbo imaging URL typically looks like: `:server/habbo-imaging/:imageType/:struct:hash`

Where
<table>
<tr>
<td>:server</td>
<td>Is the address of the server. For example https://www.habbo.com</td>
</tr>
<tr>
<td>:imageType</td>
<td>Is the type of image you are requesting. In this case that is 'badge'</td>
</tr>
<tr>
<td>:struct</td>
<td>Is the badge structure that has been explained <a href="https://github.com/notmika/group-badges/blob/master/README.md#badge-structure">here</a></td>
</tr>
<tr>
<td>:hash</td>
<td>Is the result hash of <a href="https://github.com/notmika/group-badges/blob/master/README.md#creating-a-hash">this process</a></td>
</tr>
</table>

### Creating a hash

Before being able to create a valid badge URL, you will need to know that Habbo uses a static "secret" MD5 hash in the process. This hash will be used in combination with a badge structure to create a new hash: `ef2356a4926bf225eb86c75c52309c32`

Formula for creating a valid badge URL: `BADGE_STRUCTURE + MD5(BADGE_STRUCTURE + STATIC_HASH)`

Where
<table>
<tr>
<td>BADGE_STRUCTURE</td>
<td>Is the structure of the badge you want to have returned</td>
</tr>
<tr>
<td>STATIC_HASH</td>
<td>Is <code>ef2356a4926bf225eb86c75c52309c32</code></td>
</tr>
</table>

### C# code example

This is a C# console application that creates and prints a valid badge URL.

```C#
class CreateBadgeHash
{
    static void Main()
    {
        string myStructure = "b10220s06034";
        string staticHash = "ef2356a4926bf225eb86c75c52309c32";

        System.Console.WriteLine(myStructure + CreateMD5(myStructure + staticHash));
    }

    public static string CreateMD5(string input)
    {
        using (System.Security.Cryptography.MD5 md5 = System.Security.Cryptography.MD5.Create())
        {
            byte[] inputBytes = System.Text.Encoding.ASCII.GetBytes(input);
            byte[] hashBytes = md5.ComputeHash(inputBytes);

            System.Text.StringBuilder sb = new System.Text.StringBuilder();
            for (int i = 0; i < hashBytes.Length; i++)
            {
                sb.Append(hashBytes[i].ToString("X2"));
            }
            return sb.ToString();
        }
    }
}
```
