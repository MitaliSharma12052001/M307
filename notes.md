# Field

Commutative Division Ring

## Invariants

1. Characteristic:

	 smallest $n \in \mathbb{N}$ such that $n.1_F=0$ 

2. 







# Prime Subfield



$char(F)=p$ then, $\frac{\mathbb{Z}}{p\mathbb{Z}}$ is the prime field of $F$ (field generated by $1_{F}$)







# <a name="l1"> Lemma 1</a>

## proposition



a homomorphism from a field $F$ to a field $F'$ is either $0$ or $injective$ 



## proof



$Ker(\phi)$ = $Ideal\ of\ F$ but a field has only two ideals, i.e $0$ and $F$ thus either $\phi$ is **injective** or trivial.





# Extension of a Field

* constructing fields to contain roots of polynomials in base fields polynomial ring.

## <a name="t1">Theorem 1</a>

### proposition



if $f(x) \in F[x]$ is an irreducible polynomialwith no roots in $F$, then $\exists$ an *extension* of $F$ that contains the root.



### proof (constructive)


$\lt f(x)\gt$ is a prime ideal in an integral domain and hence is a maximal ideal.

So, we can define $K:=\frac{F[x]}{\lt f(x)\gt}$, a field. now this field contains a root of f(x)

because, $\bar{x}=x\ mod(f(x)) \in K$

and $f(\bar{x})=\bar{f(x)}=f(x)\ mod (f(x))=0$



## Degree of Extension

* notation:

	 $[K:F]$ 

* definition:

	$dim(K\ as\ a\ vector\ space\ over\ F)$



### minimal polynomial and basis for  $K(F)$

#### proposition



if $p(x) \in F[x]$ is a monic irreducible polynomial with root $\theta$ and degree $n$ then, defining $K:=\frac{F[x]}{\lt p(x)\gt}$ contains the root,

and $\alpha=x\ mod(p(x))\in K$ then $\{1,\alpha,\alpha^2,\dots,\alpha^{n-1}\}$ forms a basis of $K\ over F$ 



#### proof



Let $g(x)\in \frac{F[x]}{\lt p(x)\gt}$ then, $g(x)=b(x)$ with $deg(b(x))\lt n$



thus $\{1,\alpha,\alpha^2,\dots,\alpha^{n-1}\}$ spans $K$.

assume $\Sigma_{i=0}^{n-1}(c_i\alpha^i)=0$ in $K$ thus, $p(x)|\Sigma_{i=0}^{n-1}(c_i\alpha^i)=0$

but $deg(p(x))=n\gt n-1=deg(\Sigma_{i=0}^{n-1}(c_i\alpha^i)$

so, $c_i=0\  \forall\  i \in {0,1,2,\dots,n-1}$

hence $\{1,\alpha,\alpha^2,\dots,\alpha^{n-1}\}$ are LI in $F$

Therefore we conclude that $[K:F]=n$











## simple extension



If $K$ is a field extension of $F$ and $\alpha \in K$ then, $\exists!$ minimal subfield of K containing $F\ and\ \alpha$, called $F(\alpha)$



### proposition



$F(\alpha)\cong\frac{F[x]}{\lt p(x)\gt}$



### proof



$\phi:\ F[x]\rightarrow F(\alpha)$

$f(x)\rightarrow f(\alpha)$

$Ker(\phi)=\lt p(x)\gt\ \because p(\alpha)=0\implies p(x)\subseteq Ker(\phi)$ and $g(x) \in Ker(\phi)\implies g(\alpha)=0$, but $p(x)$ is the minimal polynomial, hence $\lt p(x)\gt=Ker(\phi)$

Consider the induced map $\bar{\phi}:\frac{F[x]}{\lt p(x)\gt} \rightarrow F(\alpha)$, an injective map, since it is a homomorphism of fields ( $\lt p(x)\gt$  is a maximal ideal), also it is surjective (contains both $F$ and $\alpha$)





# example of finding  $h(x)^{-1}$ 



$p(x)=x^3-2\ \in F=\mathbb{Q}[x]$

$K:=\frac{\mathbb{Q}[x]}{(x^3-2)}\cong\{a+b\theta+c\theta^2; a,b,c \in \mathbb{Q} , \theta=x\ mod(p(x))\}$

$h(x)=1+\theta$

but $(1+x)\ and\ (x^3-2)$ are co-prime

so that $a(x)(1+x)+b(x)(x^3-2)=1_F$

so $a(x)(1+\theta)=1_F\ mod(x^3-2)$ 

$(1+\theta)^{-1}=a(x) \in K$



## <a name="t2">Theorem 2 </a>

## proposition