# fcitx-LaTeX-quick-input

帮助您在Fcitx中使用LaTeX符号(例如: `\leq`)输入Unicode特殊字符(例如`≤`). 如果您不希望输入`\`(即输入`leq`获得`≤`), 请在安装时选择`QuickPhraseWithout.mb`而非`QuickPhrase.mb`

### 安装

- 终端执行 
  ```bash
  curl -#C - -O https://raw.githubusercontent.com/KairuiLiu/fcitx-LaTeX-quick-input/master/QuickPhrase.mb && cat ./QuickPhrase.mb >> ~/.config/fcitx/data/QuickPhrase.mb && rm ./QuickPhrase.mb
  ```
- 或者将项目中的`QuickPhrase*.mb`文件放置到`~/.config/fcitx/data/QuickPhrase.mb`目录下.  
  如果`~/.config/fcitx/data/QuickPhrase.mb`中已有内容, 可将下载的`QuickPhrase.mb`的内容与之合并.

### 使用

fcitx的输入法激活状态下

1.  按下分号`;`(默认的按键是分号, 也可在fcitx设置-附加组件-快速输入中修改)
2.  输入表情的名字即可看到提示, 按需选用即可

### Unicode-LaTeX对照表

[Unicode对照表来源](http://milde.users.sourceforge.net/LUCR/Math/unimathsymbols.html#latin-extended-a)

#### 数学运算符

| Unicode编码 | LaTeX公式         | Unicode编码 | LaTeX公式         |
| ----------- | ----------------- | ----------- | ----------------- |
| ∀           | \forall           | ≽           | \succcurlyeq      |
| ∁           | \complement       | ≾           | \precsim          |
| ∂           | \partial          | ≿           | \succsim          |
| ∃           | \exists           | ⊀           | \nprec            |
| ∄           | \nexists          | ⊁           | \nsucc            |
| ∅           | \varnothing       | ⊂           | \subset           |
| ∇           | \nabla            | ⊃           | \supset           |
| ∈           | \in               | ⊄           | \nsubset          |
| ∉           | \notin            | ⊅           | \nsupset          |
| ∋           | \ni               | ⊆           | \subseteq         |
| ∌           | \nni              | ⊇           | \supseteq         |
| ∏           | \prod             | ⊈           | \nsubseteq        |
| ∐           | \coprod           | ⊉           | \nsupseteq        |
| ∑           | \sum              | ⊊           | \subsetneq        |
| −           | -                 | ⊋           | \supsetneq        |
| ∓           | \mp               | ⊎           | \uplus            |
| ∔           | \dotplus          | ⊏           | \sqsubset         |
| ∕           | \slash            | ⊐           | \sqsupset         |
| ∖           | \smallsetminus    | ⊑           | \sqsubseteq       |
| ∗           | \ast              | ⊒           | \sqsupseteq       |
| ∘           | \circ             | ⊓           | \sqcap            |
| ∙           | \bullet           | ⊔           | \sqcup            |
| √           | \sqrt             | ⊕           | \oplus            |
| ∛           | \sqrt[3]          | ⊖           | \ominus           |
| ∜           | \sqrt[4]          | ⊗           | \otimes           |
| ∝           | \propto           | ⊘           | \oslash           |
| ∞           | \infty            | ⊙           | \odot             |
| ∟           | \rightangle       | ⊚           | \circledcirc      |
| ∠           | \angle            | ⊛           | \circledast       |
| ∡           | \measuredangle    | ⊝           | \circleddash      |
| ∢           | \sphericalangle   | ⊞           | \boxplus          |
| ∣           | \mid              | ⊟           | \boxminus         |
| ∤           | \nmid             | ⊠           | \boxtimes         |
| ∥           | \parallel         | ⊡           | \boxdot           |
| ∦           | \nparallel        | ⊢           | \vdash            |
| ∧           | \wedge            | ⊣           | \dashv            |
| ∨           | \vee              | ⊤           | \top              |
| ∩           | \cap              | ⊥           | \bot              |
| ∪           | \cup              | ⊧           | \models           |
| ∫           | \int              | ⊨           | \vDash            |
| ∬           | \iint             | ⊩           | \Vdash            |
| ∭           | \iiint            | ⊪           | \Vvdash           |
| ∮           | \oint             | ⊫           | \VDash            |
| ∯           | \oiint            | ⊬           | \nvdash           |
| ∰           | \oiiint           | ⊭           | \nvDash           |
| ∲           | \varointclockwise | ⊮           | \nVdash           |
| ∳           | \ointctrclockwise | ⊯           | \nVDash           |
| ∴           | \therefore        | ⊲           | \vartriangleleft  |
| ∵           | \because          | ⊳           | \vartriangleright |
| ∷           | \Proportion       | ⊴           | \trianglelefteq   |
| ∹           | \eqcolon          | ⊵           | \trianglerighteq  |
| ∼           | \sim              | ⊶           | \multimapdotbothA |
| ∽           | \backsim          | ⊷           | \multimapdotbothB |
| ∿           | \AC               | ⊸           | \multimap         |
| ≀           | \wr               | ⊺           | \intercal         |
| ≁           | \nsim             | ⊻           | \veebar           |
| ≂           | \eqsim            | ⊼           | \barwedge         |
| ≃           | \simeq            | ⋀           | \bigwedge         |
| ≄           | \nsimeq           | ⋁           | \bigvee           |
| ≅           | \cong             | ⋂           | \bigcap           |
| ≇           | \ncong            | ⋃           | \bigcup           |
| ≈           | \approx           | ⋄           | \diamond          |
| ≉           | \napprox          | ⋅           | \cdot             |
| ≊           | \approxeq         | ⋆           | \star             |
| ≍           | \asymp            | ⋇           | \divideontimes    |
| ≎           | \Bumpeq           | ⋈           | \bowtie           |
| ≏           | \bumpeq           | ⋉           | \ltimes           |
| ≐           | \doteq            | ⋊           | \rtimes           |
| ≑           | \Doteq            | ⋋           | \leftthreetimes   |
| ≒           | \fallingdotseq    | ⋌           | \rightthreetimes  |
| ≓           | \risingdotseq     | ⋍           | \backsimeq        |
| ≔           | \coloneq          | ⋎           | \curlyvee         |
| ≕           | \eqcolon          | ⋏           | \curlywedge       |
| ≖           | \eqcirc           | ⋐           | \Subset           |
| ≗           | \circeq           | ⋑           | \Supset           |
| ≙           | \corresponds      | ⋒           | \Cap              |
| ≜           | \triangleq        | ⋓           | \Cup              |
| ≠           | \neq              | ⋔           | \pitchfork        |
| ≡           | \equiv            | ⋕           | \hash             |
| ≢           | \nequiv           | ⋖           | \lessdot          |
| ≤           | \leq              | ⋗           | \gtrdot           |
| ≥           | \geq              | ⋘           | \lll              |
| ≦           | \leqq             | ⋙           | \ggg              |
| ≧           | \geqq             | ⋚           | \lesseqgtr        |
| ≨           | \lneqq            | ⋛           | \gtreqless        |
| ≩           | \gneqq            | ⋞           | \curlyeqprec      |
| ≪           | \ll               | ⋟           | \curlyeqsucc      |
| ≫           | \gg               | ⋠           | \npreceq          |
| ≬           | \between          | ⋡           | \nsucceq          |
| ≭           | \notasymp         | ⋢           | \nsqsubseteq      |
| ≮           | \nless            | ⋣           | \nsqsupseteq      |
| ≯           | \ngtr             | ⋦           | \lnsim            |
| ≰           | \nleq             | ⋧           | \gnsim            |
| ≱           | \ngeq             | ⋨           | \precnsim         |
| ≲           | \lesssim          | ⋩           | \succnsim         |
| ≳           | \gtrsim           | ⋪           | \ntriangleleft    |
| ≴           | \NotLessTilde     | ⋫           | \ntriangleright   |
| ≵           | \NotGreaterTilde  | ⋬           | \ntrianglelefteq  |
| ≶           | \lessgtr          | ⋭           | \ntrianglerighteq |
| ≷           | \gtrless          | ⋮           | \vdots            |
| ≹           | \NotGreaterLess   | ⋯           | \cdots            |
| ≺           | \prec             | ⋰           | \iddots           |
| ≻           | \succ             | ⋱           | \ddots            |
| ≼           | \preccurlyeq      | ⋶           | \barin            |






#### 希腊语和科普特语

| Unicode编码 | LaTeX公式   | Unicode编码 | LaTeX公式    |
| ----------- | ----------- | ----------- | ------------ |
| Γ           | \Gamma      | ς           | \varsigma    |
| Δ           | \Delta      | σ           | \sigma       |
| Θ           | \Theta      | τ           | \tau         |
| Λ           | \Lambda     | υ           | \upsilon     |
| Ξ           | \Xi         | φ           | \varphi      |
| Π           | \Pi         | χ           | \chi         |
| Σ           | \Sigma      | ψ           | \psi         |
| Υ           | \Upsilon    | ω           | \omega       |
| Φ           | \Phi        | ϐ           | \varbeta     |
| Ψ           | \Psi        | ϑ           | \vartheta    |
| Ω           | \Omega      | ϕ           | \phi         |
| α           | \alpha      | ϖ           | \varpi       |
| β           | \beta       | Ϙ           | \Qoppa       |
| γ           | \gamma      | ϙ           | \qoppa       |
| δ           | \delta      | Ϛ           | \Stigma      |
| ε           | \varepsilon | ϛ           | \stigma      |
| ζ           | \zeta       | Ϝ           | \Digamma     |
| η           | \eta        | ϝ           | \digamma     |
| θ           | \theta      | Ϟ           | \Koppa       |
| ι           | \iota       | ϟ           | \koppa       |
| κ           | \kappa      | Ϡ           | \Sampi       |
| λ           | \lambda     | ϡ           | \sampi       |
| μ           | \mu         | ϰ           | \varkappa    |
| ν           | \nu         | ϱ           | \varrho      |
| ξ           | \xi         | ϵ           | \epsilon     |
| π           | \pi         | ϶           | \backepsilon |
| ρ           | \rho        |             |              |

#### 字母符号

| Unicode编码 | LaTeX公式    | Unicode编码 | LaTeX公式             |
| ----------- | ------------ | ----------- | --------------------- |
| ℂ           | \mathbb{C}   | ℭ           | \mathfrak{C}          |
| ℇ           | \Euler       | ℯ           | \mathcal{e}           |
| ℊ           | \mathcal{g}  | ℰ           | \mathcal{E}           |
| ℋ           | \mathcal{H}  | ℱ           | \mathcal{F}           |
| ℌ           | \mathfrak{H} | Ⅎ           | \Finv                 |
| ℍ           | \mathbb{H}   | ℳ           | \mathcal{M}           |
| ℏ           | \hslash      | ℴ           | \mathcal{o}           |
| ℐ           | \mathcal{I}  | ℵ           | \aleph                |
| ℑ           | \Im          | ℶ           | \beth                 |
| ℒ           | \mathcal{L}  | ℷ           | \gimel                |
| ℓ           | \ell         | ℸ           | \daleth               |
| ℕ           | \mathbb{N}   | ℼ           | \mathbb{pi}           |
| ℘           | \wp          | ℽ           | \mathbb{gamma}        |
| ℙ           | \mathbb{P}   | ℾ           | \mathbb{Gamma}        |
| ℚ           | \mathbb{Q}   | ℿ           | \mathbb{Pi}           |
| ℛ           | \mathcal{R}  | ⅀           | \mathbb{Sigma}        |
| ℜ           | \Re          | ⅄           | \Yup                  |
| ℝ           | \mathbb{R}   | ⅅ           | \CapitalDifferentialD |
| ℤ           | \mathbb{Z}   | ⅆ           | \DifferentialD        |
| Ω           | \tcohm       | ⅇ           | \ExponetialE          |
| ℧           | \mho         | ⅈ           | \ComplexI             |
| ℨ           | \mathfrak{Z} | ⅉ           | \ComplexJ             |
| Å           | \Angstroem   | ⅋           | \invamp               |
| ℬ           | \mathcal{B}  |             |                       |

#### 箭头

| Unicode编码 | LaTeX公式            | Unicode编码 | LaTeX公式               |
| ----------- | -------------------- | ----------- | ----------------------- |
| ←           | \leftarrow           | ⇁           | \rightharpoondown       |
| ↑           | \uparrow             | ⇂           | \downharpoonright       |
| →           | \rightarrow          | ⇃           | \downharpoonleft        |
| ↓           | \downarrow           | ⇄           | \rightleftarrows        |
| ↔           | \leftrightarrow      | ⇅           | \updownarrows           |
| ↕           | \updownarrow         | ⇆           | \leftrightarrows        |
| ↖           | \nwarrow             | ⇇           | \leftleftarrows         |
| ↗           | \nearrow             | ⇈           | \upuparrows             |
| ↘           | \searrow             | ⇉           | \rightrightarrows       |
| ↙           | \swarrow             | ⇊           | \downdownarrows         |
| ↚           | \nleftarrow          | ⇋           | \leftrightharpoons      |
| ↛           | \nrightarrow         | ⇌           | \rightleftharpoons      |
| ↞           | \twoheadleftarrow    | ⇍           | \nLeftarrow             |
| ↠           | \twoheadrightarrow   | ⇎           | \nLeftrightarrow        |
| ↢           | \leftarrowtail       | ⇏           | \nRightarrow            |
| ↣           | \rightarrowtail      | ⇐           | \Leftarrow              |
| ↤           | \mapsfrom            | ⇑           | \Uparrow                |
| ↥           | \MapsUp              | ⇒           | \Rightarrow             |
| ↦           | \mapsto              | ⇓           | \Downarrow              |
| ↧           | \MapsDown            | ⇔           | \Leftrightarrow         |
| ↩           | \hookleftarrow       | ⇕           | \Updownarrow            |
| ↪           | \hookrightarrow      | ⇖           | \Nwarrow                |
| ↫           | \looparrowleft       | ⇗           | \Nearrow                |
| ↬           | \looparrowright      | ⇘           | \Searrow                |
| ↭           | \leftrightsquigarrow | ⇙           | \Swarrow                |
| ↮           | \nleftrightarrow     | ⇚           | \Lleftarrow             |
| ↯           | \lightning           | ⇛           | \Rrightarrow            |
| ↰           | \Lsh                 | ⇜           | \leftsquigarrow         |
| ↱           | \Rsh                 | ⇝           | \rightsquigarrow        |
| ↲           | \dlsh                | ⇠           | \dashleftarrow          |
| ↳           | \drsh                | ⇢           | \dashrightarrow         |
| ↶           | \curvearrowleft      | ⇤           | \LeftArrowBar           |
| ↷           | \curvearrowright     | ⇥           | \RightArrowBar          |
| ↺           | \circlearrowleft     | ⇵           | \downuparrows           |
| ↻           | \circlearrowright    | ⇸           | \pfun                   |
| ↼           | \leftharpoonup       | ⇻           | \ffun                   |
| ↽           | \leftharpoondown     | ⇽           | \leftarrowtriangle      |
| ↾           | \upharpoonright      | ⇾           | \rightarrowtriangle     |
| ↿           | \upharpoonleft       | ⇿           | \leftrightarrowtriangle |
| ⇀           | \rightharpoonup      |             |                         |

#### 拉丁语1

| Unicode编码 | LaTeX公式 | Unicode编码 | LaTeX公式 |
| ----------- | --------- | ----------- | --------- |
| ¢           | \cent     | ±           | \pm       |
| £           | \pounds   | µ           | \Micro    |
| ¥           | \yen      | ×           | \times    |
| ¨           | \spddot   | ð           | \eth      |
| ¬           | \neg      | ÷           | \div      |
| ®           | \circledR |             |           |

#### 组合变音符

| Unicode编码 | LaTeX公式 | Unicode编码 | LaTeX公式  |
| ----------- | --------- | ----------- | ---------- |
| ̀            | \grave    | ̈            | \ddot      |
| ́            | \acute    | ̊            | \mathring  |
| ̂            | \hat      | ̌            | \check     |
| ̃            | \tilde    | ̰            | \utilde    |
| ̄            | \bar      | ̱            | \underbar  |
| ̅            | \overline | ̲            | \underline |
| ̆            | \breve    | ̸            | \not       |
| ̇            | \dot      |             |            |

#### 一般标点

| Unicode编码 | LaTeX公式 | Unicode编码 | LaTeX公式  |
| ----------- | --------- | ----------- | ---------- |
| ‖           | \|        | ″           | \second    |
| †           | \dagger   | ‴           | \third     |
| ‡           | \ddagger  | ‵           | \backprime |
| •           | \bullet   | ⁀           | \cat       |
| …           | \ldots    | ⁗           | \fourth    |
| ′           | \prime    |             |            |

#### 其他技术

| Unicode编码 | LaTeX公式    | Unicode编码 | LaTeX公式         |
| ----------- | ------------ | ----------- | ----------------- |
| ⌀           | \diameter    | ⌿           | \notslash         |
| ⌈           | \lceil       | ⍀           | \notbackslash     |
| ⌉           | \rceil       | ⍇           | \APLleftarrowbox  |
| ⌊           | \lfloor      | ⍈           | \APLrightarrowbox |
| ⌋           | \rfloor      | ⍉           | \invdiameter      |
| ⌐           | \invneg      | ⍐           | \APLuparrowbox    |
| ⌑           | \wasylozenge | ⍗           | \APLdownarrowbox  |
| ⌜           | \ulcorner    | ⍝           | \APLcomment       |
| ⌝           | \urcorner    | ⍞           | \APLinput         |
| ⌞           | \llcorner    | ⍟           | \APLlog           |
| ⌟           | \lrcorner    | ⏜           | \overparen        |
| ⌢           | \frown       | ⏝           | \underparen       |
| ⌣           | \smile       | ⏞           | \overbrace        |
| ⌹           | \APLinv      | ⏟           | \underbrace       |

#### 几何形状

| Unicode编码 | LaTeX公式           | Unicode编码 | LaTeX公式          |
| ----------- | ------------------- | ----------- | ------------------ |
| △           | \bigtriangleup      | ◃           | \smalltriangleleft |
| ▴           | \blacktriangleup    | ◆           | \Diamondblack      |
| ▵           | \smalltriangleup    | ◇           | \Diamond           |
| ▶           | \RHD                | ◊           | \lozenge           |
| ▷           | \rhd                | ○           | \Circle            |
| ▸           | \blacktriangleright | ●           | \CIRCLE            |
| ▹           | \smalltriangleright | ◐           | \LEFTcircle        |
| ▽           | \bigtriangledown    | ◑           | \RIGHTcircle       |
| ▾           | \blacktriangledown  | ◖           | \LEFTCIRCLE        |
| ▿           | \smalltriangledown  | ◗           | \RIGHTCIRCLE       |
| ◀           | \LHD                | ◫           | \boxbar            |
| ◁           | \lhd                | ◻           | \square            |
| ◂           | \blacktriangleleft  | ◼           | \blacksquare       |

#### 杂项符号

| Unicode编码 | LaTeX公式    | Unicode编码 | LaTeX公式       |
| ----------- | ------------ | ----------- | --------------- |
| ★           | \bigstar     | ♌           | \leo            |
| ☉           | \Sun         | ♍           | \virgo          |
| ☐           | \Square      | ♎           | \libra          |
| ☑           | \CheckedBox  | ♏           | \scorpio        |
| ☒           | \XBox        | ♐           | \sagittarius    |
| ☕           | \steaming    | ♑           | \capricornus    |
| ☞           | \pointright  | ♒           | \aquarius       |
| ☠           | \skull       | ♓           | \pisces         |
| ☢           | \radiation   | ♠           | \spadesuit      |
| ☣           | \biohazard   | ♡           | \heartsuit      |
| ☯           | \yinyang     | ♢           | \diamondsuit    |
| ☹           | \frownie     | ♣           | \clubsuit       |
| ☺           | \smiley      | ♤           | \varspadesuit   |
| ☻           | \blacksmiley | ♥           | \varheartsuit   |
| ☼           | \sun         | ♦           | \vardiamondsuit |
| ☽           | \rightmoon   | ♧           | \varclubsuit    |
| ☾           | \leftmoon    | ♩           | \quarternote    |
| ☿           | \mercury     | ♪           | \eighthnote     |
| ♀           | \female      | ♫           | \twonotes       |
| ♁           | \earth       | ♬           | \sixteenthnote  |
| ♂           | \male        | ♭           | \flat           |
| ♃           | \jupiter     | ♮           | \natural        |
| ♄           | \saturn      | ♯           | \sharp          |
| ♅           | \uranus      | ♻           | \recycle        |
| ♆           | \neptune     | ⚓           | \anchor         |
| ♇           | \pluto       | ⚔           | \swords         |
| ♈           | \aries       | ⚠           | \warning        |
| ♉           | \taurus      | ⚪           | \medcirc        |
| ♊           | \gemini      | ⚫           | \medbullet      |
| ♋           | \cancer      |             |                 |

#### 装饰物

| Unicode编码 | LaTeX公式  | Unicode编码 | LaTeX公式    |
| ----------- | ---------- | ----------- | ------------ |
| ✎           | \pencil    | ✠           | \maltese     |
| ✓           | \checkmark | ➢           | \arrowbullet |
| ✗           | \ballotx   |             |              |

#### 杂项数学符号-A

| Unicode编码 | LaTeX公式    | Unicode编码 | LaTeX公式 |
| ----------- | ------------ | ----------- | --------- |
| ⟂           | \perp        | ⟨           | \langle   |
| ⟅           | \Lbag        | ⟩           | \rangle   |
| ⟆           | \Rbag        | ⟪           | \lang     |
| ⟐           | \Diamonddot  | ⟫           | \rang     |
| ⟜           | \multimapinv | ⟮           | \lgroup   |
| ⟦           | \llbracket   | ⟯           | \rgroup   |
| ⟧           | \rrbracket   |             |           |

#### 补充箭头-A

| Unicode编码 | LaTeX公式           | Unicode编码 | LaTeX公式           |
| ----------- | ------------------- | ----------- | ------------------- |
| ⟵           | \longleftarrow      | ⟺           | \Longleftrightarrow |
| ⟶           | \longrightarrow     | ⟻           | \longmapsfrom       |
| ⟷           | \longleftrightarrow | ⟼           | \longmapsto         |
| ⟸           | \Longleftarrow      | ⟽           | \Longmapsfrom       |
| ⟹           | \Longrightarrow     | ⟾           | \Longmapsto         |

#### 补充箭头-B

| Unicode编码 | LaTeX公式             | Unicode编码 | LaTeX公式           |
| ----------- | --------------------- | ----------- | ------------------- |
| ⤀           | \psur                 | ⥙           | \LeftDownVectorBar  |
| ⤆           | \Mapsfrom             | ⥚           | \LeftTeeVector      |
| ⤇           | \Mapsto               | ⥛           | \RightTeeVector     |
| ⤒           | \UpArrowBar           | ⥜           | \RightUpTeeVector   |
| ⤓           | \DownArrowBar         | ⥝           | \RightDownTeeVector |
| ⤔           | \pinj                 | ⥞           | \DownLeftTeeVector  |
| ⤕           | \finj                 | ⥟           | \DownRightTeeVector |
| ⤖           | \bij                  | ⥠           | \LeftUpTeeVector    |
| ⤳           | \leadsto              | ⥡           | \LeftDownTeeVector  |
| ⥊           | \leftrightharpoon     | ⥢           | \leftleftharpoons   |
| ⥋           | \rightleftharpoon     | ⥣           | \upupharpoons       |
| ⥎           | \leftrightharpoonup   | ⥤           | \rightrightharpoons |
| ⥏           | \rightupdownharpoon   | ⥥           | \downdownharpoons   |
| ⥐           | \leftrightharpoondown | ⥪           | \leftbarharpoon     |
| ⥑           | \leftupdownharpoon    | ⥫           | \barleftharpoon     |
| ⥒           | \LeftVectorBar        | ⥬           | \rightbarharpoon    |
| ⥓           | \RightVectorBar       | ⥭           | \barrightharpoon    |
| ⥔           | \RightUpVectorBar     | ⥮           | \updownharpoons     |
| ⥕           | \RightDownVectorBar   | ⥯           | \downupharpoons     |
| ⥖           | \DownLeftVectorBar    | ⥼           | \strictfi           |
| ⥗           | \DownRightVectorBar   | ⥽           | \strictif           |
| ⥘           | \LeftUpVectorBar      |             |                     |

#### 杂项数学符号-B

| Unicode编码 | LaTeX公式      | Unicode编码 | LaTeX公式         |
| ----------- | -------------- | ----------- | ----------------- |
| ⦀           | \VERT          | ⧄           | \boxslash         |
| ⦁           | \spot          | ⧅           | \boxbslash        |
| ⦅           | \Lparen        | ⧆           | \boxast           |
| ⦆           | \Rparen        | ⧇           | \boxcircle        |
| ⦇           | \limg          | ⧈           | \boxbox           |
| ⦈           | \rimg          | ⧏           | \LeftTriangleBar  |
| ⦉           | \lblot         | ⧐           | \RightTriangleBar |
| ⦊           | \rblot         | ⧟           | \multimapboth     |
| ⦸           | \circledbslash | ⧫           | \blacklozenge     |
| ⧀           | \circledless   | ⧵           | \setminus         |
| ⧁           | \circledgtr    | ⧹           | \zhide            |

#### 补充数学运算符

| Unicode编码 | LaTeX公式       | Unicode编码 | LaTeX公式             |
| ----------- | --------------- | ----------- | --------------------- |
| ⨀           | \bigodot        | ⪊           | \gnapprox             |
| ⨁           | \bigoplus       | ⪋           | \lesseqqgtr           |
| ⨂           | \bigotimes      | ⪌           | \gtreqqless           |
| ⨄           | \biguplus       | ⪕           | \eqslantless          |
| ⨅           | \bigsqcap       | ⪖           | \eqslantgtr           |
| ⨆           | \bigsqcup       | ⪡           | \NestedLessLess       |
| ⨉           | \varprod        | ⪢           | \NestedGreaterGreater |
| ⨌           | \iiiint         | ⪦           | \leftslice            |
| ⨏           | \fint           | ⪧           | \rightslice           |
| ⨖           | \sqint          | ⪯           | \preceq               |
| ⨝           | \Join           | ⪰           | \succeq               |
| ⨟           | \zcmp           | ⪳           | \preceqq              |
| ⨠           | \zpipe          | ⪴           | \succeqq              |
| ⨡           | \zproject       | ⪷           | \precapprox           |
| ⨾           | \fcmp           | ⪸           | \succapprox           |
| ⨿           | \amalg          | ⪹           | \precnapprox          |
| ⩞           | \doublebarwedge | ⪺           | \succnapprox          |
| ⩤           | \dsub           | ⪻           | \llcurly              |
| ⩥           | \rsub           | ⪼           | \ggcurly              |
| ⩴           | \Coloneqq       | ⫅           | \subseteqq            |
| ⩵           | \Equal          | ⫆           | \supseteqq            |
| ⩶           | \Same           | ⫋           | \subsetneqq           |
| ⩽           | \leqslant       | ⫌           | \supsetneqq           |
| ⩾           | \geqslant       | ⫪           | \Top                  |
| ⪅           | \lessapprox     | ⫫           | \Bot                  |
| ⪆           | \gtrapprox      | ⫴           | \interleave           |
| ⪇           | \lneq           | ⫼           | \biginterleave        |
| ⪈           | \gneq           | ⫽           | \sslash               |
| ⪉           | \lnapprox       | ⫾           | \talloblong           |

#### 杂项符号和箭头

| Unicode编码 | LaTeX公式    | Unicode编码 | LaTeX公式 |
| ----------- | ------------ | ----------- | --------- |
| ⬛           | \blacksquare | ⬜           | \square   |