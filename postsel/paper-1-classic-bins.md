# Four Exhaustive Bell Bins with a Shared Geometry

## Abstract

Independent binary records can be divided into four exhaustive subensembles
whose conditional correlations match the four Bell states. No record need be
discarded. Bacciagaluppi and Hermens showed, however, that unrestricted
post-selection is too powerful: a classical sorter can also produce the
algebraic CHSH value $4$, above the quantum maximum $2\sqrt{2}$. We add one
restriction. Every correlation in every bin must be an overlap within one
shared geometry of measurement directions. This gives all four ideal
Bell-state tables, fixes the correlations at unused angles, and limits every
CHSH expression to $2\sqrt{2}$. Victor's bin label is the outcome of his
local Bell-state measurement, while the grouping of records is performed
later. The measurements commute because Alice, Bob, and Victor act on
different particles, so the account is unchanged when their temporal order is
reversed. A separate measurement by Victor gives product-state bins and the
classical CHSH bound. The shared geometry is taken here as a model postulate;
its deeper physical origin is left open.

## 1. Four exhaustive bins

Consider the ideal entanglement-swapping arrangement. Two independent sources
produce particle pairs $1,2$ and $3,4$. Alice receives particle $1$, Bob
receives particle $4$, and Victor receives particles $2$ and $3$. Alice
and Bob freely choose polarization directions $\alpha$ and $\beta$, then
record results $a,b\in\{-1,+1\}$. Before Victor's result is used, their
records are independent and unbiased:

$$
P(a,b\mid\alpha,\beta)=\frac14.
$$

Victor performs a **Bell-state measurement** (BSM), a joint measurement of his
two co-located particles. Its four possible labels are
$\Phi^+,\Phi^-,\Psi^+,\Psi^-$. After the experiment, the three laboratories
compare their records and place every trial in the bin named by Victor's
label. This is **post-selection** in the limited sense used here: records are
grouped for conditional analysis, but none are rejected.

For a Bell label $L$, let

$$
p^L(\alpha,\beta)
=P(a=b\mid\alpha,\beta,L)
$$

be the probability of equal Alice--Bob results inside that bin. The
Bacciagaluppi--Hermens four-bin construction can be written as

$$
P(L\mid\alpha,\beta,a=b)=\frac{p^L(\alpha,\beta)}2,
$$

$$
P(L\mid\alpha,\beta,a\ne b)
=\frac{1-p^L(\alpha,\beta)}2.
$$

These equations describe a joint probability table. In the classical
after-the-fact simulation they can be used as a sorting algorithm. In the
physical experiment they are not instructions evaluated by Victor: $L$ is
his detector result, and the equations are conditional descriptions of the
records later compared.

Alice's and Bob's raw results are equal on half the trials and different on
half. If the four values of $p^L$ sum to $2$, the assignment probabilities
sum to one for either case, so every record has exactly one bin. Moreover,

$$
P(L\mid\alpha,\beta)
=\frac12\frac{p^L}{2}
 +\frac12\frac{1-p^L}{2}
=\frac14.
$$

Every bin therefore has the same size for every setting pair. Bayes' rule then
returns the intended conditional probability:

$$
P(a=b\mid\alpha,\beta,L)=p^L(\alpha,\beta).
$$

Because the rule depends only on whether the two results agree, not on their
individual signs, Alice's and Bob's results also remain unbiased inside each
bin.

## 2. One geometry for all four bins

Post-selection alone places no useful upper bound on the correlations. If the
four setting pairs in one bin are independently adjustable, its correlations
can be $+1,+1,+1,-1$, giving a CHSH value of $4$. The restriction proposed
here is that all setting pairs and all four bins must instead use the same
polarization geometry:

$$
\begin{aligned}
p^{\Phi^+}(\alpha,\beta)&=\cos^2(\alpha-\beta),&
p^{\Psi^-}(\alpha,\beta)&=\sin^2(\alpha-\beta),\\
p^{\Phi^-}(\alpha,\beta)&=\cos^2(\alpha+\beta),&
p^{\Psi^+}(\alpha,\beta)&=\sin^2(\alpha+\beta).
\end{aligned}
$$

