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
- Insieme vuoto: insieme che non contiene nessun elemento, si denota con $\empty$, $\{\}$ e ha cardinalità $|\empty|=0$
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
    $\mathbb{N}\subseteq\mathbb{Z}\subseteq\mathbb{Q}\subseteq\R\subseteq\mathbb{C}$

    <u>Proprietà</u>:
    - $\mathbb{A}=\mathbb{B}\Leftrightarrow(x\in \mathbb{A}\Leftrightarrow x \in \mathbb{B})\Leftrightarrow(\mathbb{A}\subseteq\mathbb{B}$ ^ $\mathbb{B}\subseteq\mathbb{A})$
2. Intersezione $\leftrightarrow\wedge$

    $\mathbb{A}\cap\mathbb{B}=\{x:x\in\mathbb{A}\wedge x\in\mathbb{B}\}$

    <u>Proprietà</u>:
    - $\mathbb{A}\cap\empty=\empty$
    - $\mathbb{A}\cap\mathbb{B}=\mathbb{B}\cap\mathbb{A}$
    - $\mathbb{A}\subseteq\mathbb{B}\Rightarrow\mathbb{A}\cap\mathbb{B}=\mathbb{A}$
3. Unione $\leftrightarrow\vee$

    $\mathbb{A}\cup\mathbb{B}=\{x:x\in\mathbb{A}\vee x\in\mathbb{B}\}$

    <u>Proprietà</u>:
    - $\mathbb{A}\cup\empty=\mathbb{A}$
    - $\mathbb{A}\cup\mathbb{B}=\mathbb{B}\cup\mathbb{A}$
    - $\mathbb{A}\subseteq\mathbb{B}\Rightarrow\mathbb{A}\cup\mathbb{B}=\mathbb{B}$
    - $\mathbb{A}\subseteq\mathbb{A}\cup\mathbb{B},\ \mathbb{B}\subseteq\mathbb{A}\cup\mathbb{B}$
4. Differenza

    $\mathbb{B}\backslash \mathbb{A}=\{x:x\in\mathbb{B}\wedge x\not\in\mathbb{A}\}$
5. Prodotto cartesiano:
    $\mathbb{A}\times\mathbb{B}:=\{(a,\ b):a\in\mathbb{A},\ b\in\mathbb{B}\}$ con $(a,\ b)$ coppie ordinate

    <u>Proprietà</u>:
    - $|\mathbb{A}\times\mathbb{B}|=|\mathbb{A}|\cdot|\mathbb{B}|$
    - $\mathbb{A}\times\empty=\empty=\empty\times\mathbb{A}$
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
# <mark>09/03/22</mark>
## Funzioni (continuo)
<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>iniettiva</u> se $\forall x\not=y\Rightarrow f(x)\not=f(y)$ (elementi distinti di $\mathbb{A}$ hanno immagini distinte) $\Leftrightarrow f(x)=f(y)\Rightarrow x=y$

<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>suriettiva</u> se $Im(f)=B$, o equivalentemente se $\forall y\in \mathbb{B}, \exist x\in\mathbb{A}:f(x)=y$

<u>Def</u>: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>biettiva</u> o <u>biunivoca</u> se è al tempo stesso iniettiva e suriettiva

<u>Esempio</u>:

$f:\R\rightarrow\R\\\qquad\!\!x\rightarrow x^2$

È iniettiva? No, perchè $f(-1)=1=f(1)$

È suriettiva? No, perchè $f(x)=x^2\geq0\forall x\in\R\Rightarrow Im(f)\subseteq\R^+\Rightarrow Im(f)\not=\R$

<br>

Se un insieme possiede delle operazioni che verificano certe proprietà, è una struttura algebrica.

<u>Def</u>: Sia $\mathbb{X}$ un insieme, un'<u>operazione binaria interna</u> è una funzione dal prodotto cartesiano $x\times x$ in $\mathbb{X}$.

$*:x\times x \rightarrow x$

$\qquad\!\!\!(x,y)\rightarrow x*y$

$\mathbb{X}=\R$

$+:\R\times\R\rightarrow\R$

