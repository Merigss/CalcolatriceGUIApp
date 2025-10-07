# 🧮 CalcolatriceGUIApp

Un progetto Java che implementa una **calcolatrice grafica (GUI)** con Java Swing.  
Permette di eseguire operazioni base (`+`, `-`, `×`, `/`) tra due numeri interi, con un’interfaccia moderna e intuitiva.

---

## ⚙️ Funzionalità principali

✅ Interfaccia grafica basata su Java Swing  
✅ Tasti numerici e operatori (+, -, ×, ÷)  
✅ Tasto **C** → cancella l’ultimo carattere  
✅ Tasto **AC** → resetta tutto a 0  
✅ Tasto **=** → calcola il risultato  
✅ Gestione dinamica dei valori (aggiunta numeri, operatori, reset)

---

## 🧩 Descrizione delle classi

### `CalcolatriceGUIApp`
Contiene il **main** e tutta la parte grafica: finestra, display e pulsanti.  
Ogni pulsante richiama metodi di `Util` per aggiornare il display e gestire le operazioni.

### `Util`
Classe di supporto che contiene:
- `addNumber(String, String)` → aggiunge cifre o operatori.
- `canc(String)` → cancella l’ultimo carattere o reimposta a “0”.
- `operazione(String)` → calcola il risultato con una `HashMap` di operatori.

### `OperatoreBinario`
Interfaccia funzionale con:
```java
int eval(int a, int b);
