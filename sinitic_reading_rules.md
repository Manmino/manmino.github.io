# Rules for Rendering Sinitic Vocabulary in Manmino

As Sinitic vocabulary comprises a large portion of the common vocabulary of East Asia (especially Northeast Asia), 
and as said vocabulary has been standardized differently among the East Asian languages,
it is important for Manmino to have a unified standard to apply when importing common Sinitic vocabulary.

Considering that the ancestral form to most readings of Sinitic characters stems from early forms of Middle Chinese 
(Middle Chinese being a term for the language spoken during Tang Dynasty to the Song Dynasty),
Manmino uses a reconstructed version of early Middle Chinese phonology called the _Qieyun System_ to derive its own rendition.

In the Qieyun System, a character is classified by a variety of factors, such as tone, vowel qualities, and initials.
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

This set i

The Qieyun System also uses a concept known as division (等) to mark degree of palatalization. 
While it is unclear how this difference was actually realized in Middle Chinese, there are enough clues that allows 
