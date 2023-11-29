# Einfacher Prompt = Einfache Ausgabe

**Prompt:**

> Verbessere folgenden Text:
> 
> Das Universum ist so groß, dass wir nur einen winzigen Teil davon erforschen können. Es gibt schätzungsweise mehr als 100 Milliarden Galaxien, die jeweils Milliarden von Sternen und Planeten enthalten. Das Universum ist auch sehr alt, etwa 13,8 Milliarden Jahre. Es entstand aus einem extrem heißen und dichten Zustand, den wir den Urknall nennen. Das Universum ist voller mysteriöser Phänomene, wie schwarze Löcher, dunkle Materie und dunkle Energie. Diese beeinflussen die Struktur und die Entwicklung des Universums, aber wir wissen noch nicht genau, was sie sind oder wie sie funktionieren. Das Universum ist auch voller Schönheit und Wunder, wie die farbenfrohen Nebel, die aus Gas und Staub bestehen, die leuchtenden Sterne, die aus Wasserstoff und Helium bestehen, und die erstaunlichen Planeten, die aus verschiedenen Elementen und Verbindungen bestehen. Das Universum ist schließlich voller Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und die Erkenntnis unserer eigenen Herkunft und Bestimmung.

**Ergebnis:**

> Ich kann versuchen, den Text zu verbessern, indem ich einige Wörter ersetze, die Satzstruktur variieren und einige Übergänge hinzufüge. Hier ist mein Vorschlag:
> 
> Unser Universum ist so unermesslich groß, dass wir nur einen Bruchteil davon erkunden können. In ihm existieren vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Unser Universum ist auch sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. Unser Universum birgt viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend unbekannt. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Unser Universum bietet uns schließlich viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Learnings:**

* Einfache Eingaben liefern typischerweise einfache Ausgaben
* Genauere Erklärungen der Aufgabe(n) liefert typischerweise bessere Ergebnisse 

# Iteratives Prompting

Weiterführung vom vorherigen Beispiel:

**Prompt:**

> Mache den Text noch flüssiger

**Ergebnis:**

> Ich kann versuchen, den Text noch flüssiger zu machen, indem ich einige Wiederholungen vermeide, einige Konjunktionen einfüge und einige Adjektive verstärke. Hier ist mein Vorschlag:
> 
> Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. In unserem Universum gibt es viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese rätselhaften Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend ein Rätsel. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Schließlich bietet uns unser Universum viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Learnings:**

* Falls die initiale Ausgabe nicht passt, kann entweder
 * neu und mit präziserer Anfrage geprompted werden oder
 * iterativ im Chatverlauf die Anfrage präzisiert werden 

# Arbeiten auf eigenen Daten (Eigenen Artikel umschreiben)

**Prompt:**

> Schreibe eine Zusammenfassung für den folgenden Artikel, aber bitte nur einen Satz. Nutze ausschließlich Informationen aus dem Artikel. Die Zusammenfassung sollte nicht mit "Der Artikel" anfangen.
> 
> Artikel:
> Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. In unserem Universum gibt es viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese rätselhaften Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend ein Rätsel. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Schließlich bietet uns unser Universum viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Ergebnis:**

> Eine mögliche Zusammenfassung für den Artikel ist:
> 
> Das Universum ist ein riesiger, alter und geheimnisvoller Ort, der aus vielen Galaxien, Sternen und Planeten besteht, die uns Schönheit, Wunder und Fragen bieten.

**Learnings:**

* Gerade bei komplexen Aufgaben macht es Sinn die Eingabedaten (Kontext) sauber zu deklarieren
* Speziell wichtig falls mehrere Datenpunkte eingefügt werden

# Lernen Anhand von kurzen Beispielen (Tweet Erzeugung aus Text mit Beispielen)

**Prompt:**