$\qquad(x,y)\rightarrow x+y$

<u>Proprietà</u> di $(\R,+)$:

1. Commutatività:  $x+y=y+x, \forall x,y\in\R$

2. Associatività:  $(x+y)+z=x+(y+z),\forall x,y,z\in\R$

3. Esistenza dell'elemento neutro:  $\exist x'\in\R:x+x'=x'+x=x,\forall x\in\R, x'=0$

4. Esistenza dell'opposto:  $\exist x'\in\R:x+x'=x'+x=0,\forall x\in\R, (x'=-x)$

$\R\times\R\rightarrow\R$ operazione binaria interna

$\quad\!\!\!\!(x,y)\rightarrow x\cdot y$

<u>Proprietà</u> di $(\R,\cdot)$:

1. Commutatività: $x\cdot y=y\cdot x, \forall x,y\in\R$

2. Associatività: $(x\cdot y)\cdot z=x\cdot(y\cdot z),\forall x,y,z\in\R$

3. Esistenza dell'elemento neutro: $\exist x'\in\R:x\cdot x'=x'\cdot x=x,\forall x\in\R, x'=1$

4. Esistenza dell'inverso: $\exist x'\in\R:x\cdot x'=x'\cdot x=0,\forall x\in\R, (x'=\frac{1}{x})$

Infine $+$ e $\cdot$ soddisfano la proprietà distributiva: $\forall x,y,z\in\R,x\cdot(y+z)=x\cdot y+x\cdot z$

Sia $\mathbb{K}\not=\empty$ un insieme dotato di due operazioni binarie:

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

Se $v,w\in\mathbb{X}$ sono due soluzioni del problema, allora anche $v+w$ e $\lambda v, \lambda\in\R$  ($+$ e $\cdot$ operazioni su $\mathbb{X}$) sono soluzioni del problema.

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

  $\exist 0\in\R:x+0=0+x=x,\forall x\in\R$
- Esistenza dell'opposto:

  $\exist x'\in\R:x+x'=x'+x=0,\forall x\in\R$
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

$\{P:P\in\pi\}\leftrightarrow\{(x,y):x,y\in\R\}=\R^2$

$\mathbb{V}=\{$segmenti orientati $\vec{OP},P\in\pi\}=\{$vettori geometrici nel piano$\}$

In particolare esiste una blezione:

$\mathbb{V}\leftrightarrow\R^2$

$\forall P\in\pi,\vec{OP}\rightarrow(x,y)$, dove $x,y$ sono rispettivamente ascissa e ordinata di $P$

$\vec{OP}\leftarrow(x,y)$ dove $P(x,y)$

Vogliamo tradurre le operazioni su $\mathbb{V}$ in operazioni su $\R^2$:

1. $\vec{v}=\vec{OP},P(x_P,y_P)$

    $\vec{w}=\vec{OQ},Q(x_Q,y_Q)$

    $\vec{v}+\vec{w}=\vec{OR}:$ quali sono le coordinate di R?

    $OPQR\Rightarrow A(x_A,y_A)$ parallelogramma con punto medio di $PQ$ e $OR$

    $A$ punto medio di $PQ\Rightarrow\{x_A=\frac{x_P+x_Q}{2}, y_A=\frac{y_P+x_Q}{2}\}$

    $A$ punto medio di $OR\Rightarrow\{x_A=\frac{x_R}{2},y_A=\frac{y_R}{2}\}$

    $\Rightarrow\{x_R=x_P+x_Q,y_R=y_P+y_Q\}$

    Operazione binaria <u>interna</u>: $+:\R^2\times\R^2\rightarrow\R^2$

    $((x_1,y_1),(x_2,y_2))\mapsto(x_1+x_2,y_1+y_2)$
2. $\vec{v}\in\mathbb{V},\vec{v}=\vec{OP},P(x_P,y_P), \lambda\in\R$

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

    Operazione binaria <u>esterna</u>: $\cdot:\R\times\R^2\rightarrow\R^2$

    $(y,(x,y))\mapsto\lambda\cdot(x,y):=(\lambda x,\lambda y)$
    
    In conclusione abbiamo definito due operaizoni su $\R^2$ "compatibili" con le operazioni definite su $\mathbb{V}$:

      - $+: \R^2\times\R^2\rightarrow\R^2$

          $((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)+(x_2,y_2):=(x_1+y_1,x_2+y_2)$
      - $\cdot: \R^2\times\R^2\rightarrow\R^2$

          $(\lambda,(x_2,y_2))\mapsto\lambda\cdot(x_2,y_2):=(\lambda\cdot x,\lambda\cdot y)$

      <u>Proprietà di $+$ e $\cdot$</u>

      1. commutatività

          $\forall(x_1,y_1),(x_2,y_2)\in\R^2, (x_1,y_1)+(x_2,y_2)=(x_2,y_2)+(x_1,y_1)$
      2. associatività

          $\forall(x_1,y_1),(x_2,y_2),(x_3,y_3)\in\R^2,
          
          ((x_1,y_1)+(x_2,y_2))+(x_3,y_3)=(x_1,y_1)+((x_2,y_2)+(x_3,y_3))$
      3. esistenza dell'elemento neutro

          $(0,0)\in\R^2$ è tale che $(x,y)+(0,0)=(0,0)+(x,y)=(x,y)$
      4. esistenza dell'opposto

          $\forall (x,y)\in\R^2,\exist(x',y')\in\R^2:(x,y)+(x',y')=(x',y')+(x,y)=(0,0)$
      5. distributività rispetto a vettori
      
          $\forall(x_1,y_1),(x_2,y_2)\in\R^2,\forall\lambda\in\R$

          $\lambda\cdot((x_1,y_1)+(x_2,y_2))=\lambda\cdot(x_1,y_1)+\lambda\cdot(x_2,y_2)
      6. distributività rispetto a scalari

          $\forall(x,y)\in\R^2,\forall\lambda,\mu\in\R$

          $(\lambda+\mu)\cdot(x,y)=\lambda\cdot(x,y)+\mu\cdot(x,y)$
      7. qualcosa, non so cosa

          $\lambda\mu\cdot(x,y)=\lambda\cdot(\mu\cdot(x,y))$
      8. elemento neutro

          $1\cdot(x,y)=(x,y)\forall(x,y)\in\R^2$
      
      $(\R^2,+,\cdot)$ è il primo insieme di <MARK>INCOMPLETO</MARK>

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
$+:\R^2\times\R^2\rightarrow\R^2$

$((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)+(x_2,y_2):=(x_1+x_2,y_1+y_2)$

$*:\R^2\times\R^2$

$((x_1,y_1),(x_2,y_2))\mapsto(x_1,y_1)*(x_2,y_2):=(x_1\cdot x_2,y_1\cdot y_2)$

$(\R^2,+,*)$ è un campo? NO!

$\triangle:\R^2\times\R^2$
$((a,b),(c,d))\mapsto(a,b)\triangle(c,d)=(ac-bd,ad+bc)$

Mostrare che $(\R^2,+,\triangle)$ è un campo.

<u>Indizio</u>: $\R^2\leftrightarrow\mathbb{C}=\{a+ib,b\in\R,i^2=-1\}$

$(a,b)leftmapsto a+ib$

$(a,b)\mapsto a+ib$

Nota che $\mathbb{C}$ è un campo

### <u>Esempi di spazi vettoriali</u>
1. $\mathbb{V}=\{$Vettori geometrici nello spazio$\}=\{$segmenti orientati $\vec{OP},\ P$ nello spazio$\}\longleftrightarrow\R^3$

   Definiamo $+$ e $\cdot$ in modo analogo al caso dei vettori nel piano e $(V,+,\cdot)$ è uno spazio vettoriale reale.
2. L'$n$-spazio vettoriale su $\R$ (o su $\mathbb{K}$)

   $n\in\mathbb{N}, n\ge1$
   $\R^n=\R\times\cdots\times\R=\{(x_1,\cdots,x_n):x_i\in\R\forall i\}$

   Definiamo $+:\R^n\times\R^n\to\R^n$ e $\cdot:\R^n\times\R^n\to\R^n$

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

     $P(x)=a_nx^n+a_{n-1}x^{n-1}+\cdots+a_1x+a_0,a_i\in\R\forall i$
     
     Se $a_n\ne0$ diremo che $n$ è il grado di $P$ e scriviamo $deg(P)=n$.

     $\R[x]:=\{$polinomi a coefficienti reali nell'indeterminata $x$ (di grado arbitrario)$\}$

     <u>Esempio</u>: $P(x)=3x^4+2x^3-x+5\in\R[x],\ deg(P)=4$

     $+:\R[x]\times\R[x]\to\R[x]\\P(x)=a_nx^n+\cdots+a_1x+a_0\\Q(x)=b_nx^n+\cdots+b_1x+b_0\\(P+Q)(x):=(a_n+b_n)x^n+\cdots+(a_1+b_1)x+a_0+b_0$

     $\cdot:\R\times\R[x]\to\R[x]\\P\in\R[x],\ P=a_nx^n+\cdots+a_1wx+a_0\\\lambda\in\R\\(\lambda\cdot P)(x):=\lambda a_nx^n+\cdots+\lambda a_1x+\lambda a_0$

     $(\R[x],+,\cdot)$ è uno spazio vettoriale su $\R$.
     
     In modo analogo si definisce $(K[x],+,\cdot)$ dove
     
     $K[x]=\{$polinomi a coefficienti in $\mathbb{K}$ in un'indetermiinata$\}$

     Molti problemi di matemadica/fisica hanno la proprietà che l'insieme delle soluzioni ha una struttura di spazio vettoriale.

     <u>Esempi</u>:

     - $\begin{cases}x+2y+z=0\\y+7z=0\end{cases}$

       $S=\{(x,y,z)\in\R^3:x+2y+z=0$ e $y+7z=0\}=\{(13t,-7t,t),t\in\R\}$
       $S$ ha una struttuta di spazio vettoriale (<mark>cose che vedremo più avanti</mark>)

# <mark>22/03/22</mark>
## <u>Sistemi di equazioni lineari</u> (accenni)

Equazione lineare in $n$ incognite:

$x_1,\cdots,x_n: a_1x_1+a_2x_2+\cdots+a_nx_n=b\\a_i\in\R,\forall i,b\in\R$

Sistema di $n$ equazioni lineari in $n$ incognite:
$\begin{cases}a_{11}x_1+a_{12}+\cdots+a_{1n}x_n=b_1\\
a_{21}x_1+a_{22}+\cdots+a_{2n}x_n=b_2\\
\cdots\\
a_{n1}x_1+a_{n2}+\cdots+a_{nn}x_n=b_n\\\end{cases}$

Una soluzione del sistema di sopra è un vettore $(x_1,\cdots,x_n)\in\R^n$ che verifica tutte le equazioni.

<u>Esempi</u>:

$\begin{cases}x+y+z=6\\2x-y=0\end{cases}$

<u>Una</u> soluzione di questo sistema è $(1,2,3)\in\R^3$

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

    <u>N.B.</u>: $\forall a,b\in\R,\ (a+b)^2=a^2+2ab+b^2$ perchè in $\R$, la moltiplicaizone è commutativa.
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

<u>Esempio</u>: $\forall\theta\in\R$ la matrice

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

    Quindi il sistema possiede l'unica soluzione $(\frac{1}{2},-\frac{1}{2})\in\R^2$
4. $\begin{cases}x_1+x_2=2\\3x_1-3x_2=6\end{cases}$

    è compatibile e possiede infinite soluzioni date dalle soluzioni di

    $x_1+x_2=2\Rightarrow x_1=2-x_2$

    L'insieme delle soluzioni $S$ è costituito dalle coppie ordinate $(x_1,x_2)\in\R^2$ tali che:

    $\begin{cases}x_1=2-t\\x_2=t\end{cases},\ t\in\R\\S=\{(2-t,t),\ t\in\R\}\subseteq\R^2$

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

Procedendo dal basso verso l'alto trovo che il sistema possiede l'unica soluzione $(4,0,-1)\in\R^3$

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
