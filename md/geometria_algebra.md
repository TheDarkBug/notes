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

| P   | Q   | $\neg$P | P^Q | P$\bigvee$Q | P$\Rightarrow$Q | P$\Leftrightarrow$Q |
| --- | --- | ------- | --- | ----------- | --------------- | ------------------- |
| 1   | 1   | 0       | 1   | 1           | 1               | 1                   |
| 1   | 0   | 0       | 0   | 1           | 0               | 0                   |
| 0   | 1   | 1       | 0   | 1           | 1               | 0                   |
| 0   | 0   | 1       | 0   | 0           | 1               | 1                   |

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

# qui manca la distributività

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

**<u>Def</u>**: Un vettore geometrico è una classe di equipollenti **MANCA LA FINE DELLA DEFINIZIONE**

Sia $O$ un punto fissato nel piano $\Pi$, per ogni segmento orientato $\vec{AB}$ esiste un punto $P\in\Pi$ tale che $\vec{OP}$ è equipollente ad $\vec{AB}$.

$\vec{OP}$ è equipollente a tutti i segmenti orientati equipollenti ad $\vec{AB}$ e posso sceglierlo come <u>rappresentante</u> della classe di equipollenza di $\vec{AB}$.

Quindi abbiamo una biezione:

$V=\{$Vettori geometrici nel piano$\}\{$segmento orientato $\vec{OP}, P\in\Pi\}$

Classi di equipollenza $\uparrow$                                              $\uparrow$ Stesso punto di applicazione
