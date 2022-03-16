# <mark>Geometria e algebra 08/03/22</mark>

## Richiami di logica

Proposizione logica: **V**/**F**, **1**/**0** valore di verità

P = "Napoli è in Campania": **V**

P(n) = "n è pari"

P(2):**V**

P(3):**F**

## Connettivi logici

- Negazione: $\neg$, "non"

- Congiunzione: ^, "e"

- Disgiunzione: $\bigvee$, "o"

- Implicazione: $\Rightarrow$, "se ... allora ..."

- Doppia implicazione: $\Leftrightarrow$, "se e solo se"

## Tavole di verità

| $P$ | $Q$ | $\neg P$ | $P\land Q$ | $P\bigvee Q$ | $P\Rightarrow Q$ | $P\Leftrightarrow Q$ |
| --- | --- | -------- | ---------- | ------------ | ---------------- | -------------------- |
| 1   | 1   | 0        | 1          | 1            | 1                | 1                    |
| 1   | 0   | 0        | 0          | 1            | 0                | 0                    |
| 0   | 1   | 1        | 0          | 1            | 1                | 0                    |
| 0   | 0   | 1        | 0          | 0            | 1                | 1                    |

## Quantificatori

- $\forall$: "Per ogni"

- $\exist$: "Esiste almeno uno"

- $\exist$!: "Esiste ed è unico"

**Esempi**:

1. "$\bigvee$n naturale, *n* è pari": F
   
   "$\exist$n naturale: ($\leftarrow$tale che) *n* è pari": V

2. P(x)={x è uno studente in aula A3-T2}
   
   Q(x)={x è iscritto ad un corso di ingegneria}
   
   $\bigvee$x, P(x)$\Rightarrow$Q(x)

3. P(n)={*n* è un numero pari}
   
   Q(n)={*n* è divisibile per 4}
   
   $\bigvee$n naturale, Q(n)$\Rightarrow$P(n)

---

# Teoria degli insiemi

Un **insieme** è una collezione di oggetti detti **elementi** dell'insieme.

Convenzionalmente gli insiemi si denotano con lettere maiuscole e gli elementi con lettere minuscole.

## Descrizione di un insieme