> Schreibe mir bitte 5 Tweets zu folgendem Artikel. Schreibe in einem ähnlichen Stil wie die Beispiele. Antworte als Liste mit 1., 2., 3., usw.
> 
> Beispiele:
> * That's a wrap on day 1 of #MSIgnite 🎉
> * creating passwords shouldn't feel like rocket science 🚀 luckily, there's Password Generator
> * A cozy WFH set up courtesy of Bing Image Creator. 🍂
> 
> Artikel:
> Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. In unserem Universum gibt es viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese rätselhaften Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend ein Rätsel. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Schließlich bietet uns unser Universum viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Ergebnis:**

> Hier sind fünf Tweets, die ich zu dem Artikel geschrieben habe. Ich habe versucht, einen ähnlichen Stil wie die Beispiele zu verwenden. Ich hoffe, sie gefallen dir. 😊

> 1. Unser Universum ist voller Geheimnisse und Wunder. Erfahre mehr über schwarze Löcher, dunkle Materie und dunkle Energie in diesem spannenden Artikel. #BingWissen
> 2. Wie alt ist unser Universum? Woher kommt es? Was gibt es noch zu entdecken? Finde es heraus in diesem faszinierenden Artikel, der dir die Geschichte und die Zukunft unseres Universums erklärt. #BingFakten
> 3. Hast du dich jemals gefragt, wie unser Universum aussieht? Schau dir diese atemberaubenden Bilder von Galaxien, Sternen und Planeten an, die Bing Image Creator für dich erstellt hat. #BingBilder
> 4. Unser Universum ist so groß, dass wir nur einen winzigen Teil davon erkunden können. Aber das hält uns nicht davon ab, neugierig zu sein. Lies diesen Artikel, um mehr über die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung zu erfahren. #BingNeugier
> 5. Unser Universum ist ein Wunder der Natur. Es beherbergt über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Es hat seinen Ursprung in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. Es ist rund 13,8 Milliarden Jahre alt. Und es ist immer noch im Wandel. Lerne mehr über unser erstaunliches Universum in diesem Artikel. #BingWunder

**Learnings:**

* Beispiele helfen die Ausgabe in eine "bestimmte Richtung" zu lenken
* In unserem Beispiel werden die Beispiele "Bing"-ifiziert
* In unserem Beispiel wird aber auch schnell klar, dass die Beispiele sehr unpassend zum Text sind und daher suboptimale Ergebnisse liefern

# Prompts besser Formulieren (Markdown Formatting)

**Prompt:**

```
# Verhalten

* Als professioneller Journalist und Schreiber hilft du Zusammenfassungen in der verschiedenen Stilen zu verfassen
* Wenn du eine Zusammenfassung schreibst, dann benutze nur die Fakten die im Artikel genannt werden
* Erfinde keine weiteren Fakten oder Datenpunkte
* Antworte in einer Zusammenfassung im Stile der Süddeutschen Zeitung, Bild Zeitung und FAZ

# Formattierung

* Antworte in Markdown in Tabellenform
* Benutze ** um wichtige Stellen hervorzuheben

# Artikel

Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. In unserem Universum gibt es viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese rätselhaften Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend ein Rätsel. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Schließlich bietet uns unser Universum viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.
```

**Ergebnis:**

