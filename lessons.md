# Einleitung

Alle Beispiele in diesem Dokument kommen aus [Bing Chat](https://www.bing.com/chat) im "More Creative" Modus.

Beim Schreiben von Prompts, sind folgende Punkte wichtig:

- **Aufgabenstellung und Zielklarheit:** Was ist die konkrete Aufgabe und was genau wollen wir erreichen?
- **Rolle/Persona:** An welchem Vorbild soll sich der Chatbot orientieren bzw. in welche Rolle soll er schlüpfen?
- **Format:** Welches Format und welchen Umfang soll der Output haben? In welcher Tonalität oder (Programmier-)Sprache soll der Text geschrieben werden?
- **Kontext:** Was ist der Kontext und welche Informationen sind für die Beantwortung der Frage relevant? Welche Quellen, Daten oder Methoden sollen in die Antwort einfließen (insbesondere bei Chatbots mit Zugriff auf das Internet relevant)? Welche Themen oder Inhalte sollen nicht berücksichtigt werden?
- **Zielgruppe:** Wen wollen wir ansprechen?
- **Schritte:** In welcher Reihenfolge soll der Chatbot unsere Anweisungen befolgen?

**Wichtig:**

- Es sind nicht zwangsweise alle Punkte notwendig, die Aufgabenstellung wird jedoch immer benötigt!
- Neuere Modelle folgende den Anweisungen typischerweise besser, brauchen daher aber auch ggf. detailiertere Arbeitsanweisungen.

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

```
Schreibe mir 10 Titel für Blogartikel im Bereich "Strom Sparen". Benutze folgende SEO Begriffe:
* Strom sparen Tipps
* Strom sparen Haushalt
* Strom sparen Geräte
* Energieeffizienz
```

**Ergebnis:**

> Hallo, das ist Bing. Ich kann dir helfen, einige Titel für Blogartikel im Bereich “Strom Sparen” zu schreiben. Hier sind 10 mögliche Titel, die du verwenden kannst:
> 
> Strom sparen Tipps: Wie du mit einfachen Tricks deine Stromrechnung senken kannst
> Strom sparen Haushalt: Die besten Energieeffizienz-Maßnahmen für dein Zuhause
> Strom sparen Geräte: Welche Geräte verbrauchen am meisten Strom und wie du sie effizienter nutzen kannst
> Energieeffizienz: Was ist das und warum ist es wichtig für die Umwelt und deinen Geldbeutel
> Strom sparen im Winter: So heizt du dein Haus ohne hohe Kosten
> Strom sparen im Sommer: So kühlst du deine Wohnung ohne Klimaanlage
> Strom sparen mit erneuerbaren Energien: Wie du Solar-, Wind- und Wasserkraft für deinen Haushalt nutzen kannst
> Strom sparen mit Smart Home: Wie du deine Geräte mit deinem Smartphone steuern und optimieren kannst
> Strom sparen mit LED-Lampen: Wie du deine Beleuchtung umweltfreundlicher und günstiger gestalten kannst
> Strom sparen mit Ökostrom: Wie du einen grünen Stromanbieter findest und wechselst

**Learnings:**

* Hier hift es oft iterativ vorzugehen, da oft nicht klar ist, was das Modell antworten wird
* Oft gehen die Ideen vom Modell in eine andere Richtung wie ursprünglich erwartet, was iteratives Prompting sehr effektiv machen kann

# Sehr lange Text schreiben lassen

Die meisten Modellen können nur eine endliche, oft relativ begrenzte Länge an Output erzeugen. Um dies zu überlisten, können wir iterativ vorgehen.

Zuerst erzeugen wir den Buchtitel, Charaktäre und Kaptilzusammenfassungen:

**Prompt 1:**

```
# Aufgabestellung

* Agiere als erfolgreicher Kinderbuchauthor, der fesselnde Geschichten für Kleinkinder schreibt.
* Schreibe mir eine Story über einen Elephanten der im Weltraum umher reist und verschiedene Planeten besucht.

# Verhalten

* Antworte mit Buchtitel und einer kurzen Beschreibung über die gesamte Geschichte
* Antworte zusätzlich mit einer Liste an Charakteren die im Buch vorkommen (Name, kurze Beschreibung und typisches Verhalten)
* Antworte mit einer Liste an 5 Kapiteln mit deren Überschrift und einer Beschreibung, was in jedem Kapitel passiert.
```

**Ergebnis:**

> Eine mögliche Geschichte über einen Elefanten, der im Weltraum umherreist und verschiedene Planeten besucht, ist:
> 
> **Buchtitel:** Elefant im All
> **Kurze Beschreibung:**
> Der kleine Elefant Elli träumt davon, die Sterne zu sehen. Er ist fasziniert von den Geschichten, die sein Großvater ihm über das Weltall erzählt. Eines Tages findet er eine geheimnisvolle Rakete im Dschungel und beschließt, sie auszuprobieren. Er startet in den Himmel und erlebt ein fantastisches Abenteuer. Er besucht verschiedene Planeten, lernt neue Freunde kennen und entdeckt die Schönheit und Vielfalt des Universums.
> 
> **Charaktere:**
> Elli: Er ist ein neugieriger und mutiger Elefant, der gerne neue Dinge lernt. Er ist freundlich und hilfsbereit, aber manchmal auch etwas tollpatschig. Er liebt seinen Großvater und seine Familie sehr.
> Großvater: Er ist ein weiser und liebevoller Elefant, der Elli viele Geschichten über das Weltall erzählt. Er war früher ein berühmter Astronaut und hat die Rakete gebaut, die Elli findet. Er ist stolz auf Elli und unterstützt ihn bei seinem Traum.
> Luna: Sie ist eine niedliche und schüchterne Mondhäsin, die Elli auf dem Mond trifft. Sie ist einsam und wünscht sich einen Freund. Sie zeigt Elli die Geheimnisse des Mondes und verliebt sich in ihn.
> Mars: Er ist ein frecher und lustiger Marsmännchen, der Elli auf dem Mars trifft. Er ist ein großer Fan von Erdmusik und tanzt gerne. Er bringt Elli bei, wie man auf dem Mars Spaß hat und schließt sich ihm an seiner Reise an.
> Jupiter: Er ist ein mächtiger und majestätischer Gasriese, der Elli auf dem Jupiter trifft. Er ist der König des Sonnensystems und hat viele Monde als Diener. Er ist beeindruckt von Elli und schenkt ihm einen Ring als Zeichen seiner Freundschaft.
> 
> **Kapitel:**
> Kapitel 1: Der Traum vom Weltall: Elli hört eine Geschichte von seinem Großvater über das Weltall und wünscht sich, die Sterne zu sehen. Er findet eine Rakete im Dschungel und beschließt, sie auszuprobieren. Er startet in den Himmel und ist begeistert von dem, was er sieht.
> Kapitel 2: Der Mond und die Mondhäsin: Elli landet auf dem Mond und trifft Luna, eine Mondhäsin, die sich nach einem Freund sehnt. Sie zeigt Elli die Krater, die Berge und die dunkle Seite des Mondes. Sie verbringen eine schöne Zeit zusammen und Elli verspricht ihr, wiederzukommen.
> Kapitel 3: Der Mars und das Marsmännchen: Elli fliegt zum Mars und trifft Mars, ein Marsmännchen, das Erdmusik liebt. Er zeigt Elli die roten Felsen, die Vulkane und die Eiswüste des Mars. Sie tanzen und lachen zusammen und Mars schließt sich Elli an seiner Reise an.
> Kapitel 4: Der Jupiter und der Gasriese: Elli fliegt zum Jupiter und trifft Jupiter, ein Gasriese, der der König des Sonnensystems ist. Er zeigt Elli die Wolken, die Stürme und die Ringe des Jupiter. Er ist beeindruckt von Elli und schenkt ihm einen Ring als Zeichen seiner Freundschaft.
> Kapitel 5: Die Rückkehr zur Erde: Elli verabschiedet sich von seinen Freunden und fliegt zurück zur Erde. Er erzählt seinem Großvater von seinem Abenteuer und zeigt ihm die Geschenke, die er bekommen hat. Er dankt ihm für seine Geschichten und sagt ihm, dass er ihn liebt. Er schläft ein und träumt von seinem nächsten Ausflug ins Weltall.

Nun können wir die Kapitel ausschreiben:

**Prompt 2 und weitere:**

```
# Aufgabestellung

* Agiere als erfolgreicher Kinderbuchauthor, der fesselnde Geschichten für Kleinkinder schreibt.
* Du schreibst gerade das 1. Kapitel für das Buch "Elefant im All" auf Basis der Kapitelzusammenfassung weiter unten
* Du nutzt ausschließlich die Charaktere die unten genannt werden. Du erfindest keine weiteren Charaktere für die Story
* Das Kapitel soll 3 Absätze lang sein

# Charaktere

* Elli: Er ist ein neugieriger und mutiger Elefant, der gerne neue Dinge lernt. Er ist freundlich und hilfsbereit, aber manchmal auch etwas tollpatschig. Er liebt seinen Großvater und seine Familie sehr.
* Großvater: Er ist ein weiser und liebevoller Elefant, der Elli viele Geschichten über das Weltall erzählt. Er war früher ein berühmter Astronaut und hat die Rakete gebaut, die Elli findet. Er ist stolz auf Elli und unterstützt ihn bei seinem Traum.
* Luna: Sie ist eine niedliche und schüchterne Mondhäsin, die Elli auf dem Mond trifft. Sie ist einsam und wünscht sich einen Freund. Sie zeigt Elli die Geheimnisse des Mondes und verliebt sich in ihn.
* Mars: Er ist ein frecher und lustiger Marsmännchen, der Elli auf dem Mars trifft. Er ist ein großer Fan von Erdmusik und tanzt gerne. Er bringt Elli bei, wie man auf dem Mars Spaß hat und schließt sich ihm an seiner Reise an.
* Jupiter: Er ist ein mächtiger und majestätischer Gasriese, der Elli auf dem Jupiter trifft. Er ist der König des Sonnensystems und hat viele Monde als Diener. Er ist beeindruckt von Elli und schenkt ihm einen Ring als Zeichen seiner Freundschaft.

# Kapitelzusammenfassung

Der Traum vom Weltall: Elli hört eine Geschichte von seinem Großvater über das Weltall und wünscht sich, die Sterne zu sehen. Er findet eine Rakete im Dschungel und beschließt, sie auszuprobieren. Er startet in den Himmel und ist begeistert von dem, was er sieht.
```

**Ergebnis:**

> Das klingt nach einer spannenden Geschichte! Ich werde versuchen, das erste Kapitel für dich zu schreiben. Hier ist mein Vorschlag:
> 
> Elli liebte es, seinem Großvater zuzuhören, wenn er ihm Geschichten über das Weltall erzählte. Er erzählte ihm von den Planeten, den Sternen, den Monden und den Asteroiden. Er erzählte ihm von seiner Zeit als Astronaut, als er die Erde aus dem Fenster seiner Rakete sah. Er erzählte ihm von den Wundern, die er erlebt hatte, und den Gefahren, die er überwunden hatte. Elli war fasziniert von allem, was sein Großvater sagte. Er wünschte sich, er könnte auch das Weltall sehen.
> 
> Eines Tages, als er durch den Dschungel spazierte, entdeckte er etwas Seltsames. Es war eine große, silberne Röhre, die zwischen den Bäumen versteckt war. Er ging näher heran und sah, dass es eine Rakete war. Er erkannte sie sofort. Es war die Rakete, die sein Großvater gebaut hatte, als er noch jung war. Er hatte ihm oft davon erzählt. Elli war neugierig und mutig. Er beschloss, die Rakete auszuprobieren. Er kletterte in das Cockpit und drückte auf einen roten Knopf.
> 
> Die Rakete zischte und rumpelte. Sie hob vom Boden ab und schoss in den Himmel. Elli spürte, wie sein Herz schneller schlug. Er sah aus dem Fenster und konnte seinen Augen nicht trauen. Er sah die Erde schrumpfen, bis sie wie eine blaue Murmel aussah. Er sah die Wolken, die Sonne, den Mond und die Sterne. Er sah das Weltall. Er war begeistert von dem, was er sah. Er wollte mehr sehen. Er wollte die Planeten besuchen, die sein Großvater ihm beschrieben hatte. Er wollte seine eigenen Abenteuer erleben. Er wollte ein Elefant im All sein.

**Learnings:**

* Die meisten Modelle können nur eine begrenzte Anzahl an Text schreiben
* Es hilft iterativ vorzugehen, wichtig dabei ist die relevanten Informationen in die weiteren Schritte als Kontext mitzugeben
* **Achtung:** Dieses Vorgehen ist natürlich nicht perfekt und bedarf definitiv einiges an manueller Arbeit

# Weitere Resourcen

Dieses Dokument ist nur ein kleiner Auszug aus einigen Methoden im Prompting:
* Zero-Shot, Few-Shot Prompting --> Wurden hier behandelt
* Chain-of-Thought (CoT), Tree-of-Thoughts (ToT) --> Wurden hier nicht behandelt
* Retrieval Augmented Generation (RAG) --> Wurden hier nicht behandelt
* ReAct (Reason and Act) --> Wurden hier nicht behandelt
* Automatic Prompt Engineer (APE) --> Wurden hier nicht behandelt

Quellen:
[Wie schreibe ich den perfekten Prompt?](https://outrageous-drawbridge-12e.notion.site/Wie-schreibe-ich-den-perfekten-Prompt-9e33917cd43549fd83d332abc41e5240)
[Prompt-Bibliothek F3](https://outrageous-drawbridge-12e.notion.site/d16aa981eca442e7be4b82042373785d?v=40a3faa7f91a44c6877348fc5b597846)