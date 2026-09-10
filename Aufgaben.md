# Aufgaben "Legacy Systeme verbessern mit Agentic Coding" Workshoptage Rapperswil 2026

7. Analyse<br>
  Repo-Check<br>
  Scoped Analysis der Applikation<br>
  Metriken & Archäologie / Hotspots
8. Optimierungsziel auswählen<br>
  dazu nötig: Detailanalyse, Rückfragen
9. Guardrails entwickeln
10. Plan erstellen
11. umsetzen
12. GOTO 7.3


## Aufgaben für TeilnehmerInnen

1. Nimm deinen Agenten in Betrieb. Stelle sicher, dass GLM 5.3 als Model ausgewählt ist, lasse dir die Anzahl Zeilen der Agents.md nennen (sollten knapp 120 sein), frage ob Subagents genutzt werden können und mache dich mit dem Style deines Agenten vertraut. Hinweis: GLM spricht Deutsch, aber total strubes Deutsch. Redet Englisch mit dem Agent, wenn ihr könnt.

2. Lasse den Agenten das Repository untersuchen, nutze dafür Step 1 des Skill Repo-x-ray und lasse das Ergebnis als Datei festhalten. Ggf. liest du den Skill kurz durch. Nach Abschluss, lese  die Ergebnisse. Hinterfrage und lass den Agent nachbessern, sofern dir etwas auffällt dass unklar ist oder für dich nicht sauber nachvollziehbar. Oft ist dies der Fall, wenn der Agent Informationen interpretiert bevor er sie auswertet. Beispiel: Agent wertet eine Klasse als Businesslogik weil sie Logik enthält, aber sie liegt im Package UI. Der Skill erzeugt auch eine Art Logfile, wo du nach konkreten Belegen - sowohl für die Erkenntnisse als auch für Probleme - suchen kannst.

3. Untersuche die Applikation im Repository mit Step 2 des Skills. Lese auch hier zuerst, was der Agent antwortet, gehe es konzentriert top-down durch und hinterfrage einzelne Aspekte der Ergebnisse, entweder weil sie dir merkwürdig vorkommen oder weil du nicht weisst wie sie entstanden sind. Wähle ein paar Metriken aus (entweder du oder lass dir helfen), von denen du glaubst dass wir sie verbessern könnten mit unseren Ansätzen. Lass dir dann vom Agenten ein Skript schreiben, um diese Metriken zu berechnen, damit wir das Skript später erneut laufen lassen können. <br><br>
Beantworte ausserdem zwei Fragen: Was glaubst du ist die wichtigste Erkenntnis bisher und was ist die grösste Überraschung soweit?

4. Lass den Agenten in Step 3 nun die einzelnen Erkenntnisse aus Step 2 bearbeiten um zu einer nochmals überprüften Liste von möglichen Improvements zu kommen, die nach einem festen Schema notiert und priorisiert wird. Ihr gebt die Priorisierung vor und solltet auch hier Punkte hinterfragen und euch Zusammenhänge und Begründungen erläutern lassen und sie challengen, wenn sie für euch nicht richtig erscheinen oder unverständlich sind. Am Ende von Step 3 solltet feststehen, welches Element zuerst bearbeitet wird. Empfehlung: Als erstes ein Testnetz bauen lassen.

5. Step 4 lass den Agenten implementieren. Schau gerne mal in die Ergebnisse, aber achte vor allem darauf dass der Agent sich daran hält die gesteckten Regeln einzuhalten.

6. Step 5 des Skills, lass nochmal unabhängig eine Validierung durchführen um zu bestätigen dass alle Ziele erfüllt sind.

7. Nun nehme dir ein Refactoring von einem Teil der Anwendung vor. Führe dieses Schritt für Schritt durch. Notiere deine Erkenntnisse und Überraschungen, damit wir sie später besprechen können.

8. Je nachdem wie schnell du warst, mach entweder noch ein Refactoring oder nimm dir ein Feature vor. Mögliche Kandidaten: Die Struts-Actions verschlanken, Guice (teilweise) ausbauen, Konfiguration cloud-native über ENV Vars, Authentication via OAuth.