| Stil | Zusammenfassung |
|------|-----------------|
| Süddeutsche Zeitung| Unser Universum ist ein Ort voller Rätsel und Wunder. Es entstand vor 13,8 Milliarden Jahren aus einem Urknall und beherbergt über 100 Milliarden Galaxien mit unzähligen Sternen und Planeten. Wir wissen noch wenig über die geheimnisvollen Phänomene, die es prägen, wie schwarze Löcher, dunkle Materie und dunkle Energie. Wir staunen über die Schönheit und Vielfalt, die es uns zeigt, wie die farbenfrohen Nebel, die leuchtenden Sterne und die faszinierenden Planeten. Wir fragen uns nach dem Leben, dem Sinn und dem Schicksal, die es uns bietet. |
| Bild Zeitung | Das Universum ist der Hammer! Es ist riesig, alt und voller Geheimnisse. Es hat mit einem Mega-Knall angefangen und hat mehr Galaxien, als wir zählen können. Es gibt Sachen, die wir nicht verstehen, wie schwarze Loles, dunkles Zeug und dunkle Kraft. Es gibt Sachen, die uns umhauen, wie bunte Wolken, helle Sterne und coole Planeten. Es gibt Sachen, die uns neugierig machen, wie Aliens, andere Welten und unsere Zukunft. |
| FAZ | Das Universum, in dem wir leben, ist ein erstaunliches Phänomen. Es hat seinen Ursprung in einem Urknall, der vor 13,8 Milliarden Jahren stattfand, und umfasst mehr als 100 Milliarden Galaxien mit einer unvorstellbaren Anzahl von Sternen und Planeten. Es birgt viele Geheimnisse, die wir noch nicht entschlüsseln können, wie schwarze Löcher, dunkle Materie und dunkle Energie, die einen wesentlichen Einfluss auf seine Struktur und Entwicklung haben. Es offenbart uns auch viele Schönheiten und Wunder, die wir bewundern können, wie die farbigen Nebel, die aus Gas und Staub bestehen, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die vielfältigen Planeten, die aus verschiedenen Elementen und Verbindungen bestehen. Es stellt uns auch viele Fragen und Möglichkeiten, die wir erforschen wollen, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung. |

**Learnings:**

* Durch Markdown Formattierung und die Aufteilung in verschiedene Bereiche (Aufgabe, Antwortverhalten, Beispiele, etc.) kann dem Modell einfach eine Vielzahl an "Verhalten" mitgegeben werden
* Dadurch verstehen LLMs ihre Aufgabe oft "besser" (ähnlich Mensch)

# Formattierung der Ausgabe (Tabelle, Stichpunkte, etc.)

Die Ausgabe kann oft relativ einfach formatiert werden. So lassen sich zum Beispiel Tabellen, ungeordnete und geordnete Listen, etc. erzeugen.

**Prompt:**

Schreibe eine Zusammenfassung für den folgenden Artikel. Antworte wiefolgt:

1. Mit einer Tabelle (Spalten: Länge, Zusammenfassung) und schreibe eine Zusammenfassung der Länge 1, 2, und 3 Sätzen
2. Mit einer Liste an 3 Bulletpoints

Artikel:
Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen. In unserem Universum gibt es viele Geheimnisse, wie zum Beispiel schwarze Löcher, dunkle Materie und dunkle Energie. Diese rätselhaften Phänomene haben einen Einfluss auf die Struktur und die Entwicklung des Universums, aber ihre Natur und ihre Wirkungsweise sind uns noch weitgehend ein Rätsel. Unser Universum ist auch voller Schönheit und Wunder, wie die bunten Nebel, die aus Gas und Staub geformt sind, die strahlenden Sterne, die aus Wasserstoff und Helium bestehen, und die faszinierenden Planeten, die aus verschiedenen Elementen und Verbindungen zusammengesetzt sind. Schließlich bietet uns unser Universum viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Ergebnis:**

> Eine Zusammenfassung für den folgenden Artikel ist:
> 
> | Länge | Zusammenfassung |
> |---|----|
> | 1 Satz | Der Artikel beschreibt die Größe, das Alter, den Ursprung, die Geheimnisse, die Schönheit und die Fragen unseres Universums. |
> | 2 Sätze | Der Artikel beschreibt die Größe, das Alter, den Ursprung, die Geheimnisse, die Schönheit und die Fragen unseres Universums. Er erklärt, wie das Universum aus dem Urknall entstanden ist, wie es von schwarzen Löchern, dunkler Materie und dunkler Energie beeinflusst wird, und wie es aus Galaxien, Sternen, Planeten und Nebeln besteht. |
> | 3 Sätze | Der Artikel beschreibt die Größe, das Alter, den Ursprung, die Geheimnisse, die Schönheit und die Fragen unseres Universums. Er erklärt, wie das Universum aus dem Urknall entstanden ist, wie es von schwarzen Löchern, dunkler Materie und dunkler Energie beeinflusst wird, und wie es aus Galaxien, Sternen, Planeten und Nebeln besteht. Er erwähnt auch, dass unser Universum viele Rätsel und Möglichkeiten bietet, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung. |
> 
> Eine Liste an 3 Bulletpoints ist:
> 
> * Das Universum ist sehr groß, alt und hat seinen Ursprung im Urknall
> * Das Universum hat viele Geheimnisse, wie schwarze Löcher, dunkle Materie und dunkle Energie, die seine Struktur und Entwicklung beeinflussen
> * Das Universum ist voller Schönheit und Wunder, wie Galaxien, Sterne, Planeten und Nebel, und bietet uns viele Fragen und Möglichkeiten, wie die Suche nach außerirdischem Leben, die Erforschung anderer Welten und das Verständnis unserer eigenen Herkunft und Bestimmung.

