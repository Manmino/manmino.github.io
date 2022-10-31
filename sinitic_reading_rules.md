# Rules for Rendering Sinitic Vocabulary in Manmino

As Sinitic vocabulary comprises a large portion of the common vocabulary of East Asia (especially Northeast Asia), 
and as said vocabulary has been standardized differently among the East Asian languages,
it is important for Manmino to have a unified standard to apply when importing common Sinitic vocabulary.

Considering that the ancestral form to most readings of Sinitic characters stems from early forms of Middle Chinese 
(Middle Chinese being a term for the language spoken during Tang Dynasty to the Song Dynasty),
Manmino uses a reconstructed version of early Middle Chinese phonology called the _Qieyun System_ to derive its own rendition.

In the Qieyun System, character are classified by a variety of factors, such as tone, vowel qualities, and initials.
Below are the 38 categories that are used for classifying the initials, and how Manmino interprets them. Blanks are considered null initials. 

|                     | Tenuis Stop |   | Aspirated Stop |   | Voiced Stop |   | Nasal |   | Tenuis Fricative |   | Voiced Fricative |   | Approximant |   |
| ------------------- | ----------- | - | -------------- | - | ----------- | - | ----- | - | ---------------- | - | ---------------- | - | ----------- | - |
| Labials             | 幫           | b | 滂              | p | 並           | b | 明     | m |                  |   |                  |   |             |   |
| Dentals             | 端           | d | 透              | t | 定           | d | 泥     | n |                  |   |                  |   |             |   |
| Retroflex stops     | 知           | j | 徹              | c | 澄           | j | 娘     | n |                  |   |                  |   |             |   |
| Lateral             |             |   |                |   |             |   |       |   |                  |   |                  |   | 來           | l |
| Dental sibilants    | 精           | j | 清              | c | 從           | j |       |   | 心                | s | 邪                | s |             |   |
| Retroflex sibilants | 莊           | j | 初              | c | 崇           | s |       |   | 生                | s | 俟                | s |             |   |
| Palatals            | 章           | j | 昌              | c | 常           | s | 日     | n | 書                | s | 船                | s | 以           |   |
| Velars              | 見           | g | 溪              | k | 群           | g | 疑     |   |                  |   | 云                |   |             |   |
| Laryngeals          | 影           |   |                |   |             |   |       |   | 曉                | h | 匣                | h |             |   |

The Qieyun System also uses a concept known as division (等) to mark degree of palatalization. 
While it is unclear how this difference was actually realized in Middle Chinese, 
there are enough data points from Sino-xenic readings to rule that for the purposes of rendering Sinitic Vocabulary in Manmino,
Divisions 1 characters are not palatalized at all,
Division 2 characters are not palatalized mostly with only exception for velars,
and Division 3 and 4 characters are always palatalized,
converting dental stops /t/ and /d/ into their palatal approximants /tɕ/ and /dʑ/ counterparts as needed.
The only exception is made for Labials, who are depalatalized before /a/, /w/, or /u/.

Below is the table that show how different interactions between divisions, rounding (referred to being "open" or "closed" by contemporaries), and actual specific vowel-coda combinations all come together to create a specific reading for Manmino. 

| Approx. MC vowel value | 1st Div | ∅   | 1st Div | ^w   | 2nd Div | ∅   | 2nd Div | ^w  | 3rd Div | ∅   | 3rd Div | ^w   | 4th Div | ∅   | 4th Div | ^w  |
| ---------------------- | ------- | --- | ------- | ---- | ------- | --- | ------- | --- | ------- | --- | ------- | ---- | ------- | --- | ------- | --- |
| 果 (a)                | 歌       | a   | 戈       | wa   |         |     |         |     | 戈       | a   | 戈       | wa   |         |     |         |     |
| 假 (a:)               |         |     |         |      | 麻       | a   | 麻       | wa  | 麻       | a   |         |      |         |     |         |     |
| 遇 (ə)                | 模       | o   |         |      |         |     |         |     | 魚       | o   | 虞       | u    |         |     |         |     |
| 蟹 (aj)              | 咍, 泰 | ay  | 灰, 泰  | way  | 皆, 夬, 佳 | ay  | 皆, 夬, 佳 | way | 祭       | ey  | 祭       | wey  | 齊, 祭    | ey  | 齊, 祭 | wey |
| 止 (i)                |         |     |         |      |         |     |         |     | 支, 微, 之 | i   | 支, 微   | wi   |         |     |         |     |
| 止 (i)                 |         |     |         |      |         |     |         |     | 脂       | i   | 脂       | yuy  |         |     |         |     |
| 效 (aw)               | 豪       | aw  |         |      | 肴       | aw  |         |     | 宵       | yaw |         |      | 蕭       | yaw |         |     |
| 流 (əw)                | 侯       | ow  |         |      |         |     |         |     | 尤, 幽   | yu  |         |      |         |     |         |     |
| 咸 (am/p)              | 覃, 談    | am  |         |      | 咸, 銜   | am  |         |     | 鹽, 嚴   | em  | 凡      | om  | 添       | em  |         |     |
| 深 (əm/p)              |         |     |         |      |         |     |         |     | 侵       | im  |         |      |         |     |         |     |
| 山 (an/t)             | 寒     | an  | 桓       | wan  | 山, 刪  | an  | 山, 刪   | wan | 元, 仙    | an  | 元, 仙    | wan  | 仙, 先   | en  | 仙, 先   | wen |
| 臻 (ən/t)              | 痕       | on  | 魂       | on   |         |     |       |     | 臻, 眞, 欣 | in  | 諄, 眞   | yun  |         |     |         |     |
| 臻 (ən/t)              |         |     |         |      |         |     |         |     |        |      | 文       | un   |         |     |         |     |
| 宕 (aŋ/k)             | 唐       | ang | 唐       | wang |         |     |         |     | 陽       | ang | 陽       | wang |         |     |         |     |
| 江 (awŋ/k)             |         |     |         |      | 江       | ang |         |     |         |     |         |      |         |     |         |     |
| 梗 (ajŋ/k)            |         |     |         |      | 庚, 耕    | eng | 庚,耕  | ong | 庚, 清   | eng | 庚, 清    | eng  | 青      |  eng   |  青  | eng  |
| 曾 (əŋ/k)               | 登       | eng | 登       | ong  |         |     |         |     | 蒸       | eng | 蒸       | ong  |         |     |         |   |
| 通 (əwŋ/k)              | 東, 冬   | ong |         |      |         |     |         |     | 東, 鍾   | ong |         |      |         |     |         |     |

As one may observe, the interactions are highly irregular.
