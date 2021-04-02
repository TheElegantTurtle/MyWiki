* domanda: Sotto quali condizioni un sistema hamiltoniano (dimensione 2n) è integrabile?
* idea: cerchiamo [trasformazione canonica](funzioni-generatrici.md) $(p,q)->(x,y)$ che semplifichi il sistema
   - ovvero $H(p,q)=K(x)$ in modo che il sistema diventa $dx/dt=0$, $dy/dt=w(x)$
        + il sistema è integrabile: $x(t)=cost$, $y(t)=w(x)t+c$
   - significa richiedere che la funzione generatrice soddisfi eq differenziale $H(dS/dq,q)=K(x)$
   - gli $x_i=F_i(p,q)$ sono integrali primi del moto in involuzione
* **T**: Se ho n funzioni $F_i$ in involuzione fra loro in un intorno di
    $(q_0,p_0)$ e i loro gradienti sono l.i. in $(q_0,p_0)$ allora esistono n funzioni lisce
    $G_i$ definnite in un intorno di $(q_0,p_0)$ che completano la trasformazione
    $(p,q)->(F_1...F_n,G_1...G_n)=(x,y)$
    1. Siccome i gradienti delle $F_i$ sono l.i. n colonne della matrice nx2n JF sono l.i.
    2. Dopo trasformazioni canoniche di permutazione delle coordinate ottengo una sottomatrice dxd invertibile, ad es $F_p=dF/dp$
    3. [Dini] mi dice che $x=F(p,q)$ può essere localmente risolta per p, ovvero $p=P(x,q)$, $P_x=F_p^{-1}$, $P_q=-F_p^{-1}F_q$
    4. ${F_i,F_j}=0 => F_pF_q^T-F_qF_p^T=0$
    5. Moltiplico a destra per $F_p^{-T}$ e a sinistra per $F_p^{-1}$ ottenendo $-P_q^T+P_q=0$ ovvero $P_q$ è simmetrica
    6. Per [lemma di integrabilità](trasformazioni-simplettiche.md) P(x,q) è localmente il gradiente rispetto alle q di S(x,q$)
    7. $d^2S/dxdq=P_x=F_p^{-1}$ è invertibile dunque $y=dS/sx=G$, $p=dS/dq$ è trasformazione simplettica (x=F per costruzione)
    - Se le $F_i$ sono integrali del moto posso costruire il sistema semplificato
* problema: lemma locale, non mi dice nulla sulla dinamica del sistema
* **D** : Un sistema con hamiltoniana $H:McR^{2n}->R$ è detto completamente integrabile se esistono n funzioni lisce $F_i$ (con $F_1=H$)
    tali che
    1. $F_i$ sono i involuzione
    2. i loro granenti sono l.i. in ogni punto di M (passaggio da locale di lemma a globale)
    3. esistono per ogni t le traiettorie dei sistemi con hamiltoniane $F_i$ e queste traiettorie stanno in M
* noto che:
    - ora tutti i sistemi $F_i$ sono completamente integrabili ($F_1=H$ non riveste un ruolo speciale)
    - Quindi per il punto 1 tutti gli $F_j$ sono integrali del sistema con Hamiltoniana $F_i$
    - I flussi di ciascuna di queste Hamiltoniane commutano [lemma lubich pag 279]
