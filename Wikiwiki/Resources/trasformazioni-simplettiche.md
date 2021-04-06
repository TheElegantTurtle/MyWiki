# Trasformazioni Simplettiche {#Trasformazioni Simplettiche}

-   Oggetti base: parallelogrammi $P$ in $R^{2d}$
    -   sono generati da 2 vettori di $u^T=(u^p,u^q)$ e $v^T=(v^p,v^q)$
        (componenti in $R^d$)
    -   per $d=1$ hanno area $u^p v^q - v^q u^p$ (determinante)
-   App bilineare $w(u,v)=u^T E v$ (E matrice simplettica)
    -   è somma delle aree dei parallelogrammi $2d$ ottenuti proiettando
        $P$ sui piani delle coordinate $(p_i,q_i)$
-   []{#D}**D** : App linare A è []{#simplettica}**simplettica** se
    $w(Au,Av)=w(u,v)$ per ogni $u,v$
    -   equivalente a $A^T E A = E$
-   []{#D}**D** : Funzione dif $g:U->R^{2d}$ è
    []{#simplettica}**simplettica** se per ogni punto di $U$,
    $w(J(g)u,J(g)v)=w(u,v)$ per ogni $u,v$
    -   idea: ogni funzione dif è localmente lineare
    -   interpretazione geometrica: M sottovarietà 2d immagine di K (in
        $R^2$) tramite f(s,t). M è unione di parallelogrammi generati da
        $df/ds(s,t) ds$ e $df/dt(s,t) dt$. Considero W somma di w
        applicata a tutti questi parallelogrammi (integrale di w su K)
        -   []{#T}**T** se g è simplettica $W(g(M))=W(M)$
            1.  Parametrizzo g(M)
            2.  Scrivo W(g(M))
            3.  Uso chain rule e simpletticità di g per ottenere W(M)
-   []{#T}**T** (Poincarè): H(p,q) funzione $C^2(U)$, allora il suo
    \[flusso\] $f_t$ è simplettico per ogni t fissato
    1.  calcolo derivata temporale di $Jf(y)^T E Jf(y)$ (lascio t
        implicito, $y=(p_0,q_0)$)
    2.  Jf(y) come soluzione di eq variazionale in cui compare hessiana
        di H (simmetrica)
    3.  Sostituendo trovo che derivata è 0
    4.  f_0=id e soddisfa $Jf(y)^T E Jf(y)=E$, dunque è soddisfatta per
        tutti t e tutti y
-   []{#T}**T** (Lemma di integrabilità) : Sia $g:U->R^n$ dif con
    continuità e sia Jg(y) simmetrica per tutti gli y in U, allora per
    ogni y in U esiste un intorno di y in cui è definita H tc
    $g=\grad H$.
    1.  Costruttiva
    2.  Definisco su una palla centrata in $y_0$
        $H(y)=\int_0^1 y^t g(ty)dt + cost$
    3.  Derivo rispetto a $y_k$
    4.  Dalla simmetria ($df_i/dy_k=df_k/dy_i$) segue la tesi
    5.  Il lemma resta valido per insiemi semplicemente connessi
-   []{#T}**T** : $g:U->R^{2d}$ dif con continuità, allora
    $\dot{y}=f(y)$ è localmente hamiltoniano se e solo se il suo flusso
    $f_t(y)$ è simplettico per tutti gli y in U e per t piccoli
    1.  =\> segue da teorema di Poincarè
    2.  \<= assumo f simplettico, dimostro che esiste localmente H
    3.  derivo rispetto al tempo Jf\^T E Jf
    4.  uso f soluzione di equazione variazionale e sostituisco
    5.  siccome E antisimmetrica, E Jf è simmetrica e dunque è gradiente
        di una funzione H per teorema precedente