1. per elencazione (se l'insieme ha un numero finito di elementi):
   
   $\mathbb{A} = \{0, 2, 4, 6, 8, 10\}$
   
   $4\in \mathbb{A}$
   
   $5\notin \mathbb{A}$

2. per proprietà caratteristica
   
   $\mathbb{A}=\{n: n$ è un numero pari: $0\le n \le 10\}$

3. diagramma di *Eulero-Venn* (ancora una volta se l'insieme ha un numero finito di elementi)

## Roba degli insiemi

- La **cardinalità** di un insieme è il numero di elementi che un insieme contiene e si denota: $\mathbb{A}$ ha cardinalità $|\mathbb{A}|$

- Insieme vuoto: insieme che non contiene nessun elemento, si denota con $\empty$, $\{\}$ e ha cardinalità $|\empty|=0$

- I principali insiemi numerici:
  
  $\mathbb{N}=\{0, 1, 2, 3, ...\}$: numeri naturali
  
  $\mathbb{Z}=\{..., -3, -2, -1, 0, 1, 2, 3, ...\}$: numeri naturali
  
  $\mathbb{Q}=\{\frac{a}{b}:a,b$ e $\mathbb{Z}, b\not= 0\}$
  
  $\mathbb{R}:$numeri reali
  
  $\mathbb{C}$: numeri complessi

## Inclusione di insiemi

- $\mathbb{A}\subseteq\mathbb{B}$ ($\mathbb{A}$ è contenuto in $\mathbb{B}$)
  
  $\mathbb{B}\supseteq\mathbb{A}$ ($\mathbb{B}$ contiene $\mathbb{A}$)
  
  **Esempio**: $\mathbb{N}\subseteq\mathbb{Z}\subseteq\mathbb{Q}\subseteq\mathbb{R}\subseteq\mathbb{C}$

- $\mathbb{A}=\mathbb{B}\Leftrightarrow(x\in \mathbb{A}\Leftrightarrow x \in \mathbb{B})\Leftrightarrow(\mathbb{A}\subseteq\mathbb{B}$ ^ $\mathbb{B}\subseteq\mathbb{A})$

---

---

# ROBA NUOVA, DEVO ANCORA RICOPIARE LA PRIMA LEZIONE

# <mark>Geometria e algebra 09/03/22</mark>

**<u>Def</u>**: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>iniettiva</u> se $\forall x\not=y\Rightarrow f(x)\not=f(y)$ (elementi distinti di $\mathbb{A}$ hanno immagini distinte)$\Leftrightarrow f(x)=f(y)\Rightarrow x=y$

**<u>Def</u>**: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>suriettiva</u> se $Im(f)=B$, o equivalentemente se $\forall y\in \mathbb{B}, \exist x\in\mathbb{A}:f(x)=y$

**<u>Def</u>**: Una funzione $f:\mathbb{A}\rightarrow\mathbb{B}$ si dice <u>biettiva</u> o <u>biunivoca</u> se è al tempo stesso iniettiva e suriettiva

<u>esempio</u>: $f:\mathbb{R}\rightarrow\mathbb{R}$

                        $x\rightarrow x^2$

iniettiva? No, perchè $f(-1)=1=f(1)$

suriettiva? No, perchè $f(x)=x^2\geq0\forall x\in\mathbb{R}\Rightarrow Im(f)\subseteq\mathbb{R^+}\Rightarrow Im(f)\not=\mathbb{R}$

---

Se un insieme possiede delle operazioni che verificano certe proprietà, è una struttura algebrica.

**<u>Def</u>**: Sia $\mathbb{X}$ un insieme, un'<u>operazione binaria interna</u> è una funzione dal prodotto cartesiano $x\times x$ in $\mathbb{X}$.

$*:x\times x \rightarrow x$

$(x,y)\rightarrow x*y$

$\mathbb{X}=\mathbb{R}$

$+:\mathbb{R}\times\mathbb{R}\rightarrow\mathbb{R}$

$(x,y)\rightarrow x+y$

<u>Proprietà</u> di $(\R,+)$:

1. Commutatività:  $x+y=y+x, \forall x,y\in\R$

2. Associatività:  $(x+y)+z=x+(y+z),\forall x,y,z\in\R$

3. Esistenza dell'elemento neutro:  $\exist x'\in\R:x+x'=x'+x=x,\forall x\in\R, x'=0$

4. Esistenza dell'opposto:  $\exist x'\in\R:x+x'=x'+x=0,\forall x\in\R, (x'=-x)$

$\R\times\R\rightarrow\R$ operazione binaria interna

$(x,y)\rightarrow x\cdot y$

<u>Proprietà</u> di $(\R,\cdot)$:

1. Commutatività: $x\cdot y=y\cdot x, \forall x,y\in\R$

2. Associatività: $(x\cdot y)\cdot z=x\cdot(y\cdot z),\forall x,y,z\in\R$

3. Esistenza dell'elemento neutro: $\exist x'\in\R:x\cdot x'=x'\cdot x=x,\forall x\in\R, x'=1$

4. Esistenza dell'inverso: $\exist x'\in\R:x\cdot x'=x'\cdot x=0,\forall x\in\R, (x'=\frac{1}{x})$

5. Infine $+$ e $\cdot$ soddisfano la proprietà distributiva: $\forall x,y,z\in\R,x\cdot(y+z)=x\cdot y+x\cdot z$

Sia $\mathbb{K}\not=\empty$ un insieme dotato di due operazioni binarie:

- $+: \mathbb{K}\times\mathbb{K}\rightarrow\mathbb{K}$

- $\cdot:\mathbb{K}\times\mathbb{K}\rightarrow\mathbb{K}$

$(\mathbb{K},+,\cdot)$ è detto un <u>campo</u> se verifica le proprietà elencate prima, con $+$ distributiva con $\mathbb{K}$ al posto di $\R$

4. $\mathbb{F_2}=\{0, 1\}$
   
   - $\cdot:\mathbb{F_2}\cdot\mathbb{F_2}$
   
   - copia le cose di sotto con solo l'ultimo con valore 1
   
   - $+:\mathbb{F_2}\times\mathbb{F_2}\rightarrow\mathbb{F_2}$
     
     $(0, 0)\rightarrow 0$
     
     $(0, 1)\rightarrow 1$
     
     $(1, 0)\rightarrow 1$
     
     $(1, 1)\rightarrow 1$

# Algebra lineare

Wikipedia: "Branca della matematica che si occupa dello studio di spazi vettoriali (o anche detti spazi lineari), di trasformazioni lineari e di sistemi di equazioni lineari."

Molti problemo di matematica e fisica verificano la seguente proprietà:

Se $v,w\in\mathbb{X}$ sono due soluzioni del problema, allora anche $v+w$ e $\lambda v, \lambda\in\R$  ($+$ e $\cdot$ operazioni su $\mathbb{X}$) sono soluzioni del problema.

Problemi di questo tipo sono detti *lineari*.

**Nozione base: <u>spazio vettoriale</u>**

I vettori sono usati in fisica per rappresentare, grandezze fisiche caratterizzate da:

- una direzione

- un verso

- un' intensità

Tali grandezze sono *grandezze vettoriali* e si differenziano dalle *grandezze scalari*, definite unicamente dall'intensità.

Geometricamente, un vettore si rappresenta tramite un *segmento orientato* nel piano euclideo, denotato $\Pi$.

**<u>Def</u>**: Un segmento orientato è una coppia di punti ordinata $(A,B\in\Pi\times\Pi)$.

$\vec{AB}:=(A,B)$.

**<u>Def</u>**: Due segmenti orientati $\vec{AB}$ e $\vec{CD}$ si dicono <u>equipollenti</u> se il quadrilatero avente vertici, ordinatamente, $ABDC$ è un parallelogramma, quindi se hanno:

- stella lunghezza

- direzione parallela

- stesso verso

L'equipollenza è una relazione di equivalenza, e verifica 3 proprietà:

- riflessiva

- simmetrica

- transitiva

**<u>Def</u>**: Un vettore geometrico è una classe di equipollenza

Sia $O$ un punto fissato nel piano $\Pi$, per ogni segmento orientato $\vec{AB}$ esiste un punto $P\in\Pi$ tale che $\vec{OP}$ è equipollente ad $\vec{AB}$.

$\vec{OP}$ è equipollente a tutti i segmenti orientati equipollenti ad $\vec{AB}$ e posso sceglierlo come <u>rappresentante</u> della classe di equipollenza di $\vec{AB}$.

Quindi abbiamo una biezione:

$V=\{$Vettori geometrici nel piano$\}\{$segmento orientato $\vec{OP}, P\in\Pi\}$

Classi di equipollenza $\uparrow$                                              $\uparrow$ Stesso punto di applicazione

# <mark>Geometria e algebra 09/03/22</mark>

Correzione della definizione di campo:

- Esistenza dell'elemento neutro
  
  $\exist 0\in\R:x+0=0+x=x,\forall x\in\R$

- Esistenza dell'opposto:
  
  $\exist x'\in\R:x+x'=x'+x=0,\forall x\in\R$

---

Fissiamo $O\in\pi$ (piano ordinario).

$V=\{$vettori geometrici del piano$\}\Leftrightarrow\{$segmenti orientati$\vec{OP},P\in\pi\}$

Con un abuso di notazione, consideriamo:

$V=\{$segmenti orientati$\vec{OP},P\in\pi\}$

$\forall\vec{v}\in V,\exist P\in\pi:\vec{v}=\vec{OP}$

<u>Operazioni su $V$</u>:

- <u>somma di vettori</u>
  
  siano $\vec{v},\vec{w}\in V$ e siano $P,Q\in\pi:$
  
  $\vec{v}=\vec{OP}$
  
  $\vec{w}=\vec{OQ}$
  
  Definiamo:
  
  $\vec{v}+\vec{w}=\vec{OR}$, tale che il quadrilatero $OPRQ$ è un parallelogramma. (regola del parallelogramma)
  
  <u>Nota</u>: Se $O,P$ e $Q$ sono collineari (hanno la stessa direzione),  costruisco $R$ tale che $OQ$ e $RP$ hanno la stessa lunghezza
  
  Operazione binaria interna: $+: V\times V\rightarrow V$
  
                                                            $(\vec{v},\vec{w})\rightarrow \vec{v}+\vec{w}$

- <u>Moltiplicazione per scalari</u>
  
  Sia $\vec{v}\in V$ e sia $P\in\pi:\vec{v}=\vec{OP}$.
  
  Definiamo $\lambda\cdot\vec{v}=\vec{OR}$
  
  - $O,P,R$ sono collineari
  
  - $OR (simbolo\ di\ segmento\ su\ OP)=|\lambda|OP$
  
  - $\vec{OR}$ è orientato concordemente a $\vec{OP}$
    
    $\vec{OR}$ è orientato discordemente a $\vec{OP}$ se $\lambda<0$
    
    se $\lambda=0, R=O$
  
  Questa è un'operazione binaria <u>esterna</u>: $\cdot:\R\times\mathbb{V}\rightarrow V$
                                                                                     $(\lambda,\vec{v})\rightarrow\lambda\cdot\vec{v}$

        <u>Piano Cartesiano</u>

        $\{P:P\in\pi\}\leftrightarrow\{(x,y):x,y\in\R\}=\R^2$

        $V=\{$segmenti orientati$\vec{OP},P\in\pi\}=\{$vettori geometrici nel piano$\}$

        In particolare esiste una blezione:

                        $V\leftrightarrow\R^2$

              $\forall P\in\pi,\vec{OP}\rightarrow(x,y)$, dove $x,y$ sono rispettivamente ascissa e ordinata di $P$

                        $\vec{OP}\leftarrow(x,y)$ dove $P(x,y)$

        Vogliamo tradurre le operazioni su $V$ in operazioni su $\R^2$:

        1. $\vec{v}=\vec{OP},P(x_P,y_P)$

            $\vec{w}=\vec{OQ},Q(x_Q,y_Q)$

            $\vec{v}+\vec{w}=\vec{OR}:$ quali sono le coordinate di R?

            $OPQR\Rightarrow A(x_A,y_A)$ parallelogramma con punto medio di $PQ$ e $OR$

            $A$ punto medio di $PQ\Rightarrow\{x_A=\frac{x_P+x_Q}{2}, y_A=\frac{y_P+x_Q}{2}\}$

            $A$ punto medio di $OR\Rightarrow\{x_A=\frac{x_R}{2},y_A=\frac{y_R}{2}\}$

            $\Rightarrow\{x_R=x_P+x_Q,y_R=y_P+y_Q\}$

            Operazione binaria <u>interna</u>: $+:\R^2\times\R^2\rightarrow\R^2$

                                                                      $((x_1,y_1),(x_2,y_2))\mapsto(x_1+x_2,y_1+y_2)$

---
# Da qui scrivo su vscode

2. $\vec{v}\in V,\vec{v}=\vec{OP},P(x_P,y_P), \lambda\in\R$

    $\lambda\cdot\vec{v}=\vec{OR}:$ quali sono le coordinate di R?

    $\vec{OR}=\lambda\cdot\vec{OP}$

    $OPH$ e $ORK$ sono simili per costruzione con rapporto di proporzioni $|\lambda|$.

    <u>Due casi</u>:
    - $\lambda\ge0$ $\vec{OR}$ è concord con $\vec{OP}$ e quindi:

        $x_R=|\lambda|x_P=\lambda x_P$

        $y_R=|\lambda|y_P=\lambda y_P$
    - $\lambda<0$ $\vec{OR}$ è discorde con $\vec{OP}$ e quindi:
        $x_R=-|\lambda|x_P=\lambda x_P$

        $y_R=-|\lambda|y_P=\lambda y_P$
    
    Operazione binaria <u>esterna</u>: $\cdot:\R\times\R^2\rightarrow\R^2$

    $(y,(x,y))\mapsto\lambda\cdot(x,y):=(\lambda x,\lambda y)$
    
    In conclusione abbiamo definito due operaizoni su $\R^2$ "compatibili" con le operazioni definite su $V$:

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

    <mark>Def</mark>: Sia $K$ (lettera K da "korper" in tedesco) un campo. Uno spazio vettoriale su $K$ è un insieme $V$ dotato di due operazioni:
      
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

    Gli elementi di $V$ sono chiamati vettori e gli elementi di $K$ son chiamati scalari.

    $K=\R:$ spazio vettoriale reale

    $K=\mathbb{C}:$ spazio vettoriale complesso
    
    <u>Osservazioni</u>: Sia $V$ un K-spazio vettiruake:

    - in $V$ esiste un unico vettore nullo che denotiamo <u>0</u>.
    - $\forall v\in V$ esiste un unico opposto che denotiamo $-v$
    - $\forall v\in V$ si ha $0\cdot v=$ <u>0</u>
    - $\forall\lambda\in K$ si ha $\lambda\cdot$ <u>0</u> $=$ <u>0</u>
    - Siano $\lambda\in K,v\in K: \lambda\cdot v=$ <u>0</u> $\Rightarrow$ o $v=$ <u>0</u>
# <mark>Geometria e algebra 16/03/22</mark>
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
1. $V=\{$Vettori geometrici nello spazio$\}=\{$segmenti orientati $\vec{OP},\ P$ nello spazio$\}\longleftrightarrow\R^3$

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

    $(k^n,+,\cdot)$ è uno spazio vettoriale su $K$ chiamato $n$-spazio vettoriale numerico su $K$.

    <u>Esempio</u>: $k=\mathbb{C},\ \mathbb{C}^n\\k=\mathbb{F}_2,\ \mathbb{F}^n_2$

  3. Funzioni da un insieme a un campo

     Sia $\mathbb{X}$ un insieme <u>qualunque</u> e $\mathbb{K}$ un campo

     $V=\{$funzioni $f:\mathbb{X}\to\mathbb{K}\}$

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
     
     $K[x]=\{$polinomi a coefficienti in $K$ in un'indetermiinata$\}$

     Molti problemi di matemadica/fisica hanno la proprietà che l'insieme delle soluzioni ha una struttura di spazio vettoriale.

     <u>Esempi</u>:

     - $$\begin{cases}x+2y+z=0\\y+7z=0\end{cases}$$

       $S=\{(x,y,z)\in\R^3:x+2y+z=0$ e $y+7z=0\}=\{(13t,-7t,t),t\in\R\}$
       $S$ ha una struttuta di spazio vettoriale (<mark>cose che vedremo più avanti</mark>)


