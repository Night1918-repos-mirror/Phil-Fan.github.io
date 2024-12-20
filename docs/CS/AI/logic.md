# Logic


!!! note "演绎逻辑的核心逻辑"
    必然地导出


!!! tip "大部分人都是归纳鬼才、类比高手、演绎餐费"


## 基础知识

<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=883186648&bvid=BV1RK4y147no&cid=193631393&p=1&autoplay=0" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" width="100%" height="500px"></iframe>


- 概念：有意义的词项；ex：苹果、人、桌子
- 命题：概念集合，确定关系；ex：苹果是水果，人是动物，桌子是家具
- 推理：从前提必然地导出结论
- 逻辑：确保推理与论证有效的规则
- 论证：有推出关系的语群

![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/20241115223524.png)


AEIO

![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/20241115223618.png)

逻辑是形式科学，形式有效不等于内容有效




## 历史

### 1. **古代逻辑（公元前5世纪–公元5世纪）**
   - **苏格拉底、柏拉图与亚里士多德**：古希腊哲学家为逻辑学奠定了基础。尤其是亚里士多德，他被认为是逻辑学的奠基人。亚里士多德的《工具论》是逻辑学的经典之作，他提出了“三段论”作为推理的一种形式，这是传统形式逻辑的核心。
   - **智者学派**：智者学派的成员，如普罗塔戈拉斯，发展了论证技巧和修辞学，影响了后来的逻辑思考，尤其是在推理和辩论的层面。

### 2. **中世纪逻辑（公元5世纪–14世纪）**
   - **基督教哲学家的影响**：在中世纪，逻辑学的研究与神学、哲学紧密结合，特别是亚里士多德的逻辑学被基督教哲学家如托马斯·阿奎那等人所采纳并进一步发展。
   - **修辞学与辩证法**：中世纪的学者不仅关注推理的形式，也研究了语言和修辞如何影响论证的有效性，尤其在辩证法和神学辩论中尤为重要。

### 3. **近代逻辑的奠基（16世纪–19世纪）**
   - **笛卡尔与莱布尼茨**：笛卡尔强调数学与理性推理的基础，而莱布尼茨则提出了“理性语言”的概念，预示着后来的符号逻辑的发展。
   - **波尔布朗与布尔**：乔治·布尔在19世纪中期发展了代数逻辑（布尔代数），使逻辑学可以形式化、符号化，成为现代计算机科学和数字电路的基础。

### 4. **现代逻辑（20世纪至今）**
   - **符号逻辑与数理逻辑的兴起**：20世纪初，逻辑学经历了深刻的变革，尤其是在哥德尔、不完全性定理、罗素和怀特海的《数理逻辑原理》以及康托尔集合论的影响下。数学逻辑成为一门独立的学科，深入探讨了集合论、命题逻辑、谓词逻辑等基础。
   - **形式化与自动化**：随着计算机科学的发展，逻辑学的符号化与形式化理论得到了广泛应用。形式化逻辑成为计算机程序设计和人工智能的理论基础。
   - **非经典逻辑**：20世纪中期以后，随着对经典逻辑的深刻理解，非经典逻辑如模态逻辑、直觉主义逻辑、直觉主义逻辑等得到了研究。这些逻辑系统挑战了传统逻辑的某些假设，提出了更为多元和灵活的推理方式。

### 5. **当代逻辑学的发展**
   - **人工智能与自动推理**：在现代人工智能的研究中，逻辑学扮演了重要的角色，尤其是在推理、知识表示和自动定理证明等方面。
   - **量子逻辑**：量子力学的发展导致了量子逻辑的提出，这种逻辑挑战了经典逻辑中的某些基本假设，尤其是关于命题的真值和推理的规则。





## 词项逻辑：关注概念

### 三段论

思维中澄清概念关系；
- 中项必须在前提中周延至少一次



## 命题逻辑：关注命题——算算算



命题逻辑是应用一套形式化的规则对以符号表示的描述性陈述进行推理的系统。

