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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s0112061f4a7c0ab938117d9b8a2799ee0a058.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s02120ada3212b74cbe49caf606e0e0d70e4eb.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s031207618f6f0ba93034c49259a4928520232.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s04120a3a7a47255e60bef0e037c3eda3bd93c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s051202cf9b05141451e2dac0fdc70ecdebef5.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s06120f2e55a2df2985998b2fe01c4ab088b52.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s07120383e5d99f741d90d2ca3be5968ccf8e3.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s081208214885a23e3a9a577b71134fb38afff.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s091207e93f2f7320b51147a79414ec489bded.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s101205e98bd4927de1b5c5b38b0d3413eb3dc.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s11120d64c1873ba20379b3c4ead15c5bbafc1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s1212078f247c2b7ae76b9f01d9bc4dafd48dd.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s131204a15453c5e16b2b1d97a44d06369aaee.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s141200767ef113c6f2b44b00acda6920cb6b5.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s15120588e87f1333472318a7c06d63451ed51.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s16120b0f28e1db343d0c74515c1ec000bb4ce.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s1712007a27c9fc65cf92cb3b696774af14a53.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s18120251f6c873bf2c508ea7a36e4939aded2.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s19120bbedb5efd605579fb7c04a0ad6456b84.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s20120c5f3e298bddc1a9ab79c7131e42f30d3.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s211202df1b4c826a963ae26c5b128976127fe.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s22120928520d4b2c30277b2778bc56ce9c74f.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s23120133220c00372d63e0de7b936695159d0.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s2412001d73c22a119e802202041c3e4677c25.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s251208a40113994c0f0f3ef65470fe94ff04c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s26120523f1cff021c4ccd5953078c4a0c5ba9.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s2712000fc7b514efbd793434dd2673dc3385a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s28120987f821cfc93b67ec0c743aeb012b202.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s29120cd14ac242164fe1a7dc7d68ddcefffad.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s30120f1a3d013587d85f13892ac658036278c.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s311202f66475cb08233cdd9597b6d4585945c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s32120eb64cdb89ac836c49dbff9a925f3e5cf.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s33120feb3cd1c029bd8d3bcefa88514513436.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s341202cea3f94766563b73c57fe459c1f5bcc.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3512064520b80ebf423e5df37a82acee04847.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3612063ce85a24b5e73b1fc270cf2ea070b6b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s3712016d24003abb6f1a084c65a4c93e6899e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s38120ddd729bc85eb66d6738d2083f7350a83.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s391205878b6baf4f68d3cbba4aadd5db0c870.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s40120f122f212b12a0ea3473a1357dd2218f8.gif"></td>

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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s41120d0c6953308cab6e95811c8903da34800.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s421206d419ad76fd6d21eb16b37dd5b59fd05.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s43120650cb7f3be9f6ae4636dd277eb85dc66.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s441206a8ac74820a484c1144f4dc4884febfe.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s45120ca91b4bd06ec8809cb84b3eca59a5b65.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s46120c7e76e9cc4bf1047319a1cc0864b21c8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s4712051b0b00f70e81a12154da708aff0c723.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s4812058b04c196c48185cfd93d8e258fb9dbe.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s491204fe354bc0dba4af0992acbbcdbce22a9.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s50120099cffcec3c170d1fbbb385e1efbd870.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s511208b1acffab20da495e4807daa0a9d72a7.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s52120f49add513c2bc35c2c68b07929710d4a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s531200a290b0e1cb80bd70326031fa2eafc06.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s54120804345cf0fc14217e7495d5be7b49b92.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s55120814c758d148d5a710fe20710c80c0806.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s56120f5c38515e12861af1f62402f4fb4fba5.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s5712029db7c4c6a3cea502db20b34cb4aca5d.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s581200a750329c51538f52ad0055c79c72eb1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s5912060a83647ef5f1032258853021d968e95.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s6012073017a6e770fe625de9f422929ddc421.gif"></td>

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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s61120554a68021464d12373403b87c14e24b1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s62120f7bc82e48e15234aeb46b1b27d05f929.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s631208c77e92110e2b6cb817415dec8ab3fb2.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s641200c2f0fa765f1c4f901c0035c992813de.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s65120813dc417341386b1a8c9594c4ba2c857.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s66120eb7d0df6d87443d8dc408a3759f8f781.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s671207e3b27cc6f40626ffe1e5616923069bc.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s68120a6a7ebc6be83ba054399bc29275d9b44.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s691204c3c7d33e2dc6091d709e01652df0991.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s701203de0a3565438dbe1147853c196cd09c3.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s711201affa62fb8d0e1f90659ea2d96927af8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s72120f16fa6e8039910dc07bed52e42111787.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s73120a0df2047e9607c073aa6b211b0f57184.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s7412028158c30d7eba38d2bc9d445fc0ad3f8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s751209b103ff2970b5bffba6debe4da02841a.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s76120333ef08ae8700e860cdeb190d24d7c8d.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s77120527b0ac230e78598720731da69335b18.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s781206c146d80f62e105ad73c5e494c4b2085.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s79120dbfb42d6b04b7c5e47187102f50e26aa.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s80120202d91f1031461e2b08c6cd6b49614f7.gif"></td>

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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s811209b22b9ef35160086271952a742120a77.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s8212063217a5734ca0f32f493e9b74062aa88.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s83120224ea0d63108620c058be4292a35038c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s84120ada2c4cb152057c1484a02abf598ad9b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s8512013fd3100bcba34753c13e054f40a0c94.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s86120d0ac6fa26a178f35546c0f2c15756871.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s87120c90c501b2519352b48dac92b75afb61b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s88120fe1f59bed1db62fc84975623eff8e004.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s89120ebbabb6c67edc5d627f4894a3a361fd8.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s90120ededf38f228f0233a292ae94141ecc75.gif"></td>
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
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s911206fbc5f8929c02a2da86fe96855022f93.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s9212058a60c5b91a93918b92388305d0fab2e.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s9312044fc5c5d7c338ee6d544dfdd6d180613.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s941204618fdd8ed680205c5d34aee67cf2c8b.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s95120a04cb8b744683bede05fcd66bdedf25c.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s961207a61380557e6ef992be94a0b6fcd60ce.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s97120dd9fde483a087866ba02c29ed3ef5d96.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s98120ad50200599abcba289ebd2d5c1d6f4b1.gif"></td>
<td><img src="https://www.habbo.nl/habbo-imaging/badge/s99120b2c944403cfb751f19161949c4ac8aed.gif"></td>

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
