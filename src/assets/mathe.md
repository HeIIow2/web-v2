# Bruchfunktionen

# Ableitungen

Die Ableitung ist die Funktion, die die Änderung einer anderen Funktion beschreibt.

$f(x)$ | $f'(x)$
---|---
$x^n$ | $n \cdot x^{n-1}$
$3 \cdot x^4$ | $12 \cdot x^3$
$4 \cdot x = 4 \cdot x^1$ | $4 = 4\cdot1\cdot x^0$  
$ax^2 + bx + c$ | $2ax + b$  
$e^x$ | $e^x$
$n \cdot e^x$ | $n \cdot e^x$  
$e^{g(x)}$ | $g'(x) \cdot e^{g(x)}$

$$f = \sin \quad f' = \cos \quad f'' = -\sin \quad f''' = -\cos \quad f'''' = \sin$$

## Summenregel

Sind Teile einer Funktion von $+$ oder $-$ getrennt, so wird jeder dieser Teile abgeleitet:

$$f(x) = u(x) + v(x)\qquad f'(x) = u'(x) + v'(x)$$

## Produktregel

Sind Teile einer Funktion von $\cdot$ abgetrennt, so wird die Produktregel angewandt:  

$$f(x) = u \cdot v\qquad f'(x) = u' \cdot v + u \cdot v' $$

## Kettenregel

$$f(x) = u(v(x)) \qquad f'(x) = u'(v(x)) \cdot v'(x)$$

# Kurvendiskussion

[Referenz](https://studyflix.de/mathematik/kurvendiskussion-aufgaben-3117)

## Definitionsbereich

## y-Achsenabschnitt

## x-Achsenabschnitt (Nullstellen)

Die Nullstellen sind die Punkte, an denen der Graph die x-Achse schneidet.

Der $x$ Wert ergibt sich, wenn man die Funktion mit $0$ gleichstellt, und nach $x$ auflößt:

$$f(x) = 0 \qquad P(x\;|\;0)$$

### Quadratische Funktion (ABC-Formel)

Hat man eine quatratische Funktion, lässt sich die Nullstelle mithilfe der ABC-Formel ermitteln:

$$f(x) = ax^2 + bx + c \qquad x_{1,2} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

## Verhalten im Unendlichen

## Symmetrie verhalten

## Extrempunkte

Extrempunkte sind alle Hoch/Tiefpunkte einer Funktion. Folgendes ist bei einem Extrempunkt gegeben:   
 - $f'(x) = 0$

Bedingung | Art d. Punktes
---|---
$f''(x) < 0$ | Hochpunkt
$f''(x) = 0$ | Sattelpunkt
$f''(x) > 0$ | Tiefpunkt

## Monotonieverhalten

## Wendepunkte

Bei einem Wendepunkt ändert sich die Richtung. Die Richtung kann man durch die erste Ableitung beschreiben. Diese geht vom positiven ins Negative oder anders herum. In beiden fällen impliziert das jedoch, das die Änderung der Richtung *(die zweite Ableitung)* Null sein muss.

$$f''(x) = 0\qquad W(x|f(x))$$

# Tagngente Aufstellen

Man hat die Funktion $f(x)$ und will die Tangente an dem x-Wert $P_x$ finden.  
Eine Lineare Funktion hat folgende Form:
$$y = a \cdot x + c$$

## Steigung

Um die Steigung $a$ der Tangente zu berechnen, muss man die [Ableitung](#ableitungen) der Funktion $f$ berechnen. Dann setzt man $P_x$ ein:

$$a = f'(P_x)$$

## Verschiebdings

Als erstes muss man den Punkt bekommen, durch den die Tangente durchgehen soll. Da man den x-Wert schon hat ist dies einfach:

$$f(P_x) = P_x\qquad P (P_x|P_y)$$

Jetzt $c$ zu finden ist einfach. Man setzt ein und löst für $c$ auf.

$$P_y = a \cdot P_x + c$$
$$c = P_y - a \cdot P_x$$

# Stammfunktionen

Stammfunktionen sind essenziell für Integrale. Die beste Beschreibung wäre das Gegenteil einer **Ableitung**, eine "*Aufleitung*".

$f(x)$ | $F(x) + C$
-------|------------
$x^n$  | $\frac{1}{n + 1} \cdot x^{n + 1} = \frac{x^{n+1}}{n+1}$  
$x^4$ | $\frac{1}{5} \cdot x^5$  
$9 \cdot x^7$ | $\frac{9}{8} \cdot x^8$  
$n \cdot e^x$|$n \cdot e^x$
$e^{g(x)}$ | $\frac{1}{g'(x)} \cdot e^{g(x)} = \frac{e^{g(x)}}{g'(x)}$  
$e^{3x + 4}$ | $\frac{1}{3} e^{3x + 4} = \frac{e^{3x +4}}{3}$  
$10 \cdot e^{4x-8}$ | $\frac{20}{4} \cdot e^{4x-8}$  
$\frac{k}{x^n}$ | $\frac{-n \cdot k + k}{x^{n-1}}$  
$\frac{4}{x^2}$ | $- \frac{4}{x}$


Für Sinus und Cosinus siehe [Ableitungen](#ableitungen).

# Integrale

![Beispiel Graph](./assets/integral_example_small.png)

Ein Integral berechnet den Flächeninhalt unter einer Funktion.  
Die größere Zahl steht bei einem Integral *meist* oben: $n > k$. 

## Funktion und x-Achse

$$\int_k^n g(x)\; dx = \Big[ G(x) \Big]_k^n = G(n) - G(k)$$
 
Die Form die ich hier angegeben habe gilt, wenn man den Flächeninhalt der Funktion $g(x)$ in dem Intervall $n - k$, und der X-Achse finden will. Die nötigen Schritte sind:

1. man berechnet die [Stammfunktion](#stammfunktionen) von $g(x)$
2. man setzt beide Zahlen des Abschnitts in diese ein und rechnet das Ergebnis der größeren Zahl minus dem Ergebniss der kleineren Zahl:  
   $G(n) - G(k)$

## Funktion und y-Achse

Will man das gleiche mit der y-Achse machen, so bildet man die Kehrfunktion, 
$$y = x + 1 \qquad x = y - 1$$  
und macht die gleichen Schritte mit dieser.

Visuell dreht man einfach die Funktion um.

## Funktion und eine andere Funktion

Möchte man den Flächeninhalt berechnen von 2 Funktionen in einem bestimmten Intervall, wie Beispielsweise die graue Fläche in dem obigen Bild so ist dies auch nicht viel schwerer. Man muss in dem Intervall die Funktion mit dem größeren Flächeninhalt minus die Funktion mit dem kleineren berechnen. Weiß man dies nicht, kann man auch den Betrag einer Funktion minus der anderen berechnen.

$$\int_k^n \left(g(x) - f(x)\right) dx = \Big[ G(x) - F(x) \Big]_k^n = (G(n) - F(n)) - (G(k) - F(k))$$

Hier ist es besonders sinnvoll zu vereinfachen wo man kann, sonst wird es sehr schnell zu komplex.