The normalization needed above is immediate:

$$
\sum_L p^L
=\cos^2(\alpha-\beta)+\sin^2(\alpha-\beta)
 +\cos^2(\alpha+\beta)+\sin^2(\alpha+\beta)=2.
$$

For binary results, the correlation in a bin is

$$
E^L(\alpha,\beta)
=P(a=b\mid\alpha,\beta,L)-P(a\ne b\mid\alpha,\beta,L)
=2p^L-1.
$$

The four resulting tables are therefore

| Bell bin   | Alice--Bob correlation       |
| ---------- | ---------------------------- |
| $\Phi^+$   | $+\cos 2(\alpha-\beta)$      |
| $\Psi^-$   | $-\cos 2(\alpha-\beta)$      |
| $\Phi^-$   | $+\cos 2(\alpha+\beta)$      |
| $\Psi^+$   | $-\cos 2(\alpha+\beta)$      |

The correlations cancel in pairs. Since every bin has weight $1/4$, their
recombination gives

$$
\frac14\sum_L E^L(\alpha,\beta)=0,
$$

recovering the original uncorrelated ensemble.

This is one rule over a continuous range of angles, not sixteen probabilities
fitted separately to the four CHSH setting pairs. The other Bell bins are
obtained from the first by fixed reflections and sign flips. Consequently,
angles not used to define the model are predictions rather than free
parameters.

## 3. Why the maximum is $2\sqrt{2}$

Represent a polarization direction by the unit vector

$$
\mathbf a(\alpha)=(\cos2\alpha,\sin2\alpha),
\qquad
\mathbf b(\beta)=(\cos2\beta,\sin2\beta).
$$

For the $\Phi^+$ bin,
$E^{\Phi^+}(\alpha,\beta)=\mathbf a(\alpha)\mathbin{\cdot}\mathbf b(\beta)$. The remaining bins use a fixed reflection or sign change
of the same vectors. Thus every bin belongs to one shared unit-vector
geometry, the standard vector representation of quantum two-point
correlations.

For two directions on each side, one CHSH expression is

$$
\begin{aligned}
S={}&\mathbf a_1\mathbin{\cdot}\mathbf b_1
   +\mathbf a_1\mathbin{\cdot}\mathbf b_2
   +\mathbf a_2\mathbin{\cdot}\mathbf b_1
   -\mathbf a_2\mathbin{\cdot}\mathbf b_2\\
={}&\mathbf a_1\mathbin{\cdot}(\mathbf b_1+\mathbf b_2)
   +\mathbf a_2\mathbin{\cdot}(\mathbf b_1-\mathbf b_2).
\end{aligned}
$$

Because all four vectors have unit length,

$$
|S|
\leq\lVert\mathbf b_1+\mathbf b_2\rVert
   +\lVert\mathbf b_1-\mathbf b_2\rVert
\leq2\sqrt2.
$$

The final inequality follows because the squares of the two displayed lengths
sum to $4$. Equality is reached, for example, with
$\alpha_1=0$, $\alpha_2=\pi/4$, $\beta_1=\pi/8$, and
$\beta_2=-\pi/8$. The other three Bell bins reach the same magnitude with
their corresponding fixed CHSH sign pattern. The shared geometry therefore
permits the quantum maximum but excludes the independently chosen pattern
that gives $4$.

There is a short analogy with Bell's classical bound. Four predetermined
binary results satisfy

$$
(a_1b_1)(a_1b_2)(a_2b_1)(a_2b_2)=+1,
$$

so their four pairwise relationships cannot contain exactly three agreements
and one disagreement. Shared geometry imposes a continuous version of the
same consistency requirement: the four overlaps must fit one arrangement of
directions. Fine established the discrete joint-distribution condition;
Tsirelson, Landau, Masanes, and later geometric treatments established the
corresponding unit-vector condition. We use that known mathematics as a
restriction on the four post-selection bins.

## 4. Local records and measurement order

Victor's BSM is joint but local: both particles entering it are in his
laboratory. Alice measures particle $1$, Victor measures particles $2,3$,
and Bob measures particle $4$. Their measurement operators act on disjoint
parts of the four-particle system. Hence, for every setting and result,

