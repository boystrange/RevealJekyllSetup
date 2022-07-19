---
layout: slides
---

# Introduzione

Per scrivere un **blocco di slide**, creare un file con estensione
`.md` e la seguente intestazione:

``` md
---
layout: slides
---
```

All'interno del file, ogni slide consiste in un'intestazione di
primo livello (`#`, opzionale) seguita dal contenuto della slide.

Slide diverse possono essere **separate** una dall'altra da una
sequenza `%%%`.

%%%

# Formule inline

È possibile inserire **formule matematiche** come $\sin\alpha^2$ nel
testo racchiudendone il codice `LaTeX` in una coppia di simboli
`$`. Per esempio, la formula è stata ottenuta scrivendo

``` tex
$\sin\alpha^2$
```

nel testo.

%%%

# Formule display

Se si vuole inserire una formula in modo *display*, occorre
racchiuderla tra `` `$$ `` e `` $$` `` (notare il *backtick extra*
prima e dopo i `$$`). Per esempio, la formula

`$$
  \int_0^\infty f(x)
$$`

è ottenuta con il codice

``` tex
`$$
  \int_0^\infty f(x)
$$`
```

%%%

# Codice

Il codice si inserisce racchiudendolo entro tre backtick. La
sequenza di apertura di backtick è seguita dal nome del linguaggio
di programmazione usato nel codice.

## Esempio di codice Java

```java
public class Main {
	private int x;
	private int y; // questo è privato
}
```

## Esempio di codice Haskell

``` haskell
fibo :: Int -> Int
fibo 0 = 0
fibo 1 = 1
fibo n = fibo (n - 1) + fibo (n - 2)
```