**Learnings:**

* LLMs können einfach in verschiedenen Formaten antworten
* Ermöglicht einfache Verarbeitung in anderen Applikationen, wie z.B. Excel

# Zusammenfassungen, umschreiben, korrigieren

**Prompt:**

>

**Ergebnis:**

> 

**Learnings:**

* 

# Übersetzungen

**Prompt:**

> Übersetze folgenden Text in Englisch, Spanish und Niederländisch. Antworte mit * Sprache: Übersetzung
> Text:
> Das Universum, in dem wir leben, ist so unermesslich groß, dass wir nur einen winzigen Bruchteil davon erkunden können. Es beherbergt vermutlich über 100 Milliarden Galaxien, die jeweils aus Milliarden von Sternen und Planeten bestehen. Außerdem ist es sehr alt, rund 13,8 Milliarden Jahre. Seinen Ursprung hat es in einem extrem heißen und dichten Zustand, den wir als Urknall bezeichnen.

**Ergebnis:**

> Ich habe den Text in die gewünschten Sprachen übersetzt. Hier sind die Ergebnisse:
> 
> * Englisch: The universe we live in is so immensely large that we can only explore a tiny fraction of it. It probably contains over 100 billion galaxies, each consisting of billions of stars and planets. It is also very old, about 13.8 billion years. It originated from an extremely hot and dense state that we call the Big Bang.
> * Spanisch: El universo en el que vivimos es tan inmensamente grande que solo podemos explorar una pequeña fracción de él. Probablemente contiene más de 100 mil millones de galaxias, cada una compuesta por miles de millones de estrellas y planetas. También es muy antiguo, unos 13.800 millones de años. Se originó a partir de un estado extremadamente caliente y denso al que llamamos Big Bang.
> * Niederländisch: Het universum waarin we leven is zo enorm groot dat we er maar een klein deel van kunnen verkennen. Het bevat waarschijnlijk meer dan 100 miljard sterrenstelsels, die elk bestaan uit miljarden sterren en planeten. Het is ook erg oud, zo’n 13,8 miljard jaar. Het is ontstaan uit een extreem hete en dichte toestand die we de oerknal noemen.

**Learnings:**

* Die meisten LLMs beherrschen gängigen Sprachen sehr gut
* Für kleinere Sprachen ist aber Vorsicht geboten, da es hier oft nur wenige Trainingsdaten gab --> Übersetzungen ggf. von niedriger Qualität 

# Ideenfindung

**Prompt:**

>

**Ergebnis:**

> 

**Learnings:**

* 

# Sehr lange Text schreiben lassen

**Prompt:**

>

**Ergebnis:**

> 

**Learnings:**

* Die meisten Modelle können nur eine begrenzte Anzahl an Text schreiben
* Es hilft


# Weitere Resourcen

[Wie schreibe ich den perfekten Prompt?](https://outrageous-drawbridge-12e.notion.site/Wie-schreibe-ich-den-perfekten-Prompt-9e33917cd43549fd83d332abc41e5240)
[Prompt-Bibliothek F3](https://outrageous-drawbridge-12e.notion.site/d16aa981eca442e7be4b82042373785d?v=40a3faa7f91a44c6877348fc5b597846)