$$
[M_A,M_V]=[M_B,M_V]=[M_A,M_B]=0,
$$

where $[X,Y]=XY-YX$ measures the difference between the two possible
orders. The joint probability $P(a,b,L\mid\alpha,\beta)$ is consequently
the same whether Victor measures before or after Alice and Bob.

Bayes' rule allows this one joint table to be read in either direction. If
Alice and Bob are described first, their result pair conditions the
probabilities of Victor's four labels. If Victor is described first, his label
conditions the four possible Alice--Bob result pairs. This statistical
reversal is not the reason for commutation; it only relates two descriptions
of measurements that already commute.

The locality claim is operational: each apparatus interacts only with the
particles in its own laboratory. Victor uses no distant setting or result to
produce his label. The records are grouped only after ordinary communication.
The raw Alice--Bob distribution factorizes, their settings are freely chosen,
and later grouping changes no earlier record. Thus the construction introduces
neither a faster-than-light signal, a backwards influence, nor a prior
correlation with the setting choices.

## 5. Separate-measurement control

Victor may instead measure his two particles separately in one polarization
basis. This **separable-state measurement** (SSM) has four local result pairs,
which again form four equally sized bins. Write Victor's two results as
$r,s\in\{-1,+1\}$, and measure Alice's and Bob's angles relative to Victor's
basis. For the two initial singlets, conditioning on $r,s$ leaves the outer
particles in a product state, with correlation

$$
E^{r,s}(\alpha,\beta)
=rs\cos2\alpha\cos2\beta.
$$

This factorizes as $E_{ij}=u_i v_j$, with $|u_i|,|v_j|\leq1$. Its CHSH
value therefore obeys

$$
|S|\leq|v_1+v_2|+|v_1-v_2|\leq2.
$$

Each of the four values of $r,s$ occurs with probability $1/4$, and their
signs cancel when the bins are recombined. The SSM thus gives the expected
product-state statistics without the Bell-state violation. It is a control on
the construction, not a second mechanism.

## 6. Scope and open direction

The model uses exhaustive post-selection together with one substantive
restriction: every bin must share one measurement geometry. This restriction
reproduces the four ideal Bell tables, preserves unbiased raw data, reaches
but never exceeds $2\sqrt2$, and applies unchanged in either measurement
order. It also avoids setting-by-setting fine tuning because the same formulas
fix a continuous family of unused angles.

We do not derive shared geometry from a deeper physical principle here.
Rotational symmetry, conservation, macroscopic locality, and relativistic
independence are possible motivations, but deciding among them is left open.
Extensions to arbitrary qubit directions, noisy data, and partial optical Bell
analyzers are likewise reserved for later work.

## References

1. Guido Bacciagaluppi and Ronnie Hermens,
   [“Bell Inequality Violation and Relativity of Pre- and Postselection”](https://arxiv.org/abs/2002.03935),
   2020.
2. Xiao-song Ma et al.,
   [“Experimental delayed-choice entanglement swapping”](https://arxiv.org/abs/1203.4834),
   2012.
3. Arthur Fine,
   [“Hidden Variables, Joint Probability, and the Bell Inequalities”](https://doi.org/10.1103/PhysRevLett.48.291),
   1982.
4. Boris S. Tsirelson,
   [“Quantum analogues of the Bell inequalities”](http://www.ma.huji.ac.il/~ohadfeld/Tsirelson/download/qbell87.pdf),
   1987.
5. Lawrence J. Landau,
   [“Empirical two-point correlation functions”](https://doi.org/10.1007/BF00732549),
   1988.
6. Lluis Masanes,
   [“Necessary and sufficient condition for quantum-generated correlations”](https://arxiv.org/abs/quant-ph/0309137),
   2003.
7. Thinh P. Le, Chiara Meroni, Bernd Sturmfels, Reinhard F. Werner, and
   Timo Ziegler,
   [“Quantum Correlations in the Minimal Scenario”](https://arxiv.org/abs/2111.06270),
   2023.
