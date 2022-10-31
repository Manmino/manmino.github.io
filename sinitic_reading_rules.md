1. [Rules for Rendering Sinitic Vocabulary in Manmino](https://github.com/Manmino/manmino.github.io/blob/main/sinitic_reading_rules.md#Rules-for-Rendering-Sinitic-Vocabulary-in-Manmino)
2. [만민어 한자음 표기법](https://github.com/Manmino/manmino.github.io/blob/main/sinitic_reading_rules.md#만민어-한자음-표기법)

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
The only exception is made for Labials, who are depalatalized before /a/ or /u/.

Below is the table that show how different interactions between divisions, rounding (referred to being "open" or "closed" by contemporaries), and actual specific vowel-coda combinations all come together to create a specific reading for Manmino. 

| MC vowel value (reconstructed) | 1st Div | ∅   | 1st Div | ^w   | 2nd Div | ∅   | 2nd Div | ^w  | 3rd Div | ∅   | 3rd Div | ^w   | 4th Div | ∅   | 4th Div | ^w  |
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

As one may observe, the interactions are highly irregular due to there being no concensus on how to reunite the vowels among various Sino-Xenic readings: 
Generally, finals with /\*a/ vowels were rendered as /a/.
If they were palatalized both before and after the nucleus, they were instead rendered as /ja/ or /e/.
If they were rounded vowels, /wa/, /we/, /e/, /o/, were all considered as options, based on a rough analysis of descendant readings.
Similarly, finals with /\*ə/ vowels were rendered as /o/ or /e/, 
but the combination of palatalization and rounding resulted in there being no one pattern: they too were rendered based on a rough analysis of descendant readings.
The values provided in this table may not match what is on the dictionary, 
as exceptions are made for individual characters at the moment.
This document may be subject to change as we get more community feedback on how our Sino-Xenic vocabulary should sound.




# 만민어 한자음 표기법

한자 기반 어휘가 동양 공용 어휘의 상당 부분 차지 하지만 (특히 동북아시아에서),
각 동양 언어마다 해당 어휘의 발음이 서로 다르게 표준화 되었기에,
만민어에서 한자 기반 어휘를 표기할 때 단일화 된 표준을 따라 표기 하는게 중요하다.

현대 대부분의 한자 독법은 초기 중고한어에서 온 점을 고려해서
(여기서 중고한어는 당나라 시대 부터 송나라 시대에 쓰이던 언어를 뜻한다),
만민어는 초기 중고한어의 음운을 다루는 운서들중 "절운" 계열 운서들을 기반으로 한 재구를 통해 표기법을 마련했다.

절운 계열 시스템에서 각 한자는 성조, 모음 성질, 성모(聲母)등에 따라 정리된다.
다음은 38가지 성모의 분류 및 각 성모의 만민어 독법이다. 빈 공간은 성모 자음이 없는것으로 간주한다.

|                     | 무기음 |   | 유기음 |   | 유성음 |   | 비음 |   | 무기 마찰음 |   | 유기 마찰음 |   | 접근음 |   |
| ------------------- | ----------- | - | -------------- | - | ----------- | - | ----- | - | ---------------- | - | ---------------- | - | ----------- | - |
| 순음                | 幫           | b | 滂             | p | 並          | b | 明     | m |                  |   |                  |   |             |   |
| 치경 파열음    | 端           | d | 透              | t | 定           | d | 泥     | n |                  |   |                  |   |             |   |
| 권설 파열음    | 知           | j | 徹              | c | 澄           | j | 娘     | n |                  |   |                  |   |             |   |
| 측음          |             |   |                |   |             |   |       |   |                  |   |                  |   | 來           | l |
| 치경 파찰음    | 精           | j | 清              | c | 從           | j |       |   | 心                | s | 邪                | s |             |   |
| 권설 파찰음    | 莊           | j | 初              | c | 崇           | s |       |   | 生                | s | 俟                | s |             |   |
| 경구개음       | 章           | j | 昌              | c | 常           | s | 日     | n | 書                | s | 船                | s | 以           |   |
| 연구개음       | 見           | g | 溪              | k | 群           | g | 疑     |   |                  |   | 云                |   |             |   |
| 후음           | 影           |   |                |   |             |   |       |   | 曉                | h | 匣                | h |             |   |

절운 계열 시스템은 또한 등(等)이라는 개념을 통해 경구개음화의 정도를 표한다.
이게 실제 중고한어에서 어떻게 발현 되었는지 불분명하지만
각국 독음을 분석한 결과 만민어 한자음을 유측할 때 다음 규칙을 따르라 할 수 있다:
1등은 경구개화를 전혀 진행하지 않고,
2등은 연구개음 외에는 경구개화를 진행하지 않고,
3등 과 4등은 늘 경구개화를 진행하며
치경 파열음 /t/ 및 /d/는 각각 치경 파찰음 /tɕ/ 이나 /dʑ/ 으로 변이된다.
이에 순음은 예외인데, 순음 뒤 모음이 /a/나 /u/ 가 오는 경우 경구개화를 진행하지 않는다.

다음 표는 각 등, 원순화 (절운에서는 개합 - 開合), 그리고 모음-어말자음 집합이 서로 상호작용해 어떻게 만민어에서 읽는지 표한다.

| 중고한어 모음 값 (재구) | 1等 | ∅   | 1等 | ^w   | 2等 | ∅   | 2等 | ^w  | 3等 | ∅   | 3等 | ^w   | 4等 | ∅   | 4等 | ^w  |
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
| 山 (an/t)             | 寒     | an  | 桓      | wan  | 山, 刪  | an  | 山, 刪   | wan | 元, 仙    | an  | 元, 仙    | wan  | 仙, 先   | en  | 仙, 先   | wen |
| 臻 (ən/t)              | 痕       | on  | 魂       | on   |        |     |       |     | 臻, 眞, 欣 | in  | 諄, 眞   | yun  |         |     |         |     |
| 臻 (ən/t)              |         |     |         |      |         |     |         |     |        |      | 文       | un   |         |     |         |     |
| 宕 (aŋ/k)             | 唐       | ang | 唐       | wang |         |     |         |     | 陽       | ang | 陽       | wang |         |     |         |     |
| 江 (awŋ/k)             |         |     |         |      | 江       | ang |         |     |         |     |         |      |         |     |         |     |
| 梗 (ajŋ/k)            |         |     |         |      | 庚, 耕    | eng | 庚,耕  | ong | 庚, 清   | eng | 庚, 清    | eng  | 青      |  eng   |  青  | eng  |
| 曾 (əŋ/k)               | 登       | eng | 登       | ong  |         |     |         |     | 蒸       | eng | 蒸       | ong  |         |     |         |   |
| 通 (əwŋ/k)              | 東, 冬   | ong |         |      |         |     |         |     | 東, 鍾   | ong |         |      |         |     |         |     |

보이듯이, 서로 상호작용 해서 결정된 만민어 독음이 상당히 불규칙 적이다. 이는 각국 한자 독음들의 모음을 어떻게 통합할지 합의 하기 어렵기 때문이다.
운모중 /\*a/를 주 모음으로 하는 문자들은 일반적으로 만민어로도 /a/로 읽힌다.
다만, 모음 전후로 경구개화가 진행된 경우에는 /ja/ 나 /e/로 읽힌다.
모음 원순화가 진행된 경우에는 /wa/, /we/, /e/, /o/ 등으로 읽히며, 이는 특정 규칙을 따르기 보다는 후대 독음법들를 개략적 분석해 정했다.
비슷하게, 운모중 /\*ə/를 주 모음으로 하는 문자들은 일반적으로 /o/ 나 /e/ 로 읽히되,
원순화와 경구개화가 적용되는 경우에는 특정한 규칙을 찾기 힘들었다. 따라서 이들도 후대 독음법들을 개략적으로 분석해 정했다.
이 표에 있는 값이 사전에 등재된 단어와 어긋 나 있을 수 있으며,
이는 현재 때때로 각 글자마다 예외 독음을 지정하고 있는 중이기 때문이다. 
이 문서 또한 만민어 커뮤니티에서 한자 기반 어휘의 독음에 대한 개정안을 재시하는 대로 변경 될 수 있다. 
