To see how any formula was written in any question or answer, including this one, right-click on the expression and choose "Show Math As > TeX Commands". (When you do this, the '$' will not display. Make sure you add these: see the next point. There are also [other ways](https://math.meta.stackexchange.com/questions/659/how-to-view-latex-source-of-equations) to view the code for the formula or the whole post.)

1. **For inline formulas, enclose the formula in `$`…`$`. For displayed formulas, use `$$`…`$$`.**
    
    - These render differently. For example, type the following to show _inline_ mode:  
        `$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$`  
        ∑𝑛𝑖=0𝑖2=(𝑛2+𝑛)(2𝑛+1)6∑�=0��2=(�2+�)(2�+1)6
    - or type the following for display mode:  
        `$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$`  
        
        ∑𝑖=0𝑛𝑖2=(𝑛2+𝑛)(2𝑛+1)6∑�=0��2=(�2+�)(2�+1)6
        
2. For **Greek letters**, use `\alpha`, `\beta`, …, `\omega`: 𝛼�, 𝛽�, …, 𝜔�.
    
    - For uppercase letters, use `\Gamma`, `\Delta`, …, `\Omega`: ΓΓ, ΔΔ, …, ΩΩ.
    - For other Greek capital letters, use Latin `$A,`, `B`, `E$` and so on: 𝐴,𝐵,𝐸�,�,�.
    - Some Greek letters have variant forms: `\epsilon \varepsilon` 𝜖�, 𝜀�, `\phi \varphi` 𝜙�, 𝜑�, and others.
3. For **superscripts and subscripts**, use `^` and `_`. For example, `x_i^2`: 𝑥2𝑖��2, `\log_2 x`: log2𝑥log2⁡�.
    
4. **Groups**. Superscripts, subscripts, and other operations apply only to the next “group”. A “group” is either a single symbol, or any formula surrounded by curly braces `{`…`}`.
    
    - If you do `10^10`, you will get a surprise: 10101010. But `10^{10}` gives what you probably wanted: 10101010.
    - Use curly braces to delimit a formula to which a superscript or subscript applies: `x^5^6` is an error; `{x^y}^z` is 𝑥𝑦𝑧���, and `x^{y^z}` is 𝑥𝑦𝑧���. Observe the differences between `x_i^2` 𝑥2𝑖��2, `x_{i^2}` 𝑥𝑖2��2 and `{x_i}^2` 𝑥𝑖2��2.
5. **Parentheses** Ordinary symbols `()[]` make parentheses and brackets (2+3)[4+4](2+3)[4+4]. Use `\{` and `\}` for curly braces {}{}.
    
    - These do _not_ scale with the formula in between, so if you write `(\frac{\sqrt x}{y^3})` the parentheses will be too small: (𝑥√𝑦3)(��3). Using `\left(`…`\right)` will make the sizes adjust automatically to the formula they enclose: `\left(\frac{\sqrt x}{y^3}\right)` is (𝑥√𝑦3)(��3).
        
    - `\left` and`\right` apply to all the following sorts of parentheses: `(` and `)` (𝑥)(�), `[` and `]` [𝑥][�], `\{` and `\}` {𝑥}{�}, `|` |𝑥||�|, `\vert` |𝑥||�|, `\Vert` ‖𝑥‖‖�‖, `\langle` and `\rangle` ⟨𝑥⟩⟨�⟩, `\lceil` and `\rceil` ⌈𝑥⌉⌈�⌉, and `\lfloor` and `\rfloor` ⌊𝑥⌋⌊�⌋. `\middle` can be used to add additional dividers. There are also invisible parentheses, denoted by `.`: use `\left.x^2\right\rvert_3^5 = 5^2-3^2` to get
        
        𝑥2∣∣53=52−32�2|35=52−32
        
6. **Sums and integrals** `\sum` and `\int`; the subscript is the lower limit and the superscript is the upper limit, so for example `\sum_1^n` ∑𝑛1∑1�. Don't forget `{`…`}` if the limits are more than a single symbol. For example, `\sum_{i=0}^\infty i^2` is ∑∞𝑖=0𝑖2∑�=0∞�2.
    
    - Similarly, `\prod` ∏∏, `\int` ∫∫, `\bigcup` ⋃⋃,`\bigsqcup` ⨆⨆, `\bigcap` ⋂⋂, `\iint` ∬∬, `\iiint` ∭∭, `\idotsint` ∫⋯∫∫⋯∫.
7. **Fractions** There are [three ways to make fractions](https://math.meta.stackexchange.com/questions/12978/should-dfrac-be-edited-in). `\frac ab` applies to the next two groups, and produces 𝑎𝑏��; for more complicated numerators and denominators use `{`…`}`: `\frac{a+1}{b+1}` is 𝑎+1𝑏+1�+1�+1.
    
    - If the numerator and denominator are complicated, you may prefer `\over`, which splits up the group that it is in: `{a+1\over b+1}` is 𝑎+1𝑏+1�+1�+1.
    - For continued fractions, [use `\cfrac` instead of `\frac`](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference/5058#5058).
8. **Fonts**
    

- Use `\mathbb` or `\Bbb` for "blackboard bold": ℂℍℕℚℝℤ������.
- Use `\mathbf` for boldface: 𝐂𝐇𝐍𝐐𝐑𝐙������ 𝐜𝐡𝐧𝐪𝐫𝐳�ℎ����.
    - For expression based characters, use `\boldsymbol` instead: 𝜶�
- Use `\mathit` for italics: CHNQRZ������ chnqrz�ℎ����.
- Use `\pmb` for boldfaced italics: 𝐶𝐻𝑁𝑄𝑅𝑍𝐶𝐻𝑁𝑄𝑅𝑍������������ 𝑐ℎ𝑛𝑞𝑟𝑧𝑐ℎ𝑛𝑞𝑟𝑧�ℎ�����ℎ����.
- Use `\mathtt` for "typewriter" font: 𝙲𝙷𝙽𝚀𝚁𝚉������ 𝚌𝚑𝚗𝚚𝚛𝚣�ℎ����.
- Use `\mathrm` for roman font: CHNQRZCHNQRZ chnqrzchnqrz.
- Use `\mathsf` for sans-serif font: 𝖢𝖧𝖭𝖰𝖱𝖹������ 𝖼𝗁𝗇𝗊𝗋𝗓�ℎ����.
- Use `\mathcal` for "calligraphic" letters: ������ (Uppercase only.)
- Use `\mathscr` for script letters: 𝒞ℋ𝒩𝒬ℛ𝒵������ 𝒸𝒽𝓃𝓆𝓇𝓏�ℎ����
- Use `\mathfrak` for "Fraktur" (old German style) letters: ℭℌ𝔑𝔔ℜℨ������ 𝔠𝔥𝔫𝔮𝔯𝔷�ℎ����.

9. **Radical signs / roots** Use `sqrt`, which adjusts to the size of its argument: `\sqrt{x^3}` 𝑥3‾‾‾√�3; `\sqrt[3]{\frac xy}` 𝑥𝑦‾‾√3��3. For complicated expressions, consider using `{...}^{1/2}` instead.
    
10. Some **special functions** such as "lim", "sin", "max", "ln", and so on are normally set in roman font instead of italic font. Use `\lim`, `\sin`, etc. to make these: `\sin x` sin𝑥sin⁡�, not `sin x` 𝑠𝑖𝑛𝑥����. Use subscripts to attach a notation to `\lim`: `\lim_{x\to 0}`
    
    lim𝑥→0lim�→0
    
    Nonstandard function names can be set with `\operatorname{foo}(x)` foo(𝑥)foo⁡(�).
    
11. There are a very large number of **special symbols and notations**, too many to list here; see the short listing [𝐿𝐴𝑇𝐸𝑋����� and ���-𝐿𝐴𝑇𝐸𝑋����� Symbols](https://pic.plover.com/MISC/symbols.pdf) prepared by Dr. Emre Sermutlu, or the exhaustive listing [The Comprehensive 𝐿𝐴𝑇𝐸𝑋����� Symbol List](https://www.ctan.org/tex-archive/info/symbols/comprehensive/symbols-a4.pdf) by Scott Pakin. Some of the most common include:
    

- `\lt \gt \le \ge \neq` <<, >>, ≤≤, ≥≥,≠≠. You can use `\not` to put a slash through almost anything: `\not\lt` ≮≮ but it often looks bad.
    
- `\times \div \pm \mp` ××, ÷÷, ±±, ∓∓. `\cdot` is a centered dot: 𝑥⋅𝑦�⋅�
    
- `\cup \cap \setminus \subset \subseteq \subsetneq \supset \in \notin \emptyset \varnothing` ∪∪, ∩∩, ∖∖, ⊂⊂, ⊆⊆, ⊊⊊, ⊃⊃, ∈∈, ∉∉, ∅∅, ∅∅
    
- `{n+1 \choose 2k}` or `\binom{n+1}{2k}` (𝑛+12𝑘)(�+12�)
    
- `\to \gets \rightarrow \leftarrow \Rightarrow \Leftarrow \mapsto \implies \iff` →→, ←←, →→, ←←, ⇒⇒, ⇐⇐, ↦↦, ⟹⟹, ⟺⟺
    
- `\land \lor \lnot \forall \exists \top \bot \vdash \vDash` ∧∧, ∨∨, ¬¬, ∀∀, ∃∃, ⊤⊤, ⊥⊥, ⊢⊢, ⊨⊨
    
- `\star \ast \oplus \circ \bullet` ⋆⋆, ∗∗, ⊕⊕, ∘∘, ∙∙
    
- `\approx \sim \simeq \cong \equiv \prec \lhd` ≈≈, ∼∼, ≃≃, ≅≅, ≡≡, ≺≺, ⊲⊲
    
- `\infty \aleph_0` ∞ℵ0∞ℵ0 `\nabla \partial` ∇∇, ∂∂ `\Im \Re` ℑℑ, ℜℜ
    
- For modular equivalence, use `\pmod` like this: `a\equiv b\pmod n` 𝑎≡𝑏(mod𝑛)�≡�(mod�). For the binary mod operator, use `\bmod` like this: `a\bmod 17` 𝑎mod17�mod17.
    
- Use `\dots` for the triple dots in 𝑎1,𝑎2,…,𝑎𝑛�1,�2,…,�� and 𝑎1+𝑎2+⋯+𝑎𝑛�1+�2+⋯+��
    
- Script lowercase l is `\ell` ℓℓ.
    
    [Detexify](https://detexify.kirelabs.org/classify.html) lets you draw a symbol on a web page and then lists the 𝑇𝐸𝑋��� symbols that seem to resemble it. These are not guaranteed to work in MathJax, but it's a good place to start. To check that a command is supported, note that MathJax.org maintains a [list of currently supported 𝐿𝐴𝑇𝐸𝑋����� commands](https://docs.mathjax.org/en/latest/input/tex/macros/index.html), and one can also check Dr. Carol JVF Burns's page of [𝑇𝐸𝑋��� Commands Available in MathJax](https://www.onemathematicalcat.org/MathJaxDocumentation/TeXSyntax.htm).
    

12. **Spaces** MathJax usually decides for itself how to space formulas, using a complex set of rules. Putting extra literal spaces into formulas will not change the amount of space MathJax puts in: `a␣b` and `a␣␣␣␣b` are both 𝑎𝑏��. To add more space, use `\,` for a thin space 𝑎𝑏��; `\;` for a wider space 𝑎𝑏��. `\quad` and `\qquad` are large spaces: 𝑎𝑏��, 𝑎𝑏��.
    
    To set plain text, use `\text{…}`: {𝑥∈𝑠∣𝑥 is extra large}{�∈�∣� is extra large}. You can nest `$…$` inside of `\text{…}`, for example to access spaces.
    
13. **Accents and diacritical marks** Use `\hat` for a single symbol 𝑥̂ �^, `\widehat` for a larger formula 𝑥𝑦ˆ��^. If you make it too wide, it will look silly. Similarly, there are `\bar` 𝑥¯�¯ and `\overline` 𝑥𝑦𝑧⎯⎯⎯⎯⎯⎯⎯⎯⎯���¯, and `\vec` 𝑥⃗ �→ and `\overrightarrow` 𝑥𝑦−→��→ and `\overleftrightarrow` 𝑥𝑦←→��↔. For dots, as in 𝑑𝑑𝑥𝑥𝑥˙=𝑥˙2+𝑥𝑥¨�����˙=�˙2+��¨, use `\dot` and `\ddot`.
    
14. Special characters used for MathJax interpreting can be escaped using the `\` character: \$ $$, `\{` {{, `\}` }}, `\_` __, `\#` ##, `\&` &&. If you want `\` itself, you should use `\backslash` (symbol) or `\setminus` ([binary operation](https://tex.stackexchange.com/questions/511328/difference-between-commands-setminus-and-backslash/511332#511332)) for ∖∖, because `\\` is for a new line.
    

(Tutorial ends here.)