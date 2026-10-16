# GasLab BAT_FQ 🧪💨 | Gasos Ideals & Llei de Dalton

**GasLab** és una aplicació web educativa interactiva dissenyada específicament per a l'alumnat de **Física i Química de 1r de Batxillerat.**

L'eina permet practicar de manera autònoma i il·limitada la resolució numèrica de problemes sobre l'**equació d'estat dels gasos ideals**, **transformacions físiques** i la **Llei de Dalton de pressions parcials**, fent un èmfasi metodològic estricte en l'ús de **factors de conversió** en tots els passos de resolució, d'acord amb els criteris de correcció de batxillerat i de les proves d'accés a la universitat (PBAU).

## 📋 Taula de continguts

1. [Característiques Principals](#-característiques-principals)

2. [Estructura Pedagògica i Continguts](#-estructura-pedagògica-i-continguts)

   * [Mòdul 1: Entrenador de Problemes Algorítmic](#mòdul-1-entrenador-de-problemes-algorítmic)

   * [Mòdul 2: Formulari & Apunts Interactius](#mòdul-2-formulari--apunts-interactius)

3. [Metodologia: Resolució amb Factors de Conversió](#-metodologia-resolució-amb-factors-de-conversió)

4. [Eines d'Avaluació i Gestió d'Aula](#-eines-davaluació-i-gestió-daula)

5. [Tecnologies Utilitzades](#-tecnologies-utilitzades)

6. [Guia de Desplegament a GitHub Pages](#-guia-de-desplegament-a-github-pages)

7. [Incrustació a l'Aula Virtual Moodle](#-incrustació-a-laula-virtual-moodle)

8. [Autoria i Llicència](#-autoria-i-llicència)

## ✨ Característiques Principals

* **Aplicació Single-File (tot en un sol fitxer `index.html`):** No requereix servidors, Node.js ni bases de dades; s'executa a l'instant des de qualsevol navegador web (mòbil, tauleta o ordinador).

* **Generador Algorítmic Infinit:** Planteja enunciats amb dades numèriques i substàncies aleatòries ($O_2, N_2, CH_4, CO_2, CO, NO_2, H_2, C_3H_8, C_4H_{10}$), de manera que l'alumnat disposa de centenars d'exercicis diferents sense repeticions.

* **Alternança d'Incògnites:** L'aplicació no sol·licita sempre la mateixa variable: rota automàticament entre demanar volum ($V$), pressió ($P$), nombre de mols ($n$), temperatura ($T$), fracció molar ($X_i$) o pressió parcial ($P_i$).

* **Correcció Formativa Intel·ligent:** Accepta comes o punts decimals amb un marge de tolerància numèrica ($\pm 3\%$), acompanyat d'una justificació pas a pas detallada.

* **Renderització Matemàtica Neta (KaTeX):** Totes les fórmules i càlculs es mostren en notació matemàtica d'alta qualitat tipogràfica sense codi LaTeX en brut.

* **Suport Bilingüe Complet (Català / Castellano):** Commutador instantani a la capçalera que tradueix enunciats, unitats, pistes pedagògiques i resolucions.

## 🧠 Estructura Pedagògica i Continguts

L'aplicació està organitzada en dues seccions principals:

### Mòdul 1: Entrenador de Problemes Algorítmic

Organitzat per categories curriculars seleccionables mitjançant filtres:

1. **Gasos Ideals (**$P \cdot V = n \cdot R \cdot T$**):**

   * Càlcul de volum en bombones industrials a partir de la massa en $\text{kg}$.

   * Càlcul de la pressió exercida per una massa en grams dins un recipient rígid.

   * Càlcul del nombre de mols ($n$) a partir de pressions en $\text{mmHg}$ i temperatures en centígrads.

   * Càlcul de la temperatura absoluta ($T$ en $\text{K}$) necessària per a un estat determinat.

2. **Transformacions (Lleis Empíriques i Eq. General):**

   * **Llei de Boyle-Mariotte (isotèrmic,** $T = \text{ct}$**):** $P_1 \cdot V_1 = P_2 \cdot V_2$.

   * **Equació General dels gasos ideals:** $\frac{P_1 \cdot V_1}{T_1} = \frac{P_2 \cdot V_2}{T_2}$ davant canvis simultanis de pressió i temperatura.

3. **Llei de Dalton & Mescles:**

   * Mescles binàries (com $CO_2$ i $CO$ a partir de masses en grams): càlcul de mols de cada component, mols totals i pressió total $P_T$.

   * Mescles ternàries (exercici 12 dels apunts: $NO_2$, $H_2$, $O_2$): determinació aleatòria de pressió total, fracció molar ($X_i$) o pressió parcial ($P_i$).

4. **Densitat & Volum Molar:**

   * Càlcul de la densitat d'un gas en $\text{g/L}$ mitjançant l'expressió deduïda $P = \frac{d \cdot R \cdot T}{M}$.

   * Càlcul del volum ocupat en condicions normals ($\text{c.n.}: 0^\circ\text{C}, 1\text{ atm}$) aplicant el factor del volum molar ($22{,}4\text{ L/mol}$).

### Mòdul 2: Formulari & Apunts Interactius

* **Bloc 1: Lleis Experimentals dels Gasos:** Resum de Boyle-Mariotte, Charles, Gay-Lussac i Equació General.

* **Bloc 2: Equació d'Estat:** Fórmules fonamentals, deducció de la densitat i volum molar.

* **Bloc 3: Llei de Dalton:** Suma de pressions parcials, definició de fracció molar ($X_i = \frac{n_i}{n_T}$) i relació $P_i = X_i \cdot P_T$.

* **Eina de Conversió d'Unitats en Directe:** Convertidors interactius bidireccionals per a:

  * Temperatura: $^\circ\text{C} \leftrightarrow \text{K}$ ($T(\text{K}) = T(^\circ\text{C}) + 273{,}15$).

  * Pressió: $\text{mmHg} \leftrightarrow \text{atm}$ ($1\text{ atm} = 760\text{ mmHg}$).

  * Volum: $\text{mL} / \text{cm}^3 \leftrightarrow \text{L} / \text{dm}^3$.

## 📐 Metodologia: Resolució amb Factors de Conversió

L'aplicació evita les regles de tres simples mecàniques i prioritza la justificació quantitativa mitjançant **factors de conversió encadenats**, ensenyant a l'alumnat com es cancel·len les unitats:

* **Massa a mols:**

  $$
  m \text{ (g)} \cdot \frac{1\text{ mol}}{M\text{ (g)}} = n\text{ (mol)}
  $$

* **Canvi d'unitats de pressió:**

  $$
  P\text{ (mmHg)} \cdot \frac{1\text{ atm}}{760\text{ mmHg}} = P\text{ (atm)}
  $$

* **Volum molar en condicions normals:**

  $$
  n\text{ (mol gas)} \cdot \frac{22{,}4\text{ L gas}}{1\text{ mol gas}} = V_{\text{cn}}\text{ (L)}
  $$

* **Proporcions en canvis d'estat:** Expressió de la relació de compressió o expansió isotèrmica com a factor de pressió:

  $$
  V_2 = V_1 \cdot \frac{P_1}{P_2}
  $$

## 📊 Eines d'Avaluació i Gestió d'Aula

* **Identificador de l'Estudiant:** Camp per introduir el nom de l'alumne/a abans d'iniciar la pràctica.

* **Cronòmetre Flotant:** Permet mesurar el temps efectiu de treball, amb botons natius de pausa/represa i reinici.

* **Indicadors de Gamificació:** Marcador d'**Aciertos**, **Récord** de sessió i comptador de **🔥 Racha** consecutiva.

* **Desglossament per Categories:** Comptadors individuals per tipus de problema (*Ideals*, *Transf*, *Dalton*, *Densitat*).

* **Generació de PDF de Sessió:** En prémer el botó verd de la barra superior, es genera una finestra d'impressió amb un informe net que inclou:

  * Nom de l'alumne/a, data i temps emprat.

  * Balanç d'encerts, ratxa i problemes superats per categoria.

  * Breu memòria pedagògica del mètode de factors de conversió emprat per a la seva tramesa a Moodle.

## 🛠 Tecnologies Utilitzades

* **HTML5 & Vanilla JavaScript (ES6+):** Arquitectura reactiva lleugera sense dependències pesades ni entorns de compilació.

* **Tailwind CSS (CDN):** Disseny visual modern, responsive i accessible adaptat a tauletes i pantalles mòbils.

* **KaTeX (CDN) & Auto-render extension:** Processament d'alt rendiment per a la renderització immediata de les fórmules químiques i matemàtiques.

* **Font Awesome 6 (CDN):** Iconografia funcional per a la navegació i l'estatus dels exercicis.

```


```

## 👩‍🏫 Autoria i Llicència

* **Autora:** Elena Ruiz Alfaro

* **Curs acadèmic:** 2026-2027

Aquest material educatiu es distribueix sota la llicència **Creative Commons Reconeixement-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)**. En sou lliures de compartir, copiar i adaptar el codi sempre que se'n reconegui l'autoria original i no se'n faci un ús comercial.