<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=470304307&bvid=BV1UT411g7YG&cid=754709410&p=1&autoplay=0" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" width="100%" height="500px"></iframe>

### 命题连接词
复合命题

穷尽所有符合命题的判断规则

真值表

演算叫做命题演算

可以使用与或非表示所有命题连接词



如果$p$那么$q$：$p \rightarrow q$,$p$是$q$的充分条件,表示的是一种蕴含关系。所以当$p$不成立的时候，相当于$p$是空集，空集是任何集合的子集，所以$p \rightarrow q$一定成立。

| 公式 | 等价公式 |
| --- | --- |
| $\alpha \land \beta \equiv \beta \land \alpha$ ( $\land$ 的交互律 ) | $(\alpha \Rightarrow \beta) \equiv \neg \alpha \lor \beta$ ( 蕴涵消除 ) |
| $\alpha \lor \beta \equiv \beta \lor \alpha$ ( $\lor$ 的交互律 ) | $(\alpha \Leftrightarrow \beta) \equiv (\alpha \Rightarrow \beta) \land (\beta \Rightarrow \alpha)$ ( 双向消除 ) |
| $(\alpha \land \beta) \land \gamma \equiv \alpha \land (\beta \land \gamma)$ ( $\land$ 的结合律 ) | $\neg (\alpha \land \beta) \equiv (\neg \alpha \lor \neg \beta)$ ( De Morgan ) |
| $(\alpha \lor \beta) \lor \gamma \equiv \alpha \lor (\beta \lor \gamma)$ ( $\lor$ 的结合律 ) | $\neg (\alpha \lor \beta) \equiv (\neg \alpha \land \neg \beta)$ ( De Morgan ) |
| $\neg (\neg \alpha) \equiv \alpha$ ( 双重否定 ) | $(\alpha \land (\beta \lor \gamma)) \equiv (\alpha \land \beta) \lor (\alpha \land \gamma)$ ( $\land$ 对 $\lor$ 的分配律 ) |
| $(\alpha \Rightarrow \beta) \equiv \neg \beta \Rightarrow \neg \alpha$ ( 逆否命题 ) | $(\alpha \lor (\beta \land \gamma)) \equiv (\alpha \lor \beta) \land (\alpha \lor \gamma)$ ( $\lor$ 对 $\land$ 的分配律 ) |

### 推理规则

归结：$\alpha  \lor\beta, \neg \alpha$ 推出 $\beta$

有一对相反的可以抵消


### 命题范式
- 有限个简单合取式构成的析取式称为析取范式
- 由有限个简单析取式构成的合取式称为合取范式
- 析取范式与合取范式统称为范式 (normal form)


- 一个析取范式是不成立的，当且仅当它的每个简单合取式都不成立。
- 一个合取范式是成立的，当且仅当它的每个简单析取式都是成立的。

◀ 任一命题公式都存在着与之等值的析取范式与合取范式(注意：命题公式的析取范式与合取范式都不是唯一的)

!!! example "求 $\neg (\alpha \rightarrow \beta) \lor \neg \gamma$ 的析取范式与合取范式"

    $$
    \begin{aligned}
    &\neg (\alpha \rightarrow \beta) \lor \neg \gamma \\
    \Leftrightarrow &\neg (\neg \alpha \lor \beta) \lor \neg \gamma \\
    \Leftrightarrow &(\alpha \land \neg \beta) \lor \neg \gamma \quad (\text{析取范式}) \\
    \Leftrightarrow &(\alpha \lor \neg \gamma) \land (\neg \beta \lor \neg \gamma) \quad (\text{合取范式})
    \end{aligned}
    $$

## 谓词逻辑

!!! note "命题逻辑有局限性，无法表示从属关系、个体关系等"

个体、谓词、量词


<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=642822190&bvid=BV1ZY4y1J78y&cid=757283302&p=1&autoplay=0" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" width="100%" height="500px"></iframe>



