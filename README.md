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
</tr>
<tr>
<td><img src="https://www.habbo.com/habbo-imaging/badge/s010142f93213435a0f8a2ee6e57d326acb761"></td>
<td><img src="https://www.habbo.com/habbo-imaging/badge/s02014077252640988ad6ffbfbe81b9d7caa05"></td>
<td><img src="https://www.habbo.com/habbo-imaging/badge/s030140f7437c1b7f92d36acb53d331a834859"></td>
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
