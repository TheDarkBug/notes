---
title-meta: "Appunti del corso di algebra e geometria"
author-meta: "Adriano Oliviero"
date-meta: "08/03/22"
keywords: "Geometria;Algebra"
---

# <mark>Appunti del corso di algebra e geometria</mark>
Questi appunti sono scritti da Adriano Oliviero durante le lezioni della prof.ssa [Anna Iezzi](https://aiezzi.it/) e sono distribuiti sotto la [licenza GPL-v3](../LICENSE). Il repository originario per questi (ed altri appunti) è su [github](https://github.com/TheDarkBug/notes).
# <mark>08/03/22</mark>
## Richiami di logica
Proposizione logica: **V**/**F**, **1**/**0** valore di verità

P = "Napoli è in Campania": **V**

P(n) = "n è pari"

P(2): **V**

P(3): **F**

## Connettivi logici
- Negazione: $\neg$, "non"
- Congiunzione: $\wedge$, "e"
- Disgiunzione: $\vee$, "o"
- Implicazione: $\Rightarrow$, "se \cdots allora \cdots"
- Doppia implicazione: $\Leftrightarrow$, "se e solo se"
## Tavole di verità
| $P$ | $Q$ | $\neg P$ | $P\wedge Q$ | $P\vee Q$ | $P\Rightarrow Q$ | $P\Leftrightarrow Q$ |
| --- | --- | -------- | ----------- | --------- | ---------------- | -------------------- |
| 1   | 1   | 0        | 1           | 1         | 1                | 1                    |
| 1   | 0   | 0        | 0           | 1         | 0                | 0                    |
| 0   | 1   | 1        | 0           | 1         | 1                | 0                    |
| 0   | 0   | 1        | 0           | 0         | 1                | 1                    |
## Quantificatori
- $\forall$: "Per ogni"
- $\exist$: "Esiste almeno uno"
- $\exist$!: "Esiste ed è unico"

<u>Esempi</u>:
1. "$\forall n$ naturale, $n$ è pari": F

   "$\exist$n naturale: ($\leftarrow$tale che) $n$ è pari": V
2. $P(x)=\{x$ è uno studente in aula A3-T2$\}$

   $Q(x)=\{x$ è iscritto ad un corso di ingegneria$\}$

   $\forall x, P(x)\Rightarrow Q(x)$
3. $P(n)=\{n$ è un numero pari$\}$

   $Q(n)=\{n$ è divisibile per $4\}$

   $\forall n$ naturale, $Q(n)\Rightarrow P(n)$
---
## Teoria degli insiemi
Un **insieme** è una collezione di oggetti detti **elementi** dell'insieme.

Convenzionalmente gli insiemi si denotano con lettere maiuscole e gli elementi con lettere minuscole.
### Descrizione di un insieme
1. Per elencazione (se l'insieme ha un numero finito di elementi):

   $\mathbb{A} = \{0, 2, 4, 6, 8, 10\}$

   $4\in \mathbb{A}$

   $5\notin \mathbb{A}$
2. Per proprietà caratteristica

   $\mathbb{A}=\{n: n$ è un numero pari: $0\le n \le 10\}$
3. Diagramma di *Eulero-Venn* (ancora una volta se l'insieme ha un numero finito di elementi)
### Alcune informazioni sugli insiemi
- La **cardinalità** di un insieme è il numero di elementi che un insieme contiene e si denota: $\mathbb{A}$ ha cardinalità $|\mathbb{A}|$
- Insieme vuoto: insieme che non contiene nessun elemento, si denota con $\emptyset$, $\{\}$ e ha cardinalità $|\emptyset|=0$
- I principali insiemi numerici:

  $\mathbb{N}=\{0, 1, 2, 3, \cdots\}$: numeri naturali

  $\mathbb{Z}=\{\cdots, -3, -2, -1, 0, 1, 2, 3, \cdots\}$: numeri naturali

  $\mathbb{Q}=\{\frac{a}{b}:a,b$ e $\mathbb{Z}, b\not= 0\}$

  $\R$: numeri reali

  $\mathbb{C}$: numeri complessi
### Operazioni tra gli insiemi
1. Inclusione

    $\mathbb{A}\subseteq\mathbb{B}$ $(\mathbb{A}$ è contenuto in $\mathbb{B})$

    $\mathbb{B}\supseteq\mathbb{A}$ $(\mathbb{B}$ contiene $\mathbb{A})$

    <u>Esempio</u>:
    $\mathbb{N}\subseteq\mathbb{Z}\subseteq\mathbb{Q}\subseteq\mathbb{R}\subseteq\mathbb{C}$

    <u>Proprietà</u>:
    - $\mathbb{A}=\mathbb{B}\Leftrightarrow(x\in \mathbb{A}\Leftrightarrow x \in \mathbb{B})\Leftrightarrow(\mathbb{A}\subseteq\mathbb{B}$ ^ $\mathbb{B}\subseteq\mathbb{A})$
2. Intersezione $\leftrightarrow\wedge$

    $\mathbb{A}\cap\mathbb{B}=\{x:x\in\mathbb{A}\wedge x\in\mathbb{B}\}$

    <u>Proprietà</u>:
    - $\mathbb{A}\cap\emptyset=\emptyset$
    - $\mathbb{A}\cap\mathbb{B}=\mathbb{B}\cap\mathbb{A}$
    - $\mathbb{A}\subseteq\mathbb{B}\Rightarrow\mathbb{A}\cap\mathbb{B}=\mathbb{A}$
3. Unione $\leftrightarrow\vee$

    $\mathbb{A}\cup\mathbb{B}=\{x:x\in\mathbb{A}\vee x\in\mathbb{B}\}$

    <u>Proprietà</u>:
    - $\mathbb{A}\cup\emptyset=\mathbb{A}$
    - $\mathbb{A}\cup\mathbb{B}=\mathbb{B}\cup\mathbb{A}$
    - $\mathbb{A}\subseteq\mathbb{B}\Rightarrow\mathbb{A}\cup\mathbb{B}=\mathbb{B}$
    - $\mathbb{A}\subseteq\mathbb{A}\cup\mathbb{B},\ \mathbb{B}\subseteq\mathbb{A}\cup\mathbb{B}$
4. Differenza

    $\mathbb{B}\backslash \mathbb{A}=\{x:x\in\mathbb{B}\wedge x\not\in\mathbb{A}\}$
5. Prodotto cartesiano:
    $\mathbb{A}\times\mathbb{B}:=\{(a,\ b):a\in\mathbb{A},\ b\in\mathbb{B}\}$ con $(a,\ b)$ coppie ordinate

    <u>Proprietà</u>:
    - $|\mathbb{A}\times\mathbb{B}|=|\mathbb{A}|\cdot|\mathbb{B}|$
    - $\mathbb{A}\times\emptyset=\emptyset=\emptyset\times\mathbb{A}$
---
## Funzioni
<u>Def</u>: Siano $\mathbb{A},\ \mathbb{B}$ due insiemi:
  Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ è una legge che associa ad ogni elemento di $\mathbb{A}$, uno ed un solo elemento di $\mathbb{B}$.

  $f:\mathbb{A}\rightarrow\mathbb{B}\\\qquad\!\!x\rightarrow y$: $x$ è la controimmagine di $y$

<u>Def</u>: Sia $f:\mathbb{A}\rightarrow\mathbb{B}$ una funzione e sia $\mathbb{X}\subseteq\mathbb{A}$

  $f(x):=\{f(x):x\in\mathbb{X}\}$ è l'insieme di $\mathbb{X}$ tramite $f$

  $Im(f):=f(\mathbb{A})$ è l'insieme della funzione

  $Im(f)$ non è necessariamente $=Dom(f)$

  $Im(f)=Dom(f)\Rightarrow f$ è suriettiva

  $f(1)=f(2)=a\Rightarrow f$ non è iniettiva
# Latex rewrite finisce qui
# <mark>09/03/22</mark>
## Funzioni (continuo)
<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>iniettiva</u> se $\forall x\not=y\Rightarrow f(x)\not=f(y)$ (elementi distinti di $\mathbb{A}$ hanno immagini distinte) $\Leftrightarrow f(x)=f(y)\Rightarrow x=y$

<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>suriettiva</u> se $Im(f)=B$, o equivalentemente se $\forall y\in \mathbb{B}, \exist x\in\mathbb{A}:f(x)=y$

<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>biettiva</u> o <u>biunivoca</u> se è al tempo stesso iniettiva e suriettiva

<u>Esempio</u>:

$f:\R\rightarrow\mathbb{R}\\\qquad\!\!x\rightarrow x^2$

È iniettiva? No, perchè $f(-1)=1=f(1)$

È suriettiva? No, perchè $f(x)=x^2\geq0\forall x\in\mathbb{R}\Rightarrow Im(f)\subseteq\mathbb{R}^+\Rightarrow Im(f)\not=\R$

<br>

Se un insieme possiede delle operazioni che verificano certe proprietà, è una struttura algebrica.

<u>Def</u>: Sia $\mathbb{X}$ un insieme, un'<u>operazione binaria interna</u> è una funzione dal prodotto cartesiano $x\times x$ in $\mathbb{X}$.

$*:x\times x \rightarrow x$

$\qquad\!\!\!(x,y)\rightarrow x*y$

$\mathbb{X}=\R$

$+:\R\times\mathbb{R}\rightarrow\mathbb{R}$

$\qquad(x,y)\rightarrow x+y$

<u>Proprietà</u> di $(\R,+)$:

1. Commutatività:  $x+y=y+x, \forall x,y\in\mathbb{R}$

2. Associatività:  $(x+y)+z=x+(y+z),\forall x,y,z\in\mathbb{R}$

3. Esistenza dell'elemento neutro:  $\exist x'\in\mathbb{R}:x+x'=x'+x=x,\forall x\in\mathbb{R}, x'=0$

4. Esistenza dell'opposto:  $\exist x'\in\mathbb{R}:x+x'=x'+x=0,\forall x\in\mathbb{R}, (x'=-x)$

$\R\times\mathbb{R}\rightarrow\mathbb{R}$ operazione binaria interna

$\quad\!\!\!\!(x,y)\rightarrow x\cdot y$

<u>Proprietà</u> di $(\R,\cdot)$:

1. Commutatività: $x\cdot y=y\cdot x, \forall x,y\in\mathbb{R}$

2. Associatività: $(x\cdot y)\cdot z=x\cdot(y\cdot z),\forall x,y,z\in\mathbb{R}$

3. Esistenza dell'elemento neutro: $\exist x'\in\mathbb{R}:x\cdot x'=x'\cdot x=x,\forall x\in\mathbb{R}, x'=1$

4. Esistenza dell'inverso: $\exist x'\in\mathbb{R}:x\cdot x'=x'\cdot x=0,\forall x\in\mathbb{R}, (x'=\frac{1}{x})$

Infine $+$ e $\cdot$ soddisfano la proprietà distributiva: $\forall x,y,z\in\mathbb{R},x\cdot(y+z)=x\cdot y+x\cdot z$

Sia $\mathbb{K}\not=\emptyset$ un insieme dotato di due operazioni binarie:

- $+: \mathbb{K}\times\mathbb{K}\rightarrow\mathbb{K}$

- $\cdot:\mathbb{K}\times\mathbb{K}\rightarrow\mathbb{K}$

$(\mathbb{K},+,\cdot)$ è detto un <u>campo</u> se verificano le proprietà elencate prima, con $+$ distributiva con $\mathbb{K}$ al posto di $\R$

<u>Esempio</u>:

$\mathbb{F}_2=\{0, 1\}$
  - $\cdot:\mathbb{F}_2\cdot\mathbb{F}_2\rightarrow\mathbb{F_2}$

    $\qquad\!(0, 0)\rightarrow 0$

    $\qquad\!(0, 1)\rightarrow 0$

    $\qquad\!(1, 0)\rightarrow 0$

    $\qquad\!(1, 1)\rightarrow 1$
  - $+:\mathbb{F}_2\times\mathbb{F}_2\rightarrow\mathbb{F}_2$

    $\qquad\!(0, 0)\rightarrow 0$

    $\qquad\!(0, 1)\rightarrow 1$

    $\qquad\!(1, 0)\rightarrow 1$

    $\qquad\!(1, 1)\rightarrow 1$
## Algebra lineare
Wikipedia:
> Branca della matematica che si occupa dello studio di spazi vettoriali (o anche detti spazi lineari), di trasformazioni lineari e di sistemi di equazioni lineari.

Molti problemi di matematica e fisica verificano la seguente proprietà:

Se $v,w\in\mathbb{X}$ sono due soluzioni del problema, allora anche $v+w$ e $\lambda v, \lambda\in\mathbb{R}$  ($+$ e $\cdot$ operazioni su $\mathbb{X}$) sono soluzioni del problema.

Problemi di questo tipo sono detti *lineari*.

### Nozione base: <u>spazio vettoriale</u>

I vettori sono usati in fisica per rappresentare, grandezze fisiche caratterizzate da:
- una direzione
- un verso
- un'intensità

Tali grandezze sono *grandezze vettoriali* e si differenziano dalle *grandezze scalari*, definite unicamente dall'intensità.

Geometricamente, un vettore si rappresenta tramite un *segmento orientato* nel piano euclideo, denotato $\Pi$.

<u>Def</u>: Un segmento orientato è una coppia di punti ordinata $(A,B\in\Pi\times\Pi)$.

$\vec{AB}:=(A,B)$.

<u>Def</u>: Due segmenti orientati $\vec{AB}$ e $\vec{CD}$ si dicono <u>equipollenti</u> se il quadrilatero avente vertici, ordinatamente, $ABDC$ è un parallelogramma, quindi se hanno:
- stella lunghezza
- direzione parallela
- stesso verso

L'equipollenza è una relazione di equivalenza, e verifica 3 proprietà:
- riflessiva
- simmetrica
- transitiva

<u>Def</u>: Un vettore geometrico è una classe di equipollenza

Sia $O$ un punto fissato nel piano $\Pi$, per ogni segmento orientato $\vec{AB}$ esiste un punto $P\in\Pi$ tale che $\vec{OP}$ è equipollente ad $\vec{AB}$.

$\vec{OP}$ è equipollente a tutti i segmenti orientati equipollenti ad $\vec{AB}$ e posso sceglierlo come <u>rappresentante</u> della classe di equipollenza di $\vec{AB}$.

Quindi abbiamo una biezione:

$\mathbb{V}=\{$Vettori geometrici nel piano$\}\{$segmento orientato $\vec{OP}, P\in\Pi\}$

Classi di equipollenza $\uparrow\qquad\qquad\qquad\qquad\qquad\qquad\uparrow$ Stesso punto di applicazione
# <mark>09/03/22</mark>
## Algebra lineare (continuo)
### Nozione base: <u>spazio vettoriale</u> (continuo)
Correzione della definizione di campo:
- Esistenza dell'elemento neutro

  $\exist 0\in\mathbb{R}:x+0=0+x=x,\forall x\in\mathbb{R}$
- Esistenza dell'opposto:

  $\exist x'\in\mathbb{R}:x+x'=x'+x=0,\forall x\in\mathbb{R}$
---
Fissiamo $O\in\pi$ (piano ordinario).

$\mathbb{V}=\{$vettori geometrici del piano$\}\Leftrightarrow\{$segmenti orientati$\vec{OP},P\in\pi\}$

Con un abuso di notazione, consideriamo:

$\mathbb{V}=\{$segmenti orientati $\vec{OP},P\in\pi\}$

$\forall\vec{v}\in V,\exist P\in\pi:\vec{v}=\vec{OP}$

<u>Operazioni su $\mathbb{V}$</u>:
- <u>somma di vettori</u>
  siano $\vec{v},\vec{w}\in \mathbb{V}$ e siano $P,Q\in\pi:$
  $\vec{v}=\vec{OP}$
  $\vec{w}=\vec{OQ}$

  Definiamo:

  $\vec{v}+\vec{w}=\vec{OR}$, tale che il quadrilatero $OPRQ$ è un parallelogramma. (regola del parallelogramma)

  <u>Nota</u>: Se $O,P$ e $Q$ sono collineari (hanno la stessa direzione),  costruisco $R$ tale che $OQ$ e $RP$ hanno la stessa lunghezza

  Operazione binaria interna: $+:\mathbb{V}\times\mathbb{V}\rightarrow\mathbb{V}$

  $(\vec{v},\vec{w})\rightarrow \vec{v}+\vec{w}$
- <u>Moltiplicazione per scalari</u>

  Sia $\vec{v}\in\mathbb{V}$ e sia $P\in\pi:\vec{v}=\vec{OP}$.

  Definiamo $\lambda\cdot\vec{v}=\vec{OR}$
  - $O,P,R$ sono collineari
  - $OR (simbolo\ di\ segmento\ su\ OP)=|\lambda|OP$
  - $\vec{OR}$ è orientato concordemente a $\vec{OP}\\\vec{OR}$ è orientato discordemente a $\vec{OP}$ se

    $\lambda<0\vee\lambda=0, R=O$

  Questa è un'operazione binaria <u>esterna</u>:

    $\cdot:\R\times\mathbb{V}\rightarrow \mathbb{V}\\\qquad\!\!\!(\lambda,\vec{v})\rightarrow\lambda\cdot\vec{v}$

## Piano Cartesiano

$\{P:P\in\pi\}\leftrightarrow\{(x,y):x,y\in\mathbb{R}\}=\mathbb{R}^2$

$\mathbb{V}=\{$segmenti orientati $\vec{OP},P\in\pi\}=\{$vettori geometrici nel piano$\}$

In particolare esiste una blezione:

$\mathbb{V}\leftrightarrow\mathbb{R}^2$

$\forall P\in\pi,\vec{OP}\rightarrow(x,y)$, dove $x,y$ sono rispettivamente ascissa e ordinata di $P$

$\vec{OP}\leftarrow(x,y)$ dove $P(x,y)$

Vogliamo tradurre le operazioni su $\mathbb{V}$ in operazioni su $\mathbb{R}^2$:

1. $\vec{v}=\vec{OP},P(x_P,y_P)$

    $\vec{w}=\vec{OQ},Q(x_Q,y_Q)$

    $\vec{v}+\vec{w}=\vec{OR}:$ quali sono le coordinate di R?

    $OPQR\Rightarrow A(x_A,y_A)$ parallelogramma con punto medio di $PQ$ e $OR$

    $A$ punto medio di $PQ\Rightarrow\{x_A=\frac{x_P+x_Q}{2}, y_A=\frac{y_P+x_Q}{2}\}$

    $A$ punto medio di $OR\Rightarrow\{x_A=\frac{x_R}{2},y_A=\frac{y_R}{2}\}$

    $\Rightarrow\{x_R=x_P+x_Q,y_R=y_P+y_Q\}$

    Operazione binaria <u>interna</u>: $+:\mathbb{R}^2\times\mathbb{R}^2\rightarrow\mathbb{R}^2$

    $((x_1,y_1),(x_2,y_2))\mapsto(x_1+x_2,y_1+y_2)$
2. $\vec{v}\in\mathbb{V},\vec{v}=\vec{OP},P(x_P,y_P), \lambda\in\mathbb{R}$

    $\lambda\cdot\vec{v}=\vec{OR}:$ quali sono le coordinate di R?

    $\vec{OR}=\lambda\cdot\vec{OP}$

    $OPH$ e $ORK$ sono simili per costruzione con rapporto di proporzioni $|\lambda|$.

    <u>Due casi</u>:
    1. $\lambda\ge0$ $\vec{OR}$ è concord con $\vec{OP}$ e quindi:

        $x_R=|\lambda|x_P=\lambda x_P$

        $y_R=|\lambda|y_P=\lambda y_P$
    2. $\lambda<0$ $\vec{OR}$ è discorde con $\vec{OP}$ e quindi:

        $x_R=-|\lambda|x_P=\lambda x_P$

        $y_R=-|\lambda|y_P=\lambda y_P$

    Operazione binaria <u>esterna</u>: $\cdot:\R\times\mathbb{R}^2\rightarrow\mathbb{R}^2$

    $(y,(x,y))\mapsto\lambda\cdot(x,y):=(\lambda x,\lambda y)$

    In conclusione abbiamo definito due operaizoni su $\mathbb{R}^2$ "compatibili" con le operazioni definite su $\mathbb{V}$:

      - $+: \mathbb{R}^2\times\mathbb{R}^2\rightarrow\mathbb{R}^2$

          $((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)+(x_2,y_2):=(x_1+y_1,x_2+y_2)$
      - $\cdot: \mathbb{R}^2\times\mathbb{R}^2\rightarrow\mathbb{R}^2$

          $(\lambda,(x_2,y_2))\mapsto\lambda\cdot(x_2,y_2):=(\lambda\cdot x,\lambda\cdot y)$

      <u>Proprietà di $+$ e $\cdot$</u>

      1. commutatività

          $\forall(x_1,y_1),(x_2,y_2)\in\mathbb{R}^2, (x_1,y_1)+(x_2,y_2)=(x_2,y_2)+(x_1,y_1)$
      2. associatività

          $\forall(x_1,y_1),(x_2,y_2),(x_3,y_3)\in\mathbb{R}^2,

          ((x_1,y_1)+(x_2,y_2))+(x_3,y_3)=(x_1,y_1)+((x_2,y_2)+(x_3,y_3))$
      3. esistenza dell'elemento neutro

          $(0,0)\in\mathbb{R}^2$ è tale che $(x,y)+(0,0)=(0,0)+(x,y)=(x,y)$
      4. esistenza dell'opposto

          $\forall (x,y)\in\mathbb{R}^2,\exist(x',y')\in\mathbb{R}^2:(x,y)+(x',y')=(x',y')+(x,y)=(0,0)$
      5. distributività rispetto a vettori

          $\forall(x_1,y_1),(x_2,y_2)\in\mathbb{R}^2,\forall\lambda\in\mathbb{R}$

          $\lambda\cdot((x_1,y_1)+(x_2,y_2))=\lambda\cdot(x_1,y_1)+\lambda\cdot(x_2,y_2)
      6. distributività rispetto a scalari

          $\forall(x,y)\in\mathbb{R}^2,\forall\lambda,\mu\in\mathbb{R}$

          $(\lambda+\mu)\cdot(x,y)=\lambda\cdot(x,y)+\mu\cdot(x,y)$
      7. qualcosa, non so cosa

          $\lambda\mu\cdot(x,y)=\lambda\cdot(\mu\cdot(x,y))$
      8. elemento neutro

          $1\cdot(x,y)=(x,y)\forall(x,y)\in\mathbb{R}^2$

      $(\mathbb{R}^2,+,\cdot)$ è il primo insieme di <MARK>INCOMPLETO</MARK>

    <u>Def</u>: Sia $\mathbb{K}$ (lettera K da "korper" in tedesco) un campo. Uno spazio vettoriale su $\mathbb{K}$ è un insieme $\mathbb{V}$ dotato di due operazioni:
      # <mark>Revisione conclusa qui (29/03/22 19:42:57)</mark>
    - $+: V\times V\rightarrow V$
    - $\cdot: K\times V\rightarrow V$

    che verificano le seguenti proprietà:
    1. commutatività: $\forall v,w\in V, v+w=w+v$
    2. associatività: $\forall u,v,w\in V,(u+v)+w=u+(v+w)$
    3. esistenza dell'elemento neutro:

        $\exist 0\in V: 0+v=v+0=v, \forall v\in V$
    4. esistenza dell'opposto:

        $\forall v\in V,\exist v'\in V: v+v'=v'+v=0$
    5. distributività rispetto alla somma di vettori:

        $\\forall v,w\in V,\forall \lambda\in K, \lambda\cdot(v+w)=\lambda\cdot v+\lambda\cdot w$
    6. distributività rispetto alla somma di scalari:

        $\forall v\in V, \forall \lambda,\mu\in K,(\lambda+\mu)\cdot v=\lambda\cdot v+\mu\cdot v$
    7. $\forall v\in V,\forall\lambda,\mu\in K,\lambda\mu\cdot v=\lambda\cdot(\mu\cdot v)$
    8. $1\cdot v=v,\forall v\in V$.

    Gli elementi di $\mathbb{V}$ sono chiamati vettori e gli elementi di $\mathbb{K}$ son chiamati scalari.

    $K=\R:$ spazio vettoriale reale

    $K=\mathbb{C}:$ spazio vettoriale complesso

    <u>Osservazioni</u>: Sia $\mathbb{V}$ un K-spazio vettiruake:

    - in $\mathbb{V}$ esiste un unico vettore nullo che denotiamo <u>0</u>.
    - $\forall v\in V$ esiste un unico opposto che denotiamo $-v$
    - $\forall v\in V$ si ha $0\cdot v=$ <u>0</u>
    - $\forall\lambda\in K$ si ha $\lambda\cdot$ <u>0</u> $=$ <u>0</u>
    - Siano $\lambda\in K,v\in K: \lambda\cdot v=$ <u>0</u> $\Rightarrow$ o $v=$ <u>0</u>
# <mark>16/03/22</mark>
$+:\mathbb{R}^2\times\mathbb{R}^2\rightarrow\mathbb{R}^2$

$((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)+(x_2,y_2):=(x_1+x_2,y_1+y_2)$

$*:\mathbb{R}^2\times\mathbb{R}^2$

$((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)*(x_2,y_2):=(x_1\cdot x_2,y_1\cdot y_2)$

$(\mathbb{R}^2,+,*)$ è un campo? NO!

$\triangle:\mathbb{R}^2\times\mathbb{R}^2$
$((a,b),(c,d))\mapsto(a,b)\triangle(c,d)=(ac-bd,ad+bc)$

Mostrare che $(\mathbb{R}^2,+,\triangle)$ è un campo.

<u>Indizio</u>: $\mathbb{R}^2\leftrightarrow\mathbb{C}=\{a+ib,b\in\mathbb{R},i^2=-1\}$

$(a,b)leftmapsto a+ib$

$(a,b)\mapsto a+ib$

Nota che $\mathbb{C}$ è un campo

### <u>Esempi di spazi vettoriali</u>
1. $\mathbb{V}=\{$Vettori geometrici nello spazio$\}=\{$segmenti orientati $\vec{OP},\ P$ nello spazio$\}\longleftrightarrow\mathbb{R}^3$

   Definiamo $+$ e $\cdot$ in modo analogo al caso dei vettori nel piano e $(V,+,\cdot)$ è uno spazio vettoriale reale.
2. L'$n$-spazio vettoriale su $\R$ (o su $\mathbb{K}$)

   $n\in\mathbb{N}, n\ge1$
   $\R^n=\R\times\cdots\times\mathbb{R}=\{(x_1,\cdots,x_n):x_i\in\mathbb{R}\forall i\}$

   Definiamo $+:\R^n\times\mathbb{R}^n\to\mathbb{R}^n$ e $\cdot:\R^n\times\mathbb{R}^n\to\mathbb{R}^n$

   $(x_1,\cdots,x_n)+(y_1,\cdots,y_n):=(x_1+y_1,\cdots,x_n+y_n)$

   $\lambda\in K$ <mark>INCOMPLETO</mark>

    $\forall n\ge1,(\R^n,+,\cdot)$ è uno spazio vettoriale reale chiamato $n$-spazio vettoriale <u >numerico</u> su $\R$.

    Elemento <u>neutro</u>: <u>0</u> $=(0,\cdots,0)$

    Elemento <u>opposto</u> di $x=(x_1,\cdots,x_n)$ è $-x=(-x_1,\cdots,-x_n)$

    <u>Osservazione</u>: $n=1:\ \R$ è uno spazio vettoriale su $\R$ (ogni campo $\mathbb{K}$ è uno spazio vettoriale su se stesso)

    In maniera analoga definiamo $+$ e $\cdot$ su

    $k^n=\{(x_1,\cdots,x_n):x_i\in K\forall i\}$

    $(k^n,+,\cdot)$ è uno spazio vettoriale su $\mathbb{K}$ chiamato $n$-spazio vettoriale numerico su $\mathbb{K}$.

    <u>Esempio</u>: $k=\mathbb{C},\ \mathbb{C}^n\\k=\mathbb{F}_2,\ \mathbb{F}^n_2$

  3. Funzioni da un insieme a un campo

     Sia $\mathbb{X}$ un insieme <u>qualunque</u> e $\mathbb{K}$ un campo

     $\mathbb{V}=\{$funzioni $f:\mathbb{X}\to\mathbb{K}\}$

     - Binaria interna: $+:V\times V\to V\\(f,g)\to f+g$

        dove $f+g: X\to K\\x\mapsto(f+g)(x):=f(x)+g(x)$
     - Binaria esterna: $\cdot: K\times V\to V\\(\lambda\cdot)$ <mark>INCOMPLETO</mark>
  4. Polinomi a coefficisnti reali in una indeterminata

     Sia $x$ un'indeterminata.
     Un <u>polinomio</u> a coefficienti reali nell'indeterminata $x$ è un'espressione formale del tipo:

     $P(x)=a_nx^n+a_{n-1}x^{n-1}+\cdots+a_1x+a_0,a_i\in\mathbb{R}\forall i$

     Se $a_n\ne0$ diremo che $n$ è il grado di $P$ e scriviamo $deg(P)=n$.

     $\R[x]:=\{$polinomi a coefficienti reali nell'indeterminata $x$ (di grado arbitrario)$\}$

     <u>Esempio</u>: $P(x)=3x^4+2x^3-x+5\in\mathbb{R}[x],\ deg(P)=4$

     $+:\R[x]\times\mathbb{R}[x]\to\mathbb{R}[x]\\P(x)=a_nx^n+\cdots+a_1x+a_0\\Q(x)=b_nx^n+\cdots+b_1x+b_0\\(P+Q)(x):=(a_n+b_n)x^n+\cdots+(a_1+b_1)x+a_0+b_0$

     $\cdot:\R\times\mathbb{R}[x]\to\mathbb{R}[x]\\P\in\mathbb{R}[x],\ P=a_nx^n+\cdots+a_1wx+a_0\\\lambda\in\mathbb{R}\\(\lambda\cdot P)(x):=\lambda a_nx^n+\cdots+\lambda a_1x+\lambda a_0$

     $(\R[x],+,\cdot)$ è uno spazio vettoriale su $\R$.

     In modo analogo si definisce $(K[x],+,\cdot)$ dove

     $K[x]=\{$polinomi a coefficienti in $\mathbb{K}$ in un'indetermiinata$\}$

     Molti problemi di matemadica/fisica hanno la proprietà che l'insieme delle soluzioni ha una struttura di spazio vettoriale.

     <u>Esempi</u>:

     - $\begin{cases}x+2y+z=0\\y+7z=0\end{cases}$

       $S=\{(x,y,z)\in\mathbb{R}^3:x+2y+z=0$ e $y+7z=0\}=\{(13t,-7t,t),t\in\mathbb{R}\}$
       $S$ ha una struttuta di spazio vettoriale (<mark>cose che vedremo più avanti</mark>)

# <mark>22/03/22</mark>
## <u>Sistemi di equazioni lineari</u> (accenni)

Equazione lineare in $n$ incognite:

$x_1,\cdots,x_n: a_1x_1+a_2x_2+\cdots+a_nx_n=b\\a_i\in\mathbb{R},\forall i,b\in\mathbb{R}$

Sistema di $n$ equazioni lineari in $n$ incognite:
$\begin{cases}a_{11}x_1+a_{12}+\cdots+a_{1n}x_n=b_1\\
a_{21}x_1+a_{22}+\cdots+a_{2n}x_n=b_2\\
\cdots\\
a_{n1}x_1+a_{n2}+\cdots+a_{nn}x_n=b_n\\\end{cases}$

Una soluzione del sistema di sopra è un vettore $(x_1,\cdots,x_n)\in\mathbb{R}^n$ che verifica tutte le equazioni.

<u>Esempi</u>:

$\begin{cases}x+y+z=6\\2x-y=0\end{cases}$

<u>Una</u> soluzione di questo sistema è $(1,2,3)\in\mathbb{R}^3$

<u>Domanda</u>:

Supponiamo di avere un sistema lineare:

1. Esiste almeno una soluzione?
2. "Quante" sono?
3. Come si interpreta geometricamente il corrispondente insieme di soluzioni?

## <u>Matrici</u>
- Un esempio di spazio vettoriale
- Uno strumento conciso per rappresentare oggetti *parola incomprensibile*, tra cui molti dell'algebra lineare

Sia $\mathbb{K}$ un campo.
Siano $m,n\ge1$ due numeri

<u>Def</u>: Una matrice $m\times n$ a elementi in $\mathbb{K}$ è una tabella rettangolare di $m\cdot n$ elementi di $\mathbb{K}$, disposti su $m$ righe e $n$ colonne

<u>Notazione</u>:

$A=\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{ij} & \cdots & a_{1n}\\
a_{21} & a_{22} & \cdots & a_{ij} & \cdots & a_{2n}\\
\vdots\\
a_{i1} & a_{i2} & \cdots & a_{ij} & \cdots & a_{in}\\
\vdots\\
a_{n1} & a_{n2} & \cdots & a_{nj} & \cdots & a_{nn}\\
\end{bmatrix}$

$(a_{ij})_{1\le i \le n\ \wedge\ 1\le j \le n}$: $i$ è la riga e $j$ è la colonna, come in c++ (o qualunque linguaggio "normale")

Ciascuno degli elementi $a_{ij}$ è detto entrata (o coefficiente) dellel matrici

<u>Un po' di terminologia</u>

- Se $n=m$, una matrice $n\times n$ si dice matrice <u>quadrata</u> di ordine $n$

  Ha due diagonali (solo se è quadrata eh)
- Una matrice $1\times n$ è chiamata vettore riga.

  Una matrice $n\times1$ è chiamata vettore colonna.

<u>Notazione</u>:
$M_{m,n}(K)=\{$matrici $n\times m$ a coefficienti in $K\}$

M$_{n}(K):=\{$matrici quadrete di ordine $n\}$

<u>Def</u>: Siano $A=(a_{ij}),\ B=(b_{ij})\in M_{m,n}(K)$.

Diciamo che $A=B$ se $a_{ij}=b_{ij}\forall 1\le i \le n,\ 1\le j \le n$

Definiamo due operazioni su $M_{m,n}$
- <u>Somma di matrici</u>

  $+: M_{m,n}\times M_{m,n}\rightarrow M_{m,n}(K)\\(A,B)\longmapsto A+B$

  $A=\begin{bmatrix}
  a_{11} & \cdots & a_{1n}\\
  \vdots\\
  a_{m1} & \cdots & a_{mn}\\
  \end{bmatrix}=(a_{ij})\in M_{m,n}(K)$

  $B=\begin{bmatrix}
  b_{11} & \cdots & b_{1n}\\
  \vdots\\
  b_{m1} & \cdots & b_{mn}\\
  \end{bmatrix}=(b_{ij})\in M_{m,n}(K)$

  $A+B:=\begin{bmatrix}
  a_{11}+b_{11} & \cdots & a_{1n}+b_{1n}\\
  \vdots\\
  a_{m1}+b_{m1} & \cdots & a_{mn}+b_{mn}\\
  \end{bmatrix}=(a_{ij}+b_{ij})$ <mark>incompleto</mark>, probabilmente $\in M_{m,n}(K)$
- <u>Moltiplicazione per scalari</u>

  $\cdot:K\times M_{m,n}(K)\rightarrow M_{m,n}(K)\\(\lambda,A)\longmapsto\lambda\cdot A$

  $A=(a_{ij})\in M_{m,n}(K)\\\lambda\in K$

  $\lambda\cdot A=(\lambda a_{ij})\in M_{m,n}(K)$

<u>Proprietà</u>:
1. $+$ è commutativa: $A+B=B+A$
2. $+$ è associativa: $(A+B)+C=A+(B+C)$
3. Elemento neutro rispetto a $+$:

   $0_{m,n}=\begin{bmatrix}0&\cdots&0\\\vdots\\0&\cdots&0\end{bmatrix}$
4. Elemento opposto rispetto a $+$:
   $A=(a_{ij})\Rightarrow-A=(-a_{ij})$
5. $\lambda\cdot(A+B)=\lambda\cdot A + \lambda\cdot B$
6. $(\lambda+\mu)\cdot A=\lambda\cdot A+\mu\cdot A$
7. $(\lambda\mu)\cdot A=\lambda\cdot(\mu\cdot A)$
8. $1\cdot A = A$
  $\forall m,n\ge1$ interi, $(M_{m,n}(K),+,\cdot)$ è uno spazio vettoriale su $\mathbb{K}$

<u>Prodotto di matrici</u> (prodotto riga per colonna):

$(a_1\cdots\ a_n)\in M_{1,n}(K):$ vettore riga

$(b_1\cdots\ b_n)\in M_{n,1}(K):$ vettore colonna

$(a_1\cdots\ a_n)\cdot(b_1\cdots\ b_n):=a_1b_1+\cdots+a_nb_n=\sum^n_{k=1}{a_kb_k}$

Generalizziamo al prodotto di due matrici

$\begin{bmatrix}
a_{11}&\cdots&a_{1n}\\
a_{m1}&\cdots&a_{mn}
\end{bmatrix}
\cdot
\begin{bmatrix}
b_{11}&\cdots&b_{1p}\\
b_{q1}&\cdots&b_{qp}
\end{bmatrix}=
\begin{bmatrix}
c_{ij}
\end{bmatrix}$

$c_{ij}=$prodotto della $i$-esima riga di $A$ e della $j$-esima colonna di $B$

Per definire il prodotto abbiamo bisogno che $n=q$

$\forall\ 1\ge i\ge n,\ \forall\ 1\ge j\ge p$ definiamo

$c_{ij}=(a_{i1}\cdots a_{in})\cdot(b_{1j}\cdots b_{nj})=a_{i1}b_{1j}+\cdots+a_{in}b_{nj}=\sum^n_{n=1}{a_{ik}b_{kj}}$

Più formalmente, il prodotto di due matrici è una funzione:

$M_{m,n}(K)\times M_{n,p}(K)\rightarrow M_{m,p}(K)\\(A,B)\longmapsto C=AB$

$A=(a_{ij}): 1\le i\le m,\ 1\le j\le n$

$B=(b_{ij}): 1\le i\le n,\ 1\le j\le p$

$C=AB=(c_{ij}): 1\le i\le m,\ 1\le j\le p$

<mark><u>NOTA BENE</u></mark>: il prodotto è definito se e solo se il numero di colonne di $A$ è uguale al numero di righe di $B$.

<u>Caso particolare</u>

$n=p=m:$ otteniamo un'operazione binaria interna su $M_n(K)$

# <mark>23/03/22</mark>

## Operazioni tra matrici
### <u>Proprietà</u>
1. Non è commutativa

    Due matrici quadrate $A,B\in M_n(K)$ <u>commutano</u> se $AB=BA$.
2. È <u>associativa</u>

    $\forall A\in M_{m,n}(K),\forall B\in M_{n,P}(K),\forall C\in M_{P,q}(K)\\(AB)C=A(BC)$
3. È distributiva rispetto a $+$

   $\forall A,B\in M_{m,n}(K), \forall C\in M_{n,P}(K),\forall D\in M_{n,P}(K)\\(A+B)C=AC+BC\\A(C+D)=AC+AD$
4. Due elementi neutri, uno a destra e uno a sinistra (perchè $\cdot$ non è commutativa).
   - a destra: $I$ tale che $AI=A, \forall A\in M_{m,n}(K)$
   - a sinistra: $I$ tale che $IA=A, \forall A\in M_{m,n}(K)$

    $\begin{bmatrix}
    a&b&c\\
    d&e&f\\
    \end{bmatrix}\cdot
    \begin{bmatrix}
    a'&b'&c'\\
    d'&e'&f'\\
    g'&h'&i'\\
    \end{bmatrix}=
    \begin{bmatrix}
    a&b&c\\
    d&e&f\\
    \end{bmatrix}\Rightarrow
    \begin{cases}
    aa'+bd'+cd'=a\rightsquigarrow a'=1,\ d'=0,\ g'=0\\
    ab'+be'+ch'=b\rightsquigarrow b'=0,\ d'=0,\ g'=0\bigcirc incompleto\ \bigcirc
    \end{cases}\\\vdots\\
    \begin{bmatrix}
    a'&b'&c'\\
    d'&e'&f'\\
    g'&h'&i'\\
    \end{bmatrix}=
    \begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}$

    <u>Def</u>: $\forall n\ge1$, la matrice <u>unità</u> o <u>identità</u>di ordine $n$ è

    $I_n=(\delta_{ij})_{1\le i\le n,\ 1\le j\le n}$

    dove

    $\delta_{ij}=\begin{cases}1\ se\ i=j\\0\ se\ i\not=j\end{cases}$

    Quindi $\forall A\in M_{m,n}(K)$ abbiamo:

      $I_mA=A\\AI_n=A,$

    Cioè $I_m$ è l'elemento neutro a sinistra e $I_n$ è l'elemento neutro a destra.

    <u>N.B.</u>: $\forall a,b\in\mathbb{R},\ (a+b)^2=a^2+2ab+b^2$ perchè in $\R$, la moltiplicaizone è commutativa.
    - $\forall A,B\in M_n(\R)\\(A+B)^2=\\(A+B)(A+B)=\\(A+B)A+(A+B)B=\\A^2+BA+AB+B^2$

      non si può semplificare perchè nelle matrici il prodotto <u>non</u> è commutativo

    - Se $A\in M_n(K),\forall K\ge1$, denotiamo $A^K=A\cdot A$

Lavoriamo ora con $M_n(K)\rightsquigarrow M_n(K)\times M_n(K)\rightarrow M_n(K)\\(A,B)\longmapsto AB$
In questo caso $I_n$ è l'elemento neutro (a destra e a sinistra) rispetto al prodotto.

<u>Def</u>: $A\in M_n(K)$ si dice <u>invertibile</u> se $\exist B\in M_n(K)$ tale che

$AB=BA=I_n$

<u>Osservazioni</u>
1. Se B esiste allora è unica.

    <u>Dim</u>.
    Se $C$ è tale che $AC=I_n=CA$, allora:

    $B=BI_n=B(AC)=(BA)C=I_nC=C\Rightarrow B=C$

    Chiamiamo $B$ l'<u>inversa</u> di $A$ e la denotiamo $A^{-1}$.
2. Se $B$ soddisfa $AB=I_n$ o $BA=I_n$ allora $B=A^{-1}$  

    <u>Esempi</u>
    - $I_n$ e invertibile e $I_n^{-1}=I_n$
    - $O_n=\begin{bmatrix}0&\cdots\ \ \ 0\\\vdots&\ \ \ \ \ \ \ \vdots\\0&\cdots\ \ \ 0\end{bmatrix}$

    - $A=\begin{bmatrix}1&1\\1&1\end{bmatrix}\in M_2(\R)\\\exist B=\begin{bmatrix}a&b\\c&d\end{bmatrix}\in M_2(\R)$ <mark>Incompleto</mark>
    - $A=\begin{bmatrix}1&2\\3&4\end{bmatrix}$

      $\begin{bmatrix}a&b\\c&d\end{bmatrix}\cdot\begin{bmatrix}1&2\\3&4\end{bmatrix}=\begin{bmatrix}1&0\\0&1\end{bmatrix}\Rightarrow\begin{cases}a+3b=1\\2a+4b=0\\c+3d=0\\2c+4d=1\end{cases}\Rightarrow\begin{cases}-2b+3b=1\\a=-2b\\c=-3d\\-6d+4d=1\end{cases}\Rightarrow\\\Rightarrow\begin{cases}b=1\\a=-2\\c=\frac{3}{2}\\d=-\frac{1}{2}\end{cases}$

      Quindi $A^{-1}=\begin{bmatrix}-2&1\\\frac{3}{2}&-\frac{1}{2}\end{bmatrix}$

      <u>Osservazione</u>: Supponiamo che $A$ sia invertibile.

      $\exist A^{-1}$

      Sia $B$ una matrice tale che

      $AB=I_n$

      Voglio dimostrare che $BA=I_n$

      $BA=I_nBA=A^{-1}ABA=A^{-1}I_nA=A^{-1}A=I_n$

<u>Proposizione</u>: Siano $A,B\in M_n(K)$ invertibili.

  Allora $AB$ è invertibile e $(AB)^{-1}=B^{-1}A^{-1}$

<u>Dim</u>

Infatti:

$(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AI_nA^{-1}=AA^{-1}=I_n$

## Altra terminologia
<u>Def</u>: Sia $A=(a_{ij})\in M_{m\times n}(K)$.

La <u>trasposta</u> di $A$ è la matrice $n\times m$:

$A^T=(a_{ji})=\begin{bmatrix}
a_{11}&a_{21}&\cdots&a_{m1}\\
a_{12}&a_{22}&\cdots&a_{m2}\\
\vdots\\
a_{1n}&a_{2n}&\cdots&a_{mn}
\end{bmatrix}\in M_{n,m}(K)$

<u>Esempio</u>:

$A=\begin{bmatrix}
1&2&3\\4&5&6
\end{bmatrix}\ A^T=\begin{bmatrix}
1&4\\2&5\\3&6
\end{bmatrix}$

<u>Def</u>: Una matrice quadrata $A\in M_n(K)$ si dice simmetrica se $A^T=A$.

Se invece $A^T=-A$, $A$ si dice *anti*simmetrica.

<u>Esempio</u>:

$A=\begin{bmatrix}
1&2&3&4\\
2&5&6&7\\
3&6&8&9\\
4&7&9&10
\end{bmatrix}\ A^T=\begin{bmatrix}
1&2&3&4\\
2&5&6&7\\
3&6&8&9\\
4&7&9&10
\end{bmatrix}$

<u>Osservazione</u>: se $A=(a_{ij})$ è antisimmetrica $\Rightarrow$

$a_{ij}=-a_{ji}\ \forall i,j$,

Quando $i=j,\ a_{ii}=a_{ii}\Rightarrow2a_{ii}=0\Rightarrow a_{ii}=0$

<u>Def</u>: Una matrice quadrata $A\in M_n(K)$ si dice <u>ortogonale</u> se $(A^T)A=I_n=A(A^T)\rightsquigarrow A^{-1}=A^T$

<u>Esempio</u>: $\forall\theta\in\mathbb{R}$ la matrice

$\begin{bmatrix}
cos(\theta)&-sin(\theta)\\sin(\theta)&cos(\theta)  
\end{bmatrix}$ è ortogonale.

---
$\begin{bmatrix}
1&0&0\\3&2&0\\4&5&6
\end{bmatrix}$ triangolare inferiore

$\begin{bmatrix}
-2&0&7&0\\0&1&-8&0\\
0&0&0&5\\0&0&0&\pi
\end{bmatrix}$ triangolare superiore

$\begin{bmatrix}
1&0\\0&-3
\end{bmatrix}$ diagonale

$\begin{bmatrix}
3&0&0\\0&3&0\\0&0&3
\end{bmatrix}$ scalare

<u>Def</u>: Una matrice quadrata $A\in M_n(K)$ si dice:
- triangolare inferiore (risp. superiore) se $a_{1j}=0$ se $j>i$ (risp. se $j< i$)
- diagonale se è al tempo stesso triangolare superiore e triangolare inferiore, ossia se $a_{ij}=0\forall i\not=j$
- scalare se $A$ è diagonale con tutti gli elementi uguali sulla diagonale, cioè:

  $A=\lambda I_n, \lambda\in K$.
# <mark>29/03/22</mark>
## Sistemi di equazioni lineari
<u>Def</u>: Siano $x_1,\cdots,x_n$ n indeterminante.

Un'<u>equazione lineare</u> nelle indeterminate $x_1,\cdots,x_n$ a coefficienti in $\mathbb{K}$ è un'equazione della forma:

  (*) $a_1x_1+a_2x_2+\cdots+a_nx_n=b, a_i\in K\forall i,\ b\in K$

  Una <u>soluzione</u> di (*) è un elemento $(x_1,\cdots,x_n)\in K^n$ che sostituito alla $n$-upla $(x_1,\cdots,x_n)$ dà luogo ad un'identità.

  L'equazione (*) si dice <u>omogenea</u> (risp non omogenea) se $b=0$ (se $b\not=0$).

<u>Sistema di eq lineari</u>: consideriamo simmetricamente un eq. lineari in $x_1,\cdots,x_n$.

$\begin{cases}
a_{11}x_1+a_{12}x_2+\cdots+a_{1n}=b_1\\
a_{21}x_1+a_{22}x_2+\cdots+a_{2n}=b_2\\
\vdots\\
a_{m1}x_1+a_{m2}x_2+\cdots+a_{mn}=b_m\\
\end{cases}$

$a_{ij}$ equazione $i$-esima, variabile $x_j$

<u>Def</u>: il sistema (**) si deice omogeneo (risp non omogeneo) se $b_i=0\ \forall i$ (se $\exist i\in\{1,\cdots,m\}$)

<u>Def</u>:
- Una soluzione di (**) è un elemento $(x_1,\cdots,x_n)\in K^n$ che è soluzione simultanea di tutte le eq. lineari.
- Un sistema si dice <u>compatibile</u> se possiede almeno una soluzione. Si dice <u>incompatibile</u> se non possiede soluzioni.
- Due sistemi si dicono <u>equivalenti</u> se hanno lo stesso sistema di soluzioni.


<u>Esempi</u> $(K=\R)$:
1. Un sistema omogeneo in $n$ indeterminante è sempre compatibile in quanto $(0,\cdots,0)\in K^n$ è sempre soluzione.
2. non lo segno
3. $\begin{cases}x_1+x_2=0\\x_1-x_2=1\end{cases}$

    "addizionando le due equazioni" otteniamo:

    $x_1+x_2+(x_1-x_2)=0+(1)\Rightarrow2x_1=1\Rightarrow x_1=\frac{1}{2}$

    sostituendo $x_1=\frac{1}{2}$ nella I equazione, trovo $x_2=-\frac{1}{2}$.

    Quindi il sistema possiede l'unica soluzione $(\frac{1}{2},-\frac{1}{2})\in\mathbb{R}^2$
4. $\begin{cases}x_1+x_2=2\\3x_1-3x_2=6\end{cases}$

    è compatibile e possiede infinite soluzioni date dalle soluzioni di

    $x_1+x_2=2\Rightarrow x_1=2-x_2$

    L'insieme delle soluzioni $S$ è costituito dalle coppie ordinate $(x_1,x_2)\in\mathbb{R}^2$ tali che:

    $\begin{cases}x_1=2-t\\x_2=t\end{cases},\ t\in\mathbb{R}\\S=\{(2-t,t),\ t\in\mathbb{R}\}\subseteq\mathbb{R}^2$

<u>Notazione matriciale di un sistema</u>:

$\begin{cases}
a_{11}x_1+\cdots+a_{1n}x_n=b_1\\
\vdots\\
a_{m1}x_1+\cdots+a_{mn}x_n=b_m
\end{cases}$

$A=(a_{ij})=\begin{bmatrix}
a_{11}&\cdots&a_{1n}\\
\vdots\\
a_{m1}&\cdots&a_{mn}
\end{bmatrix}\in M_{m,n}(K)$

Vettore (colonnna) della indeterminante:
$x=\begin{bmatrix}x_1\\\vdots\\x_n\end{bmatrix}$

Vettore dei termini noti: $b=\begin{bmatrix}b_1\\\vdots\\b_n\end{bmatrix}\in M_{m,1}(K)$

Riscriviamo (**) come:
$AX=b$

La matrice: $(A\ \vdots\ b)=\begin{bmatrix}
a_{11}&a_{1n}&\vdots&b_1\\
\vdots&&\vdots&\vdots\\
a_{m1}&a_{mn}&\vdots&b_m\\
\end{bmatrix}$

Consideriamo il sistema seguente:

$\begin{cases}
x_1+x_2+x_3=3\\
2x_2-x_3=1\\
3x_3=-3
\end{cases}$

La sua matrice orlata:

$\begin{bmatrix}
1&1&1&\vdots&3\\
0&2&-1&\vdots&1\\
0&0&3&\vdots&-3\\
\end{bmatrix}$

Risolvo per sostituzione:

$\begin{cases}
x_1=4\\
x_2=0\\
x_3=-1
\end{cases}$

Procedendo dal basso verso l'alto trovo che il sistema possiede l'unica soluzione $(4,0,-1)\in\mathbb{R}^3$

Un sistema di questo tipo è detto "a scalini" o "a gradini".

<u>Def</u>: Una <u>matrice a scalini</u> (o a gradini) è una matrice avente le seguenti proprietà:
1. Ogni riga, dopo la prima, inizia con almeno uno zero in più rispetto alla riga precedente
2. Se una riga è nulla allora ogni riga sottostante è nulla

Il primo elemento <u>diverso da zero</u> su ogni riga (se presente) è detto <u>pivot</u>.

<u>Def</u>: Un sistema lineare si dice <u>a scalini</u> (o a gradini) se la sua matrice orlata è una matrice a scalini.

Esempi:
1. $\begin{bmatrix}
1&1&1&\vdots&3\\
0&2&-3&\vdots&1\\
0&0&3&\vdots&-3
\end{bmatrix}$ è una matrice a scalini.

    pivot: $1,2,3$
2. $\begin{bmatrix}
1&-1&2&4&5&&\vdots&3\\
0&2&-3&\vdots&1\\
0&0&3&\vdots&-3
\end{bmatrix}$ è una matrice a scalini.
# <mark>INCOMPLETO: SI È SPENTO IL PC</mark>
# <mark>30/03/22</mark>
## Sistema lineare $\longrightarrow$ sistema a scalini.
### Algoritmo (o metodo di eliminazione) di Gauss-Jordan.
Tale metodo consiste nell'effettuare delle operazioni successive sulle equazioni del sistema (o equivalentemente sulle righe della matrice orlata) che non ne alterino l'insieme delle soluzioni.

<u>Operazioni elementari</u>:

$(*)=\begin{cases}
  a_1x_1+\cdots+a_nx_n=b\\
  a_{1'}x_1+\cdots+a_{n'}x_n=b'
\end{cases}$

1. Il sistema (*) è equivalente a:

   $(**)=\begin{cases}
      a_{1'}x_1+\cdots+a_{n'}x_n=b'\\
      a_1x_1+\cdots+a_nx_n=b
   \end{cases}$

   Scambiare tra loro due equazioni di un sistema non cambia l'insieme delle soluzioni.
2. Il sistema (*) di partenza è equivalente a:

   $(**)=\begin{cases}
      \lambda a_1x_1+\cdots+\lambda a_nx_n=\lambda b\\
      a_{1'}x_1+\cdots+a_{n'}x_n=b'
   \end{cases},\ \lambda\not=0,\ \lambda\in\mathbb{K}$

   Moltiplicare (primo e secondo membro) per uno scalare non nullo non cambia l'insieme delle soluzioni:

   $(x_1,\cdots,x_n)$ è soluzione di $a_1x_1+\cdots+a_nx_n=b$

   $(x_1,\cdots,x_n)$ è soluzione di $\lambda a_1x_1+\cdots+\lambda a_nx_n=\lambda b$
3. Il sistema (*) è equivalente al sistema in cui un'equazione è sostituita con quella ottenuta sommando ad essa un multiplo di un'altra equazione:

   $(**)=\begin{cases}
      a_1x_1+\cdots+a_nx_n+\lambda(a_{1'}x_1+\cdots+a_{n'}x_n)=b+\lambda b'\\
      a_{1'}x_1+\cdots+a_{n'}x_n=b'
   \end{cases}$

   <u>Dim</u>:

   $(x_1,\cdots,x_n)$ è soluzione di $(*)\Leftrightarrow(x_1,\cdots,x_n)$ è soluzione di $(**)$

   $\Rightarrow)$ Assumiamo che $(x_1,\cdots,x_n)$ è soluzione di (*)

    $a_1x_1+\cdots+a_nx_n=b\\a_{1'}x_1+\cdots+a_{n'}x_n=b'$

    $b=a_1x_1+\cdots+a_nx_n\\b'=a_{1'}x_1+\cdots+a_{n'}x_n$

    $b+b'=b+\lambda b'$

    Sostituisco $b$ e $b'$

    $a_1x_1+\cdots+a_nx_n+\lambda(a_{1'}x_1+\cdots+a_{n'}x_n)=b+\lambda b'$

    $\Leftarrow)\ (x_1,\cdots,x_n)$ è soluzione di $(**)\Rightarrow\cdots(x_1,\cdots,x_n)$ è soluzione di (*)
#### Operazioni elementari sulle equazioni di un <u>sistema</u>
. Scambiare tra loro due equazioni del sistema

II. Moltiplicare un'equazione per uno scalare <u>non nullo</u>

III. Sostituire un'equazione con quella ottenuta "sommando" ad essa un multiplo di un'altra equazione

#### Operazioni elementari sulle righe di una <u>matrice</u>
I. Scambiare tra loro due righe di una matrice

$R_i\leftrightarrow R_j:
\begin{bmatrix}
1&2&3&4\\
5&6&7&8\\
9&10&11&12
\end{bmatrix}\xRightarrow{R_1\leftrightarrow R_3}\begin{bmatrix}
9&10&11&12\\
5&6&7&8\\
1&2&3&4
\end{bmatrix}$

II. Moltiplicare una riga della matrice per uno scalare non nullo:

$R_i\leftarrow\lambda R_i:
\begin{bmatrix}
1&2&3&4\\
5&6&7&8\\
9&10&11&12
\end{bmatrix}\xRightarrow{R_1\leftarrow2R_1}\begin{bmatrix}
2&4&6&8\\
5&6&7&8\\
9&10&11&12
\end{bmatrix}$


III. Sostituire una riga della matrice con quella ottenuta sommando ad essa un multiplo di un'altra riga:

$R_i\leftarrow R_i\lambda R_j:
\begin{bmatrix}
9&10&11&12\\
5&6&7&8\\
1&2&3&4
\end{bmatrix}\xRightarrow{R_1\leftarrow R_1-9R_3}\begin{bmatrix}
0&-8&-16&-24\\
5&6&7&8\\
1&2&3&4
\end{bmatrix}$

#### Algoritmo di Gauss-Jordan:
Successione di operazioni elementari che permettono di trasformare il sistema (o la corrispondente matrice orlata) in un sistema a scalini (in una matrice a scalini) equivalente al sistema di partenza.

<u>Esempio</u>:

$\begin{bmatrix}
  1&2&3&4\\
  5&6&7&8\\
  9&10&11&12
\end{bmatrix}\xRightarrow{R_2\leftarrow R_2-5R_1}
\begin{bmatrix}
  1&2&3&4\\
  0&-4&-8&-12\\
  9&10&11&12
\end{bmatrix}\xRightarrow{R_3\leftarrow R_3-9R_1}$

$\begin{bmatrix}
  1&2&3&4\\
  0&-4&-8&-12\\
  0&-8&-16&-24
\end{bmatrix}\xRightarrow{R_3\leftarrow R_3-2R_2}
\begin{bmatrix}
  1&2&3&4\\
  0&-4&-8&-12\\
  0&0&0&0
\end{bmatrix}$

<u>NB</u>: L'output dell'algoritmo non è unico perchè dipende dalle scelte effettuate

#### Risoluzione di un sistema lineare con il metodo di eliminazione di Gauss-Jordan

Supponiamo di avere un sistema lineare qualsiasi:

1. Scriviamo la corrispondente matrice orlata $\mathbb{A}$
2. Utilizziamo l'algoritmo di Gauss-Jordan per ottenere da $\mathbb{A}$ una matrice $\mathbb{B}$ a scalini equivalente per righe
3. Se l'ultimo pivot di $\mathbb{B}$ appartiene all'ultima colonna, il sistema non è compatibile.
4. Scriviamo il sistema a scalini corrispondente a $\mathbb{B}$ e lo risolviamo introducendo delle eventuali variabili libere

<u>Esempio</u>:
1. Con numeri:
   1.  $\begin{cases}
         x_3+2x_4=3\\
         2x_1+4x_2-2x_3=4\\
         2x_1+4x_2-x_3+2x_4=7
       \end{cases}\Rightarrow
       \begin{bmatrix}
         0&0&1&2&3\\
         2&4&-2&0&4\\
         2&4&-1&2&7
       \end{bmatrix}\xRightarrow{R_1\leftrightarrow R_2}$

   2.  $\begin{bmatrix}
         2&4&-2&0&4\\
         0&0&1&2&3\\
         2&4&-1&2&7
       \end{bmatrix}\xRightarrow{R_3\leftarrow R_3-R_1}
       \begin{bmatrix}
         2&4&-2&0&4\\
         0&0&1&2&3\\
         0&0&1&2&3
       \end{bmatrix}\xRightarrow{R_3\leftarrow R_3-R_2}$

       $\begin{bmatrix}
         2&4&-2&0&4\\
         0&0&1&2&3\\
         0&0&0&0&0
       \end{bmatrix}$
   3. È compatibile (l'ultimo pivot (1) non appartiene all'ultima colonna).

      Variabili libere: $x_2,\ x_4$

      Risolvo:

      $\begin{cases}
       2x_1+4x_2-2x_3=4\\
       x_3+2x_4=3\\
       0=0
      \end{cases}\Rightarrow
      \begin{cases}
       2x_1+4x_2-2x_3=4\\
       x_3=3-2x_4
      \end{cases}\Rightarrow
      \begin{cases}
       2x_1+4x_2-6-4x_4=4\\
       x_3=3-2x_4
      \end{cases}\Rightarrow
      \begin{cases}
       x_1=5-2s-2t\\
       x_2=s\\
       x_3=3-2t\\
       x_4=t
      \end{cases}s,t\in\mathbb{R}$

      $\mathbb{S}=\{(5-2s-2t,s,3-2t,t),\ s,t\in\mathbb{R}\}:\infty^2$ soluzioni
2. Con parametro: <mark>INCOMPLETO</mark>
    1. $\Rightarrow\begin{pmatrix}
         a&-a&0&1&1-a\\
         1&-2&-1&0&0\\
         0&1&a&1&a-1
       \end{pmatrix}$
    2. $\xRightarrow{R_1\leftrightarrow R_2}
       \begin{pmatrix}
         1&-2&-1&0&0\\
         a&-a&0&1&1-a\\
         0&1&a&1&a-1
       \end{pmatrix}\xRightarrow{R_2\leftrightarrow R_2-aR_1}
       \begin{pmatrix}
         1&-2&-1&0&0\\
         0&a&a&1&1-a\\
         0&1&a&1&a-1
       \end{pmatrix}\xRightarrow{R_2\leftrightarrow R_3}$

       $\begin{pmatrix}
         1&-2&-1&0&0\\
         0&1&a&1&a-1\\
         0&a&a&1&1-a
       \end{pmatrix}\xRightarrow{R_3\leftrightarrow R_3-aR_2}
       \begin{pmatrix}
         1&-2&-1&0&0\\
         0&1&a&1&a-1\\
         0&0&a-a^2&1-a&1-a^2
       \end{pmatrix}\leftarrow$ a scalini $\forall a$

       $a-a^2=0\Leftrightarrow a=0\vee a=1$

       $a=0\rightarrow
       \begin{pmatrix}
         1&-2&-1&0&0\\
         0&1&0&1&-1\\
         0&0&0&1&1
       \end{pmatrix}\leftarrow$ compatibile

       $a=1\rightarrow
       \begin{pmatrix}
         1&-2&-1&0&0\\
         0&1&1&1&0\\
         0&0&0&0&0
       \end{pmatrix}\leftarrow$ compatibile

       $a\not=0,\ a\not=1\\
       \begin{pmatrix}
        1&-2&-1&0&0\\
        0&1&a&1&a-1\\
        0&0&a-a^2&1-a&1-a^2
       \end{pmatrix}\rightarrow
       \begin{cases}
        x_1-2x_2-x_3=0\\
        x_2+ax_3=a-1-x_4\\
        (a-a^2)x_3=1-a^2-(1-a)x_4
       \end{cases}$

# <mark>05/04/22</mark>
## Ultime considerazioni sui sistemi lineari
$(*)AX=b,A\in M_n(K),b\in M_{n,1}(K)$,

A invertibile.

$\Updownarrow$

$\exist A^{-1}\in M_(K): A^{-1}A=AA^{-1}=In$

Quindi abbiamo:

$A^{-1}AX=A^{-1}b\Leftrightarrow InX=A^{-1}b\Leftrightarrow X=A^{-1}b$

<u>Proposizione</u> (metodo dell'inversa)

Sia $A\in M_n(K)$ una matrice <u>invertibile</u> e $b\in M_{n,1}(K)$. Allora il sistema

$AX=b$

possiede l'unica soluzione $X=A^{-1}b$

### Come si calcola l'inversa di una matrice?

L'algoritmo di Gauss-Jordan offre un metodo efficiente per il calcolo dell'inversa di una matrice.

<u>Idea</u>:

$\begin{pmatrix}
  1&2&3\\
  4&5&6\\
  7&8&9\\
\end{pmatrix}\xLeftrightarrow{R_3\leftarrow R_3-7R_1}
\begin{pmatrix}
  1&2&3\\
  4&5&6\\
  0&-6&-12\\
\end{pmatrix}$

$\begin{pmatrix}
  1&0&0\\
  0&1&0\\
  0&0&1
\end{pmatrix}\rightarrow
\begin{pmatrix}
  1&0&0\\
  0&1&0\\
  -7&0&1
\end{pmatrix}$

$\begin{pmatrix}
  1&0&0\\
  0&1&0\\
  -7&0&1
\end{pmatrix}
\begin{pmatrix}
  1&2&3\\
  4&5&6\\
  7&8&9\\
\end{pmatrix}=
\begin{pmatrix}
  1&2&3\\
  4&5&6\\
  0&-6&-12\\
\end{pmatrix}$

$A\in M_n(K)$

$P_r\cdots P_2P_1A=In$

$(A\quad\vdots\quad In)\rightarrow(In\quad\vdots\quad A^{-1})$

Sistema lineare omogeneo a coefficienti in $\mathbb{K}$

$(*)\begin{cases}
  a_{11}x_1+\cdots+a_{1n}x_n=0\\
  \vdots\\
  a_{m1}x_1+\cdots+a_{mn}x_n=0\\
\end{cases}$

$S_0$: insieme delle soluzioni di (*)

$S_0$ è un sottoinsieme di $K^n$ con qualche interessante proprietà.
1. <u>0</u>$=(0,\cdots,0)\in S_0$ (il vettore nullo è sempre soluzione di un sistema omogeneo) $\Rightarrow S_0\not=0$
2. Se $(x_1,\cdots,x_n),(y_1,\cdots,y_n)\in S_0\Rightarrow(x_1,\cdots,x_n)+(y_1,\cdots,y_n)\in S_0$

   <u>Dim</u>:

   Se $(x_1,\cdots,x_n),(y_1,\cdots,y_n)\in S_0$

   $\Updownarrow$

   $\forall i,a_{i1}x_1+\cdots+a_{in}x_n=0,\quad a_{i1}y_1+\cdots+a_{in}y_n=0$

   Mostriamo che $(x_1,\cdots,x_n)+(y_1,\cdots,y_n)=(x_1+y_1,\cdots,x_n+y_n)\in S_0$, cioè $(x_1+y_1,\cdots,x_n+y_n)$ verifica $a_{i1}x_1+\cdots+a_{in}x_n=0,\forall i$

   Abbiamo:

    $\forall i\quad a_{i1}(x_1+y_1)+\cdots+a_{in}(x_n+y_n)=\\=a_{i1}x_1+a_{i1}+\cdots+a_{in}x_n+a_{in}y_n=\\=a_{i1}x_1+\cdots+a_{i1}x_n+a_{in}y_1+\cdots+a_{in}y_n$
3. Se $(x_1,\cdots,x_n)\in S_0\Rightarrow\lambda(x_1,\cdots,x_n)\in S_0,\forall\lambda\in\mathbb{K}$

   <u>Dim</u>:

   $(x_1,\cdots,x_n)\in S_0\Rightarrow\forall i\quad a_{i1}x_1+\cdots+a_{in}x_n=0$

   Mostriamo che $\forall\lambda\in K,\quad\lambda(x_1,\cdots,x_n)=(\lambda x_1,\cdots,\lambda x_n)\in S_0:\forall i$ abbiamo: $a_{i1}(\lambda x_1)+\cdots+a_{in}(\lambda x_n)=\lambda(a_{i1}x_1+\cdots+a_{in}x_n)=0$

Le proprietà 1, 2 e 3 fanno di $S_0$ un "sottospazio vettoriale" di $K^n$

Più in generale definiamo:

<u>Def</u>: Sia $V$ uno spazio vettoriale du $K$.

  Un sottioinsieme $w$ di $V\quad(w\subseteq V)$ si dice <u>sottospazio vettoriale</u> se:
1. $w\not=\emptyset$
2. $\forall w_1,w_2\in W:w_1+w_1\in W$
3. $\forall w\in W,\forall\lambda\in K:\lambda w\in W$

<u>Osservazioni</u>:
- La proprietà 3 implica che <u>0</u> $\in W$.

  <u>Dim</u>: $W\not=0\Rightarrow\exists w\in W\xRightarrow{\boxed{3}\ con\ \lambda=0}0\cdot w=$ <u>0</u> $\in W$
- Un sottospazio vettoriale è uno spazio vettoriale:
    - Il vettore nullo <u>0</u> $\in W$ per l'osservazione precedente
    - $\forall w\in W,(-1)\cdot w=-w\in W$
    - Tutte le altre proprietà discendono da $V$ in quanto $W\subseteq V$.

<u>Esempi</u>
1. L'insieme delle soluzioni di un sistema lineare <u>omogeneo</u> a n incognite e a coefficienti in $K$ è un sottospazio vettoriale di $K^n$.
2. $V=K^n\\W=\{(0,x_2,\cdots,x_n):x_i\in K\quad\forall i=2,\cdots,n\}$

   Vediamo che $W$ è un sottospazio vettoriale di $K^n$:
   1. $W\not=\emptyset$, poichè $(0,\cdots,0)\in W$
   2. Siano <u>x</u> $=(0,x_2,\cdots,x_n),$ <u>y</u> $=(0,y_2,\cdots,y_n)\in W$

      Allora

      <u>x</u>$+$<u>y</u> $=(0,x_2,\cdots,x_n)+(0,y_2,\cdots,y_n)=(0,x_2+y_2,\cdots,x_n+y_n)$
  3. Sia <u>x</u> $=(0,x_2,\cdots,x_n)\in W,\quad\lambda\in K$

      Allora $\lambda\cdot$ <u>x</u> $=(0,\lambda x_2,\cdots,\lambda x_n)\in W$

      Nota che $W$ è l'insieme delle soluzioni del sistema lineare omogeneo

      $\begin{cases}x_1=0\end{cases}$
  4. Ogni spazio vettoriale $V$ ha due sottospazi vettoriali "banali":

      $W_1=\{$<u>0</u>$\}$

      $W_2=V$
  5. $V$ spazio vettoriale su $K$

      $v\in V$.

      $W=<v>:=\{\lambda v:\lambda\in K\}$
      1. <u>0</u> $=0\cdot v\in W$
      2. $w_1,w_2\in W\Rightarrow\exists\lambda_1,\lambda_2\in K:w_1=\lambda_1v$ e

          $w_2=\lambda_2v\Rightarrow w_1+w_2=\lambda_1v+\lambda_2v=(\lambda_1+\lambda_2)v\in W$
      3. $w\in W\Rightarrow\exists\lambda\in K:w=\lambda v$

          $\forall\mu\in K\quad\mu w=\mu\lambda v\in W$

          Quindi $W$ è un sottoinsieme vettoriale di $V$ chiamato <u>retta vettoriale</u>

          $V=\mathbb{R}^2,v=(1,1)$

          $W=<v>=\{\lambda(1,1):\lambda\in\mathbb{R}\}=\{(\lambda,\lambda):\lambda\in\mathbb{R}\}=\{(x,y)\in\mathbb{R}^2:y=x\}$ (passa per l'origine)

          Più in generale, $v=(a,b)\in\mathbb{R}^2$ Allora $<v>=\{(\lambda a,\lambda b\lambda\in\mathbb{R}\}$ è la retta passante per l'origine definita dall'equazione $bx-ay=0$
# <mark>06/04/22</mark>
# <mark>Mi sono perso qualcosa, stavo mangiando una pizzetta</mark>
<u>Def</u>: Sia $V$ uno spazio vettoriale su $K$.

Un sottoinsieme $W\subseteq$ <mark>Incompleto</mark>

Def (equivalente): $W\subseteq V$ è un sottospazio vettoriale se e solo se:
1. $W\not=0$
2. $\forall w_1,w_2\in W,\forall\lambda,\mu\in K\\\lambda w_1+\mu w_2\in W$

<u>Esempio</u>:

$V=\mathbb{R}^3$

$w_1=\{(x,y,x)\in\R^3:x,y\in\R\}$

$w_2=\{(x,y,x^2)\in\R^3:x,y\in\R\}$

1. $w_1$ + un sottospazio di $\R^3$
   1. $w_1\not=\emptyset$ poichè $(0,0,0)\in W_1$
   2. $(\forall w_1,w_2\in W_1,\forall\lambda,\mu\ni\R:\qquad\lambda w_1+\mu w_2\in W_1)$

      Siano $w_1,w_2\in W_1$. Allora $\exists x_1,y_1,x_2,y_2\in\R$ tali che $w_1=(x_1,y_1,z_1),w_2=(x_2,y_2,z_2)$.

      $\forall\lambda\mu\in\R$ abbiamo:

      $\lambda w_1+\mu w_2=\lambda(x_1,y_1,z_1)+\mu(x_2,y_2,z_2)=(\lambda x_1+\mu x_2)\lambda y_1+\mu y_2,(\lambda x_1+\mu x_2)=(x',y',z')\in W_1,\\x'=\lambda x_1+\mu x_2\\y'=\lambda y_1+\mu y_2$ <mark>potrebbe essere sbagliato</mark>
2. $w_2=\{(x,y,x^2):x,y\in\R\}$

   $w_1=(3,0,9)$    

   $w_2=(2,1,4)$    

   $\lambda=1\qquad\qquad\lambda w_1+\mu w_2=(1,-1,5)\not\in W_2:\qquad5\not=1^2$

   $\mu=-1$

   $(x_1,y_1,x_1^2)+(x_2,y_2,x_2^2)=(x_1+x_2,y_1+y_2,x_1^2+x_2^2)\Rightarrow\\\Rightarrow(x_1+x_2)^2\not=x_1^2+x_2^2$

<mark>tutte le $u$ e le $w$ sono maiuscole (si me ne sono accorto ora)</mark>
<u>Proposizione</u>: Sia $V$ uno spazio vettoriale su $K$ e siano $u,w\subseteq V$ due sottospazi di $V$. Allora anche $u\cap w$ è un sottospazio vettoriale.

<u>Ricordiamo</u>: $u\cap w=\{V:v\in u$ e $v\in W\}$

<u>Dim</u>:
1. $u\cap w\not=0$ poichè <u>0</u> $\in u$ ($u$ è un sottospazio) e <u>0</u> $\in w$ ($w$ è un sottospazio)
2. $\forall v_1,v_2\in u\cap w,\quad\forall\lambda,\mu\in K$

   Allora $\lambda v_1+\mu v_2\in u\cap W$ (poichè $u$ e $w$ sono sottospazi e $v_1,v_2\in u$ e $v_1,v_2\in W$)

Più in generale dati $n$ sottospazi $w_1,w_n\\w_1\cap\cdots\cap w_n=\bigcap^n_{i=1}w_i$ è un sottospazio.

<u>Attenzione</u>:
1. $u\cup w$ in generale non è un sottospazio

   <u>Esempio</u>:

   $V=\R^2\\u=\{(x,0):x\in\R\}\\w={0,y}:y\in\R$

   $v_1,v_2\in u\cup w:v_1+v_2\not\in u\cup w$

   $v_1=(1,0)\\v_2=(0,1)\\v_1+v_2=(1,1)\not\in u\cup w$

<u>Osservazione</u>: $w\subseteq v$ sottospazio.

Il complementare $V\backslash W=\{v\in V:v\not\in W\}$ non è <u>mai</u> un sottospazio di $V$ perchè <u>0</u> $\not\in V\backslash W\quad($ <u>0</u> $\in W)$

<u>Idea</u>: Vogliamo costruire un sottospazio che contiene due sottospazi di $U$ e $W$

<u>Proposizione</u>: Sia $V$ uno spazio vettoriale su $K$ e siano $U,W$ due sottospazi vettoriali di $V$.

Allora l'insieme:
$$U+W=\{u+w:u\in U,w\in W\}$$
è un sottospazio vettoriale di $V$ chiamato <u>sottospazio somma</u> di $U$ e $W$.

<u>Osservazione</u>: $U\cup W\subseteq U+W$

  Infatti $U\subseteq U+W:\forall u\in U,u=u+$<u>0</u>

  $W\subseteq U+W:\forall w\in W,w=$ <u>0</u>$+w$

<u>Dim</u>:

Facciamo vedere che $u+w$ è un sottospazio di $V$:
1. $u+w\not=0$ poichè <u>0</u> = <u>0</u> $+$ <u>0</u> $\in U+W$
2. Siano $v_1,v_2\in u+w$. Allora $\exists u_1,u_2\in U,w_1,w_2\in W:$

   $v_1=u_1+w_1$

   $v_2=u_2+w_2$

   Siano $\lambda\mu\in K$

   Allora abbiamo:

   $\lambda v_1+\mu v_2=\lambda(u_1+w_1)+\mu(u_2+w_2)=\\=\lambda u_1+\lambda w_1+\mu u_2 + \mu w_2
   =\\=\lambda u_1+\mu u_2+\lambda w_1+\mu w_2\in U+W$

<mark>prof cambia blocco appunti</mark>
$V=\R^2$

$U=<(1,0)>$
<mark>incompleto</mark>

<u>Def</u>: $U,W$ sottospazi di $V$

$U\cap W=\{$ <u>0</u> $\}$ allora $U+W$ è detto SOMMA DIRETTA di $U$ e $W$ e so denota $U\oplus W$.

Se $V=U+W$ (O+) allora $U$ e $W$ si dicono supplementari.
---
Riardiamo: $<(a,b)>=\{\lambda(a,b):\lambda\in\R\}=\{\}$
<mark>incompleto</mark>

<u>Proposizione</u>: Sia $V=U+W$. Allora $V=U+W$ se e solo se ogni elemento di v si scrive in modo unico nella forma $u+w, u\in U, w\in W$.

<u>Dim</u>:

$\Rightarrow)$ Supponiamo che $V=U+W$

Siano $u_1\in U,w_1\in W$ e $u_2\in U,w_2\in W:\quad V=u_1+w_1=u_2+w_2$ (vogliamo far vedere che $u_1=u_2$ e $w_1=w_2$)

- $\Downarrow\\u_1-u_2=u_1-u_2\Rightarrow u_1-u_2\in U\cap W=\{$ <u>0</u> $\}\Rightarrow u_1=u_2$
- $w_1-w_2=w_1-w_2\Rightarrow u_1-u_2\in U\cap W=\{$ <u>0</u> $\}\Rightarrow u_1=u_2$

<mark>incompleto</mark>
# <mark>08/04/22</mark>
<mark>incompleto</mark>
<u>Esempi</u>
1. $V=\R^3$

   $v_1=(1,2,0),\quad v_2=(1,0,1)\in\R^3$

   $v=(-1,4,-3)$ è combinazione lineare di $v_1$ e $v_2$.

   Infatti

   $$2v_1+(-3)v_2=(2,4,0)-(3,0,3)=(-1,4,-3)=v$$
2. $V=\R^3$

   $v_1=(1,2,3),\quad v_2=(3,2,1),\quad v_3=(-1,6,13)\in\R^3$

   <u>Domanda 1</u>: <u>0</u> $=(0,0,0)$ è combinazione lineare di $v_1,\quad v_2$ e $v_3$?

   Si! La combinazione lineare banale restituisce <u>sempre</u> il vettore nullo:

   $0\cdot v_1+0\cdot v_2+0\cdot v_3=$ <u>0</u>

   <u>Domanda 2</u>: esiste una combinazione lineare <u>non banale</u> di $v_1,v_2,v_3$ che restituisce il vettore nullo?

   $\exists\lambda,\mu,\delta\in\R,\quad(\lambda,\mu,\delta)\not=(0,0,0)$ tali che $\lambda v_1+\mu v_2+\delta v_3=$ <u>0</u>?

   $\lambda(1,2,3)+\mu(3,2,1)+\delta(-1,6,13)=(0,0,0)\Rightarrow$
   
   $\Rightarrow(\lambda+3\mu-\delta,2\lambda+2\mu+6\delta,3\lambda+\mu+13\delta)\Rightarrow$
   
   $\Rightarrow
   \begin{cases}
    \lambda+3\mu-\delta=0\\
    2\lambda+2\mu+6\delta=0\\
    3\lambda+\mu+13\delta=0\\
   \end{cases}$ sistema lineare <u>omogeneo</u>

   $\begin{pmatrix}
     1&3&-1&0\\
     2&2&6&0\\
     3&1&13&0
   \end{pmatrix}\xrightarrow{R_2\leftarrow-2R_1\wedge R_3\leftarrow R_3-3R_1}
   \begin{pmatrix}
   1&3&-1&0\\
   0&-4&8&0\\
   0&-8&16&0
   \end{pmatrix}\xrightarrow{R_3\leftarrow R_3-2R_2}
   \begin{pmatrix}
   1&3&-1&0\\
   0&-4&8&0\\
   0&0&0&0
   \end{pmatrix}$

   $\begin{cases}
     \lambda+3\mu-\delta=0\\
     -4\mu+8\delta=0
   \end{cases}\Rightarrow
   \begin{cases}
   \lambda=-3\mu+\delta=-5\delta\\
   \mu=2\delta
   \end{cases}$

   $S=\{(-5\delta,2\delta,\delta):\delta\in\R\}$

   $\forall\delta\not=0$ otteniamo i coefficienti di una combinazione lineare non banale che restituisce il vettore nullo

   $\delta=1:(-5,2,1)\\\qquad-5v_1+2v_2+v_3=-5(1,2,3)+2(3,2,1)+(-1,6,13)=(0,0,0)$

<u>Osservazioni</u>
- L'insieme delle combinazioni lineari di $v\in V$ è la retta vettoriale $<v>$:
  $$<v>:=\{\lambda v:\lambda\in K\}$$
- $\forall i=1,\cdots,n,\quad v_i$ è combinazione lineare di $v_1,\cdots,v_n$:

  $$v_i=0\cdot v_1+\cdots+0\cdot v_{i-1}+1\cdot v_i+0\cdot v_{i+1}+\cdots+0v_n$$
- Dalla definizione di sottospazio segue che se $v_1,\cdots,v_n\in W$ e $W$ è un sottospazio, allora tutte le combinazioni lineari di $v_1,\cdots,v_n$ appartengono a $W$.

  L'insieme
  $$<v_1,\cdots,v_n>:=\{\lambda_1v_1+\cdots+\lambda_nv_n:\lambda_i\in K,\forall i=1,\cdots,n\}$$

  è un sottospazio di $V$ chiamato il <u>sottospazio generato</u> (o *span* o copertura lineare) da (di) $v_1,\cdots,v_n$.

  È il "più piccolo" sottospazio di $V$ che contiene $v_1,\cdots,v_n$:

  Se $W$ è un sottospazio che contiene $v_1,\cdots,v_n$
  $$<v_1,\cdots,v_n>\subseteq W$$
  
  <u>Esempio</u>
  
  $V=M_2(\R)$

  $v_1=\begin{pmatrix}1&0\\0&1\end{pmatrix},\quad v_2=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$

  $<v_1,v_2>=<\begin{pmatrix}1&0\\0&1\end{pmatrix},\begin{pmatrix}0&1\\-1&0\end{pmatrix}>=\begin{cases}a\begin{pmatrix}1&0\\0&1\end{pmatrix}+b\begin{pmatrix}0&1\\-1&0\end{pmatrix}:a,b\in\R\end{cases}=\\=\begin{cases}\begin{pmatrix}a&0\\0&a\end{pmatrix}+\begin{pmatrix}0&b\\-b&0\end{pmatrix}:a,b\in\R\end{cases}=\\=\begin{cases}\begin{pmatrix}a&b\\-b&a\end{pmatrix}:a,b\in\R\end{cases}$

  $\begin{pmatrix}1&3\\-3&1\end{pmatrix}\in<v_1,v_2>$

  $<v_1,v_2>=M_2(\R)$? No, perchè $\begin{pmatrix}1&2\\-3&2\end{pmatrix}\not\in<v_1,v_2>$

  $<v_1,v_2>\subset M_2(\R)$

  <u>Osservazione</u>

  $\forall m\leq n$
  $$<v_1,\cdots,v_m>\subseteq <v_1,\cdots,v_m,v_{m+1},\cdots,v_n$$
  $\uparrow$ ogni combinazione lineare di $v_1,\cdots,v_m$ è anche combinazione lineare di $v_1,\cdots,v_n$

  $\lambda_1v_1+\lambda_nv_n=\lambda_1v_1+\cdots+\lambda_mv_m+0\cdot v_{m+1}+\cdots+0\cdot v_n$

Ripartiamo dall'esercizio 1 del foglio 2:

$V=\R^2,\quad v=(1,2),w=(3,4)\in\R^2$

Abbiamo mostrato che:
- $\forall(a,b)\in\R^2,\exists\lambda,\mu\in\R:(a,b)=\lambda(1,2)+\mu(3,4)$, o equivalentemente,
  
  $(a,b)\in<(1,2),(3,4)>$
  
  Poichè $<(1,2),(3,4)>\subseteq\R^2$, otteniamo che $<(1,2),(3,4)>=\R^2$, cioè $(1,2)$ e $(3,4)$ "generano" tutto $\R^2$ attraverso le loro combinazioni linerai.

  Diremo che $\{(1,2),(3,4)\}$ è un "sistema di generatori" di $\R^2$
- $(0,0)=\lambda(1,2)+\mu(3,4)\Leftrightarrow\lambda=\mu=0$, cioè l'unica combinazione lineare di $(1,2)$ e $(3,4)$ che restituisce il vettore nullo è quella banale.

  Diremo che $(1,2)$ e $(3,4)$ sono linearmente indipendenti.
  
Più in generale definiamo:

<u>Def</u>: Sia $V$ uno spazio vettoriale su $K$

Diciamo che $v_1,\cdots,v_n\in V$ <u>generano</u> $V$ oppure che $\{v_1,\cdots,v_n\}$ è un <u>sistema di generatori</u> di $V$ se:
$$<v_1,\cdots,v_n>=V$$

<u>Osservazione</u>: Poichè abbiamo sempre $<v_1,\cdots,v_n>\subseteq V$, per mostrare che $\{v_1,\cdots,v_n\}$ è un sistema di generatori di $V$ basta dimostrare che
$$V\subseteq<v_1,\cdots,v_n>,$$
cioè che $\forall v\in V,\exists\lambda_1,\cdots,\lambda_n\in K$ tali che
$$v=\lambda_1v_1+\cdots+\lambda_nv_n$$

## Definizione di vettori linearmente indipendenti
<u>Def</u> (<mark>difficile, la chiede 100%</mark>): Sia $V$ uno spazio vettoriale su $K$.

I vettori $v_1,\cdots,v_n\in K$ si dicono **linearmente indipendenti** se
$\lambda_1v_1+\lambda_2v_2+\lambda_nv_n=$ <u>0</u> $\Rightarrow\lambda_1=\cdots=\lambda_n=0$, o equivalentemente se l'unica combinazione lineare di $v_1,\cdots,v_n$ che restituisce il vettore nullo è quella banale.

Altrimenti, se esistono $\lambda_1,\cdots,\lambda_n$ <u>non tutti nulli</u> $((\lambda_1,\cdots,\lambda_n)\not=(0,\cdots,0))$ tali che $\lambda_1v_1+\cdots+\lambda_nv_n=$ <u>0</u>, $v_1,\cdots,v_n$ si dicono <u>linearmente dipendenti</u>.

<u>Esempio</u>:

$V=\R^3$

$v_1=(8,-2,0),\quad v_2=(0,3,4),\quad v_3=(-2,2,2)\in\R^3$

<u>Domanda</u>: $v_1,v_2,v_3$ sono linearmente indipendenti?

Siano $\lambda,\mu,\delta\in\R$ tali che:

$\lambda v_1+\mu v_2+\delta v_3=$ <u>0</u> $\Rightarrow\lambda(8,-2,0)+\mu(0,3,4)+\delta(-2,2,2)=(0,0,0)\Rightarrow$
$\Rightarrow
\begin{cases}
  8\lambda-2\delta=0\\
  -2\lambda+3\mu+2\delta=0\\
  4\mu+2\delta=0
\end{cases}$

$\begin{pmatrix}
  8&0&-2&\vdots&0\\
  -2&3&2&\vdots&0\\
  0&4&2&\vdots&0
\end{pmatrix}\xrightarrow{R_2\leftarrow R_2+\frac{1}{4}R_1}
\begin{pmatrix}
  8&0&-2&0\\
  0&3&\frac{3}{2}&0\\
  0&4&2&0
\end{pmatrix}\xrightarrow{R_3\leftarrow R_3-\frac{4}{3}R_2}
\begin{pmatrix}
  8&0&-2&0\\
  0&3&\frac{3}{2}&0\\
  0&0&0&0
\end{pmatrix}\Rightarrow
\begin{cases}
8\lambda-2\delta=0\\
3\mu+\frac{3}{2}\delta=0
\end{cases}\Rightarrow
\begin{cases}
\lambda=\frac{1}{4}\delta\\
\mu=-\frac{1}{2}\delta
\end{cases}$

$S=\{(\frac{1}{4}\delta,-\frac{1}{2}\delta,\delta):\delta\in\R\}$

$\delta=4\leadsto(1,-2,4)$

$$v_1-2v_2+4v_3=(0,0,0)$$

$\Rightarrow v_1,v_2$ e $v_3$ sono <u>linearmente dipendenti</u>

<u>Osservazioni</u>
1. Un vettore $v\in V$ è <u>linearmente dipendente</u> se e solo se $v=$ <u>0</u>
   
   $\Leftarrow)$ se $v=$ <u>0</u> allora $1\cdot v=$ <u>0</u> $\Rightarrow\ v$ è linearmente dipendente

   $\Rightarrow)\quad\exists\lambda\not=0:\lambda v=$ <u>0</u> $\Rightarrow\lambda^{-1}\lambda v=\lambda^{-1}$ <u>0</u> $\Rightarrow1\cdot v=$ <u>0</u>
2. Due vettori $v_1,v_2\in V$ sono linearmente dipendenti $\Leftrightarrow\exists\lambda\in K$ tale che $v_1=\lambda v_2$ o $v_2=\lambda v_1$.
   
   <u>Esempio</u>: $V=\R^3$

   $v_1=\begin{pmatrix}1\\2\\3\end{pmatrix},\quad v_2=\begin{pmatrix}3\\6\\9\end{pmatrix}=3v_1\Rightarrow v_1,v_2$ sono linearmente dipendenti.

   Infatti se $v_2=3v_1\Rightarrow3v_1-v_2=$ <u>0</u>

   $\Leftarrow)$ Supponiamo $\exists\lambda\in K:v_1=\lambda v_2$ o $v_2=\lambda v_1$.

   Se $v_1=\lambda v_2\Rightarrow1\cdot v_1-\lambda v_2=$ <u>0</u>

   Se $v_2=\lambda v_1\Rightarrow\lambda v_1-v_2=$ <u>0</u>

   In ogni caso $v_1,v_2$ sono linearmente dipendenti.

   $\Rightarrow)$ Supponiamo $v_1,v_2$ linearmente dipendenti $\Rightarrow\exists\lambda_1\lambda_2\in K,(\lambda_1,\lambda_2)\not=(0,0):\lambda_1v_1+\lambda_2v_2=$ <u>0</u>

   Se $\lambda_1\not=0\Rightarrow v_1=-\frac{\lambda_2}{\lambda_1}v_2$

   Se $\lambda_2\not=0\Rightarrow v_2=-\frac{\lambda_1}{\lambda_2}v_1$

   Quindi $\exists\lambda\in K:v_1=\lambda v_2$ o $v_2=\lambda v_1$

   <u>Esempio</u>: $v_1=(1,2,3),\quad v_2=(0,0,0)\in\R^3$ sono linearmente dipendenti poichè $v_2=0\cdot v_1\Rightarrow0\cdot v_1+(-1)v_2=$ <u>0</u>
3. $v_1,\cdots,v_n\in V$ sono linearmente dipendenti $\Leftrightarrow\exist i\in\{1,\cdots,n\}$ tale che $v_i$ è combinazione lineare degli altri.
   
   <u>Esempio</u>: $v_1=(1,1,1),\quad v_2=(1,-1,3),\quad v_3=(2,0,4)$

   $v_1,v_2,v_3$ sono linearmente dipendenti poichè $v_3=v_1+v_2\Rightarrow v_1+v_2-v_3=$ <u>0</u>
4. Se l'insieme $\{v_1,\cdots,v_n\}$ contiene il vettore nullo allora $v_1,\cdots,v_n$ sono linearmente dipendenti.

<u>Def</u>: Un sottoinsieme finito $\{v_1,\cdots,v_n\}$ di $V$ si dice <u>base</u> di $V$ se:
1. $v_1,\cdots,v_n$ sono linearmente indipendenti
2. $v_1,\cdots,v_n$ generano $V,\forall v\in V\\\exists\lambda_1,\cdots,\lambda_n\in K:\lambda_1v_1+\cdots+\lambda_nv_n=v$.


# <mark>12/04/22</mark>

<u>Def</u>: Sia $V$ uno spazio vettoriale su $K$ e siano $v_1,\cdots,v_n\in V$
- Diciamo che $\{v_1,\cdots,v_n\}$ è un sistema di generatori o che $v_1,\cdots,v_n$ generano $V$ se
  $$<v_1,\cdots,v_n>=V$$
  o equivalentemente se
  $$\forall v\in V,\exists(\lambda_1,\cdots,\lambda_n)\in K^n$$
  tali che
  $$(*)\lambda_1v_1+\cdots+\lambda_nv_n=v$$
- Diciamo che $v_1,\cdots,v_n$ sono linearmente indipendenti se $\lambda_1v_1+\cdots+\lambda_nv_n=$ <u>0</u> $\Rightarrow\lambda_1=\lambda_2=\cdots=\lambda_n=0$

  $[(\lambda_1,\cdots,\lambda_n)=(0,\cdots,0)]$

- Diciamo che $\{v_1,\cdots,v_n\}$ è una <u>base</u> di $V$ se:
  1. $v_1,\cdots,v_n$ generano $V$
  2. $v_1,\cdots,v_n$ sono linearmente indipendenti.
  
<u>Proposizione</u>: Sia $V$ uno spazio vettoriale su $K$ e sia $\{v_1,\cdots,v_n\}$ una base di $V$

Allora $\forall v\in V\exists!(\lambda_1,\cdots,\lambda_n)\in K^n$ tale che
$$\lambda_1v_1+\cdots+\lambda_nv_n=\mu_1v_1+\cdots+\mu_nv_n$$
allora $(\lambda_1,\cdots,\lambda_n)=(\mu_1,\mu_n)\Leftrightarrow\lambda_i=\mu_i,\forall i=1,\cdots,n$

I coefficienti $\lambda_1,\cdots,\lambda_n\in K$ della combinazione lineare (*) Si dicono le coordinate di $v$ rispetto alla base $\{v_1,\cdots,v_n\}$ e $(\lambda_1,\cdots,\lambda_n)$ si dice la $n$-upla delle coordinate di $v$ rispetto alla base $\{v_1,\cdots,v_n\}$

<u>Dim</u>

Poichè $\{v_1,\cdots,v_n\}$ è una bse allora i vettori $v_1,\cdots,v_n$ sono linearmente indipendenti.

La conclusione segue dall'esercizio 6-(d) del foglio 4

<u>Esempio</u>

$V=\R^2$

$v_1=(1,0),\quad v_1=(0,1)\in\R^2$
- $v_1,v_2$ generano $\R^2:\forall(a,b)\in\R^2$

  $(a,b)=a(1,0)+b(0,1)$
- $v_1,v_2$ sono linearmente indipendenti. Infatti se $\lambda_1,\lambda_2\in\R$ sono tali che:
  $$\lambda_1(1,0)+\lambda(0,1)=(0,0)\Rightarrow(\lambda_1,\lambda_2)=(0,0)$$

  Quindi $\mathbb{B}=\{(1,0),(0,1)\}$ è **una** base di $\R^2$

  Si noti che parliamo di **una** base di $\R^2$, in quanto essa non è unica.

  $w_1=(1,2),w_2=(3,4)$ generano $\R^2$ e sono linearmente indipendenti

  $\Rightarrow\mathbb{B}'={w_1,w_2}$ è un'altra base di $\R^2$

<u>Def</u>: Due vettori $v_1,v_2\in\R^2$ si dicono collineari se v_1,v_2 sono linearmente dipendenti, cioè se $\exists\lambda\in K$ tale che:
$$v_1=\lambda v_2\quad o\quad v_2=\lambda v_1$$

Geometricamente è semplice vedere che ogni coppia di vettori non collineari $v_1,v_2$ costituisce una base di $\R^2$

Vedremo che tutte le basi di $\R^2$ sono della forma $\{v_1,v_2\}$ con $v_1,v_2$ non collineari.

In particolare tutte le basi di $\R^2$ sono costituite da 2 elementi

<u>Lemma</u> (di Steinitz)

Sia $V$ uno spazio vettoriale con base $\mathbb{B}=\{v_1,\cdots,v_n\}$ e siano $w_1,\cdots,w_m\in V$

$w_1,\cdots,w_m$ sono linearmente indipendenti $\Rightarrow m\le n$

$\qquad\qquad\qquad\qquad\qquad\Updownarrow m>n\Rightarrow w_1,\cdots,w_m$ sono linearmente dipendenti.

Utilizziamo il lemma di Steinitz per dimostrare il risultato seguente:

<u>Teorema di equipotenza delle basi</u>

Sia $V$ uno spazio vettoriale su K.

Siano $\{v_1,\cdots,v_n\}$ e $\{w_1,\cdots,w_n\}$ due basi di $V$.

Allora $n=m$

<u>Dim</u>: Idea: $m=n\Leftrightarrow m\le n$ e $m\ge n$.
- Poichè $\{v_1,\cdots,v_n\}$ è una base di $V$ e $v_1,\cdots,v_n$ sono linearmente indipendenti $\xRightarrow{lemma}m\le n$
- Poichè $\{w_1,\cdots,w_n\}$ è una base di $V$ e $v_1,\cdots,v_n$ sono linearmente indipendenti $\xRightarrow{lemma}n\le m$

  Quindi $m\le n$ e $n\le m\Leftrightarrow n=m$

<u>Def</u>: Sia $V$ uno spazio vettoriale su $K$ e sia $\{v_1,\cdots,v_n\}$ una base finita di V.

Il numero $n$ si dice *dimensione* di $V$ e si denota

$dim_K(V)$ o più semplicemente $dim(V)$

Se $V=\{$<u>0</u>$\}$ allora si pone $dim(V)=0$.

Se $V=\{$<u>0</u>$\}$ oppure se $V$ ha una base finita diciamo che $V$ ha <u>dimensione finita</u>.

<u>Esempi</u>
1. $\R^2$ è uno spazio vettoriale di dimensione 2, poichè abbiamo visto che $\{(1,0),(0,1)\}$ è una base di $\R^2$.
2. $V=K^n=\{(x_1,\cdots,x_n):x_i\in K,\forall i=1,\cdots,n\},n\ge 1$

    Siano

    $e_1=(1,0,\cdots,0)$

    $e_2=(0,1,\cdots,0)$

    $\vdots$

    $e_n=(0,\cdots,0,1)$

    È facile mostrare che $\{e_1,\cdots,e_n\}$ è una base di $K^n$ detta **base canonica** di $K^n$.

    Quindi $dim_KK^n=n$.

    $\forall x'=(x_1,\cdots,x_n)\in K^n$, abbiamo

    $x'=x_1e_1+x_2e_2+\cdots+x_ne_n$

    cioè $x'$ è la $n$-upla delle coordinate di $x'$ rispetto a $\{e_1,\cdots,e_n\}$
3. $V=M_2(\R)$

    Siano:

    $E_{11}=\begin{pmatrix}1&0\\0&0\end{pmatrix},E_{12}=\begin{pmatrix}0&1\\0&0\end{pmatrix},E_{21}=\begin{pmatrix}0&0\\1&0\end{pmatrix},E_{22}=\begin{pmatrix}0&0\\0&1\end{pmatrix}$

    $\forall\begin{pmatrix}a&b\\c&d\end{pmatrix}=aE_{11}+bE_{12}+cE_{21}+dE_{22}$.

    Si mostra facilmente che $E_{11},E_{12},E_{21},E_{22}$ siano linearmente indipendenti.

    Quindi $\{E_{11},E_{12},E_{21},E_{22}\}$ è una base di $M_2(\R)\Rightarrow dim_\R$ <mark>incompleto</mark>

$V,\mathbb{B}=\{v_1,\cdots,v_n\}$ una base di $V$.

Consideriamo la funzione

$$\varphi_\mathbb{B}:V\rightarrow K^n$$
$$v=\lambda_1v_1+\cdots+\lambda_nv_n\mapsto(\lambda_1,\cdots,\lambda_n)$$
- <u>iniettiva</u>: se $v,w$ sono tali che $\varphi_\mathbb{B}(v)=\varphi_\mathbb{B}(w)\Rightarrow v=w$.

    $v,w\in V\Rightarrow v=\lambda_1v_1+\cdots+\lambda_nv_n\\\qquad\qquad\quad\ w=\mu_1v_1+\cdots+\mu_nv_n$
- <u>suriettiva</u>? $\forall(\lambda_1,\lambda_n)\in K^n,\exists v\in V$ tale che
$$\varphi_\mathbb{B}=(\lambda_1,\cdots,\lambda_n)$$
Basta prendere $v=\lambda_1v_1+\cdots+\lambda_nv_n$ (\boxed)

Quindi $\varphi_\mathbb{B}$ è biettiva.

Inoltre $\varphi_\mathbb{B}$ soddisfa le seguenti proprietà:

1. $\forall w_1,w_2\in V,\varphi_\mathbb{B}(w_1+w_2)=\varphi_\mathbb{B}(w_1)+\varphi_\mathbb{B}(w_2)$.

<u>Dim</u>

Siano $w_1w_2\in V$. Quindi $\exists\lambda_1,\cdots,\lambda_n,\mu_1,\cdots,\mu_n\in K$ tali che
$$w_1=\lambda_1v_1+\cdots+\lambda_nv_n,\quad w_2=\mu_1v_1+\cdots+\mu_nv_n$$
Quindi $\varphi_\mathbb{B}(w_1)=(\lambda_1,\cdots,\lambda_n),\varphi_\mathbb{B}(\mu_1,\cdots,\mu_n)$

Ora $w_1+w_2=\lambda_1v_1+\cdots+\lambda_nv_n+\mu_1v_1+\cdots+\mu_nv_n=(\lambda_1\mu_1)v_1+\cdots+(\lambda_n\mu_n)v_n$

$\varphi_\mathbb{B}(w_1+w_2)=(\lambda_1+\mu_1,\cdots,\lambda_n+\mu_n)=(\lambda_1,\cdots,\lambda_n)+(\mu_1,\cdots,\mu_n)=\varphi_B(w_1)+\varphi_B(w_2)$
2. $\forall\lambda\in K$ <mark>Incompleto</mark>

Le proprietà 1 e 2 fanno di $\varphi_B$ quella che chiameremo un'"applicazione lineare".

Chiamiamo $\varphi_B$ **isomorfismo coordinato** rispetto alle basi $B$.

<u>Teorema</u> (di esistenza della base): Sia $V\not=\{$<u>0</u>$\}$

$L=\{v_1,\cdots,v_p\}$ un insieme di vettori linearmente indipendenti

$G=\{v_1,\cdots,v_p,\cdots,v_m\},m\ge p$, un sistema di generatori.

Allora esiste una base $B$ di $V$ tale che
$$L\subseteq B\subseteq G$$

Prima della dimostrazione:

<u>Corollario</u> 1: Sia $V\not=\{$<u>0</u>$\}$ uno spazio vettoriale di dimensione finita. Allora:
1. Da qualsiasi sistema di generatori è possibile <u>estrarre</u> una base di $V$
2. È possibile <u>completare</u> qualsiasi insieme di vettori linearmente indipendenti a una base di $V$

<u>Esempio</u>

$V=\R^3$

$v_1=(1,2,3),v_2=(4,6,9)\in\R^3$

$L=\{(1,2,3),(4,6,9)\}$ è un insieme di vettori linearmente indipendenti.

$L\subseteq G=\{(1,2,3),(4,6,9),(1,0,0),(0,1,0),(0,0,1)\}$

$G$ è un sistema di generatori.

Per il teorema esiste una base $B$ di $\R^3$ tale che
$$L\subseteq B\subseteq G$$
<u>Tentativo</u> 1: $\{(1,2,3),(4,6,9),(1,0,0)\}$

Linearmente indipendenti?: Siano $\lambda,\mu,\delta\in\R:$
$$\lambda(1,2,3)+\mu(4,6,9)+\delta(1,0,0)=(0,0,0)$$
$\Rightarrow\begin{cases}
\lambda+4\mu+\delta=0\\
2\lambda+6\mu=0\\
3\lambda+9\mu=0
\end{cases}\Rightarrow
\begin{cases}
\mu=-\delta\\
0=0\\
\lambda=-3\mu
\end{cases}\Rightarrow
\begin{cases}
\mu=-\delta\\
\lambda=3\delta
\end{cases}\Rightarrow
S=\{(3\delta,-\delta,\delta):\delta\in\R\}$

$\delta=1\leadsto(3,-1,1)\Rightarrow3(1,2,3)-(4,6,9)+(1,0,0)=(0,0,0)\Rightarrow$ sono linearmente dipendenti.

<u>Tentativo</u> 1: $\{(1,2,3),(4,6,9),(0,1,0)\}$

Linearmente indipendenti?
1. No $\leadsto\{(1,2,3),(4,6,9),(0,1,0)\}$ <mark>Incompleto</mark>
# <mark>13/04/22</mark>
## Continuando da ieri, Corollario 1
<u>Corollario 2</u>: Sia $V$ uno spazio vettoriale su $K$ di dimensione $n$.
1. Ogni sistema di generatori di $V$ con $n$ elementi è una base di $V$
2. Ogni insieme di $n$ vettori linearmente indipendenti è una base di $W$

<u>Dim</u>
1. $G=\{v_1,\cdots,v_n\}$ sistema di generatori

    Per il corollario 1 $\exists$ una base $B$ di $V$ tale che
    
    $B\subseteq G\Rightarrow B=G$, cioè $G$ è una base di $V$
    
    $B$ ha $n$ elementi poichè $dim(V)=n$
2. $L=\{v_1,\cdots,v_n\},v_1,\cdots,v_n$ sono linearmente indipendenti.

    Per il corollario 1, $\exists$ una base $B$ di $V$ tale che

    $L\subseteq B\Rightarrow B=L$

<u>Proposizione</u>: Sia $V$ uno spazio vettoriale di dimensione finita.

Sia $W$ un sottospazio di $V$. Allora:
1. $dim(W)\le dim(V)$
2. $dim(W)=dim(V)\Leftrightarrow V=W$

<u>Dim</u>

Sia $n=dim(V)$
1. Si mostra che anche $W$ è di dimensione finita (non è scontato) <mark>vedi note della prof, non lo spiega qui in classe</mark>.

    Sia dunque $\{w_1,\cdots,w_m\}$ una base finita di $W$

    Ora $w_1,\cdots,w_m$ sono vettori linearmente indipendenti di $W\subseteq V\xRightarrow{Lemma\ di\ Steinitz}m\le n\Leftrightarrow dim(W)\le dim(V)$
2. $\Leftarrow)$ ovvio.

    $\Rightarrow)$ Supponiamo $dim(W)=dim(V)=n$.

    Sia $B=\{w_1,\cdots,w_n\}$ una base di $W$.

    Ora $w_1,\cdots,w_n$ sono vettori linearmente indipendenti di $V$ e quindi B è anche una base di $V$.

    $W=<w_1,\cdots,w_n>=V$

    $\uparrow$ sistema di generatori di W, $\quad\uparrow$ sistema di generatori di V

<u>Osservazione</u>: $W$ è un sottospazio, $dim(W)=0\Leftrightarrow W=\{$<u>0</u>$\}$

<u>Def</u>: Sia $V$ uno spazio vettoriale e $W\subseteq V$ un sottospazio.

Allora l'intero

$$dim(V)-dim(W)$$

Si dice **codimensione** di $W$ in $V$

<u>Teorema</u> (formula di Grassman):

Sia $V$ uno spazio vettoriale, siano $U,W$ due sottospazi di $V$ di dimensione finita.

Allora $U\cap W$ e $U+W$ hanno dimensione finita e
$$dim(U+W)=dim(U)+dim(W)-dim(U\cap W)$$
In particolare se $U\oplus W$ è somma diretta $(U\cap W=\{$<u>0</u>$\})$ allora $dim(U\cap W)=0$ e $dim(U+W)=dim(U)+dim(W)$

<mark>Esempi mancanti, non so se possono servire</mark>.

<u>Proposizione</u>: Siano $U,W$ due sottospazi di $V$ tali che $U\cap W=\{$<u>0</u>$\}$.

Siano $B_u,B_w$ due basi rispettivamente di $U$ e $W$, allora $B_u\cup B_w$ è una base di $U\oplus W$

<u>Dim</u>: per esercizio

<u>Def</u>: Sia $V$ uno spazio vettoriale su $K$ e sia $\{v_1,\cdots,v_p\}$ un sottoinsieme finito di $V$, il **rango** di $\{v_1,\cdots,v_p\}$ è la dimensione del sottospazio vettoriale generato da $v_1,\cdots,v_p$.
$$rg(\{v_1,\cdots,v_p\})=dim(<v_1,\cdots,v_p>)$$
Equivalentemente, il rango è il numero massimo di vettori linearmente indipendenti in $\{v_1,\cdots,v_p\}$.

<u>Esempio</u>:

$rg(\{(0,1,0,0),(0,0,1,0),(0,1,1,0)\})=2$

$v_1,v_2$ linearmente indipendenti.

<u>Osservazioni</u>:
1. $0\leq rg(\{v_1,\cdots,v_p\})\leq p$
    - $rg(\{v_1,\cdots,v_p\})=0\Leftrightarrow v_1=\cdots=v_p=$<u>0</u>
    - $rg(\{v_1,\cdots,v_p\})=p\Leftrightarrow v_1,\cdots,v_p$ sono linearmente indipendenti
2. Se $dim(V)=n$ e $v_1,\cdots,v_p\in V$ allora $rg(\{v_1,\cdots,v_p\})\leq min\{p,n\}$