### 量词

**全称量词 (universal quantifier, $\forall$)**

- 全称量词用符号 ∀ 表示，表示一切的、凡是的、所有的、每一个等。
- $\forall x$ 表示定义域中的所有个体，$\forall x P(x)$ 表示定义域中的所有个体具有性质 P

**存在量词 (existential quantifier, $\exists$)**

- 存在量词用符号 ∃ 表示，表示存在、有一个、某些等。
- $\exists x$ 表示定义域中存在一个或若干个个体，$\exists x P(x)$ 表示定义域中存在一个个体或若干个个体具有性质 P
### 谓词
- 谓词中个体变元用个体常量带入后就变成了命题，如 $\text{car}(x)$ （$x$ 是车）这个谓词中 $x$ 用吉普车代替，则 $\text{car}($ 吉普车 $)$ 是命题。
- 函数是从定义域到值域的映射；谓词是从定义域到 $\{ \text{True}, \text{False} \}$ 的映射

**合式公式**

- 命题常项、命题变项、原子谓词（不存在任何量词与联结词）是合式公式。
- 如果 $A$ 和 $B$ 是合式公式，那么 $\neg A$、$A \land B$、$A \lor B$、$A \rightarrow B$、$A \leftrightarrow B$ 都是合式公式
- 如果 $A$ 是合式公式，$x$ 是个体变元，则 $\exists x A(x)$ 和 $\forall x A(x)$ 也是合式公式
- 有限次地使用上述规则获得的公式是合式公式

### 推理规则

- 全称量词消去 (Universal Instantiation, UI): $(\forall x) A(x) \rightarrow A(y)$
- 全称量词引入 (Universal Generalization, UG): $A(y) \rightarrow (\forall x) A(x)$
- 存在量词消去 (Existential Instantiation, EI): $(\exists x) A(x) \rightarrow A(c)$
- 存在量词引入 (Existential Generalization, EG): $A(c) \rightarrow (\exists x) A(x)$





!!! example "证明案例"

    === "例子1"
        ![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/781f560aea6dc20644c2a507f5c82c9.png)

    === "例子2"
        ![](https://philfan-pic.oss-cn-beijing.aliyuncs.com/img/76ee4f24bdd379d37727a1cc78a6626.png)

    === "例子3"
        每一个奇数均存在一个大于它的奇数：
        - $\text{odd}(x): x$ 是奇数
        - $\text{Great}(x, y): x 大于 y$
        - $(\forall x)(\text{odd}(x) \rightarrow (\exists y)(\text{odd}(y) \land \text{Great}(y, x)))$

        证明：

        1. $(\neg \forall x) \text{Plane}(x) \rightarrow \text{on\_fly}(x)$
        2. $(\exists x)(\neg \text{Plane}(x) \rightarrow \text{on\_fly}(x))$
        3. $(\exists x)(\neg \text{Plane}(x) \lor \text{on\_fly}(x))$
        4. $(\exists x)(\text{Plane}(x) \land \neg \text{on\_fly}(x))$
        5. $\text{Plane}(a) \land \neg \text{on\_fly}(a)$
        6. $\text{Plane}(a)$
        7. $\neg \text{on\_fly}(a)$
        8. $(\forall x)(\text{plane}(x) \rightarrow (\text{in\_ground}(x) \lor \text{on\_fly}(x)))$
        9. $\text{plane}(a) \rightarrow (\text{in\_ground}(a) \lor \text{on\_fly}(a))$
        10. $\text{in\_ground}(a) \lor \text{on\_fly}(a)$
        11. $\text{in\_ground}(a)$
        12. $\text{Plane}(a) \land \text{in\_ground}(a)$
        13. $(\exists x)(\text{plane}(x) \land \text{in\_ground}(x))$


### 应用领域：专家系统
把某个领域的自然语言、文本语句进行逻辑化，使用谓词进行表达，把问题推给推理机，推理机就能得出结论

