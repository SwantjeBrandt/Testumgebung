# Testumgebung



## Überblick: Zusammenhänge testen

<!-- class="animate__animated animate__bounceInRight" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Welcher Test passt, wenn ich einen Zusammenhang prüfen will?</i></span>
</div>

<div style="height: 15px;"></div>

--{{0}}--<div style="border-left: 6px solid #2e9e5b; background: rgba(46,158,91,0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
💡 <b>Lehrbuch Hinweis:</b> In diesem Kurs lernst du, <b>welchen Test</b> du für Zusammenhänge brauchst, <b>wie du ihn in JASP durchführst</b> und <b>wie du das Ergebnis liest und berichtest</b>. Das Skalenniveau entscheidet über den Test.
</div>

<div style="height: 15px;"></div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>Nominal</b></div>
<div style="font-size: 0.9em;"><b>Chi-Quadrat-Test</b><br>Hängen zwei Kategorien zusammen?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Bedingung (mit/ohne Musik) und Gehpause (ja/nein).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📶</div>
<div style="text-align: center; font-size: 1.1em;"><b>Ordinal</b></div>
<div style="font-size: 0.9em;"><b>Spearman-Korrelation</b> oder <b>Kendall-Tau</b><br>Gehen höhere Ränge der einen mit höheren Rängen der anderen Variable einher?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #2a9a50; border-radius: 0 8px 8px 0; font-size: 0.85em;">📋 Trainingshäufigkeit (Kategorien) und Borg-Wert.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #eef2fb; border: 2px solid #4e66bd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Metrisch</b></div>
<div style="font-size: 0.9em;"><b>Pearson-Korrelation (<i>r</i>)</b><br>Wie stark ist der lineare Zusammenhang zweier Messwerte?</div>
<div style="margin-top: 10px; padding: 8px 10px; background: #ffffff; border-left: 4px solid #4e66bd; border-radius: 0 8px 8px 0; font-size: 0.85em;">🏃🏾‍♀️ Tempo der Musik (BPM) und Strecke.</div>
</div>

</div>

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Ein Zusammenhang sagt nichts über <b>Ursache und Wirkung</b>. Dafür braucht es ein Experiment (siehe Kapitel Design). Außerdem gilt: Auch ein starker Zusammenhang kann durch eine dritte Variable entstehen (Störvariable).
</div>

<div style="height: 15px;"></div>

{{1}} <section>

#### So gehst du in JASP grundsätzlich vor

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📂</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Daten laden</b></div>
<div style="font-size: 0.9em;">Datei (.csv oder .xlsx) über „Open“ öffnen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Skalenniveau prüfen</b></div>
<div style="font-size: 0.9em;">Spaltensymbol anklicken: nominal, ordinal oder scale einstellen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔍</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Daten ansehen</b></div>
<div style="font-size: 0.9em;">„Descriptives“ ➜ Histogramme und Streudiagramm anfordern.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Test wählen</b></div>
<div style="font-size: 0.9em;">Passende Analyse im Menü wählen, Variablen ins Feld ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Voraussetzungen prüfen</b></div>
<div style="font-size: 0.9em;">Linearität im Streudiagramm, Normalverteilung, Ausreißer.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📖</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Ergebnis lesen</b></div>
<div style="font-size: 0.9em;">Korrelationskoeffizient, <i>p</i>-Wert und Konfidenzintervall ablesen und berichten.</div>
</div>

</div>

<!-- TODO: Screenshot JASP-Oberfläche -->

<div style="border-left: 6px solid #e0a526; background: rgba(224,165,38,0.14); border-radius: 8px; padding: 0.7rem 1.2rem;">
📌 <b>Merke:</b> Ob ein Zusammenhang statistisch signifikant ist, sagt dir der <i>p</i>-Wert. Wie <b>stark</b> er ist, sagt dir der Koeffizient (<i>r</i>, ρ, τ, φ). Berichte immer beides.
</div>

<div style="height: 15px;"></div>

</section>

---

## 🏷️ Chi-Quadrat-Test

<!-- class="animate__animated animate__bounceInRight" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Wann nutze ich den Chi-Quadrat-Test und wie werte ich ihn aus?</i></span>
</div>

<div style="height: 15px;"></div>

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Hängen <b>zwei Kategorien</b> zusammen bzw. unterscheiden sich Häufigkeiten?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Beide Variablen <b>nominal</b> (oder ordinal mit wenigen Stufen).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;">Jede Person zählt in genau <b>einer Zelle</b>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Unabhängige Beobachtungen, erwartete Häufigkeiten in der Regel ≥ 5.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
40 Läufer:innen (20 mit, 20 ohne Musik). Gemessen wird, ob sie den Lauf <b>ohne Gehpause</b> schaffen (ja/nein). Hängt das mit der Musikbedingung zusammen?
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Musikbedingung und Gehpause sind unabhängig voneinander. |
| **H1 (ungerichtet)** | Musikbedingung und Gehpause hängen zusammen. |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Beide Variablen als nominal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Frequencies ➜ Classical ➜ Contingency Tables.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Musikbedingung in „Rows“, Gehpause in „Columns“.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Statistik</b></div>
<div style="font-size: 0.9em;">Unter „Statistics“ <b>χ²</b> und unter „Nominal“ <b>Phi and Cramér’s V</b> anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zellen</b></div>
<div style="font-size: 0.9em;">Unter „Cells“ „Expected counts“ und „Row“-Prozente anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Voraussetzung</b></div>
<div style="font-size: 0.9em;">Erwartete Häufigkeiten ablesen: sind alle ≥ 5?</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Frequencies ➜ Classical ➜ Contingency Tables</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Chi-Quadrat-Test -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Contingency Tables</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Bedingung</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">ohne Gehpause</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">mit Gehpause</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Total</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">mit Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">16</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">4</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">ohne Musik</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">9</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">11</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Total</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">25</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">15</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">40</td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Chi-Squared Tests</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Value</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">df</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">χ²</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">5,23</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">1</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,022</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">N</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">40</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;"></td></tr>
</table>
</div>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Nominal</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;"></th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Value</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Phi-Coefficient</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,36</td></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Cramér’s V</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,36</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,022 ➜ die Variablen hängen signifikant zusammen.</li>
<li><b>Anteile:</b> Mit Musik schaffen 16 von 20 Personen (80 %) den Lauf ohne Gehpause, ohne Musik 9 von 20 (45 %).</li>
<li><b>φ bzw. V:</b> ,36 ➜ mittlerer bis großer Zusammenhang.</li>
<li><b>Erwartete Häufigkeiten:</b> 12,5 bzw. 7,5, alle ≥ 5, die Voraussetzung ist erfüllt.</li>
<li><b>Hinweis:</b> JASP bietet zusätzlich „χ² continuity correction“ (Yates) an. Sie ist bei 2 × 2-Tabellen mit kleinen Häufigkeiten konservativer.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

φ (bei 2 × 2) bzw. Cramér’s V: ab ,1 klein, ab ,3 mittel, ab ,5 groß (Cohen, 1988). Bei größeren Tabellen hängen die Grenzwerte von den Freiheitsgraden ab.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Der Anteil der Personen, die den Lauf ohne Gehpause absolvierten, war mit Musik höher (80 %) als ohne Musik (45 %), χ²(1, N = 40) = 5,23, p = ,022, φ = ,36.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Erwartete Häufigkeiten ≥ 5 | „Expected counts“ in den Zellen | 12,5 und 7,5 ➜ erfüllt | Fisher’s exact test |
| Unabhängige Beobachtungen | Studiendesign | jede Person nur einmal ➜ erfüllt | McNemar-Test (verbundene Daten) |
| Häufigkeiten statt Anteile | Rohdaten | Personenzahlen ➜ erfüllt | Zählwerte verwenden |

</details>

**Frage 1:** Warum prüfst du bei einem Chi-Quadrat-Test die erwarteten Häufigkeiten?

- [( )] Weil sonst der Test keine Teststatistik liefert
- [(X)] Weil bei zu kleinen erwarteten Häufigkeiten das Ergebnis unzuverlässig wird
- [( )] Weil sie die Effektstärke sind
- [( )] Weil sie die Normalverteilung zeigen

<details>
<summary><b>👉 Erklärung</b></summary>

Der Chi-Quadrat-Test ist eine Näherung. Bei erwarteten Häufigkeiten unter 5 nutzt du besser Fisher’s exact test.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring &amp; Bortz (2016); JASP Team (2024)
</div>

</section>

---

## 📏 Pearson-Korrelation

<!-- class="animate__animated animate__bounceInRight" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Wann nutze ich den Pearson-Korrelation und wie werte ich ihn aus?</i></span>
</div>

<div style="height: 15px;"></div>

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Wie stark ist der <b>lineare Zusammenhang</b> zweier Messwerte?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Beide Variablen <b>metrisch</b>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;">Jede Person liefert <b>beide Werte</b>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Linearer Zusammenhang, annähernd normalverteilte Variablen, keine starken Ausreißer.</div>
</div>

</div>

<div style="border: 2px solid #4e66bd; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
🏃🏾‍♀️ <span style="background: linear-gradient(transparent 55%, rgba(71, 69, 173, 0.55) 60%);"><b>Wirkung auf die Ausdauerleistung</b></span> 🏃🏾‍♀️<br>
20 Personen laufen jeweils zu Musik mit einem anderen Tempo (60 bis 180 BPM). Hängt das <b>Tempo der Musik</b> mit der gelaufenen <b>Strecke</b> zusammen?
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Es gibt keinen linearen Zusammenhang zwischen Tempo und Strecke (ρ = 0). |
| **H1 (ungerichtet)** | Es gibt einen linearen Zusammenhang (ρ ≠ 0). |
| **H1 (gerichtet)** | Je höher das Tempo, desto größer die Strecke (ρ &gt; 0). |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Tempo und Strecke jeweils als scale.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Regression ➜ Classical ➜ Correlation.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Tempo und Strecke ins Feld „Variables“ ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Koeffizient</b></div>
<div style="font-size: 0.9em;"><b>Pearson’s r</b> anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Report significance“ und „Confidence intervals“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📈</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Streudiagramm</b></div>
<div style="font-size: 0.9em;">Unter „Plots“ „Scatter plots“ anhaken und die Linearität prüfen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Regression ➜ Classical ➜ Correlation ➜ Pearson’s r</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Pearson-Korrelation -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Pearson Correlations</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">r</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">95 % CI</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Tempo (BPM)</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Strecke (m)</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,60</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,005</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">[,22; ,83]</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Stärke:</b> r = ,60 ➜ starker positiver Zusammenhang.</li>
<li><b>Richtung:</b> Das Vorzeichen zeigt: höheres Tempo geht mit größerer Strecke einher.</li>
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,005 ➜ der Zusammenhang ist signifikant.</li>
<li><b>Konfidenzintervall:</b> [,22; ,83], es enthält die Null nicht.</li>
<li><b>Bestimmtheitsmaß:</b> r² = ,37 ➜ rund 37 % der Streuung der Strecken hängen mit dem Tempo zusammen.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

|<i>r</i>|: ab ,1 klein, ab ,3 mittel, ab ,5 groß (Cohen, 1988).

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Das Tempo der Musik und die gelaufene Strecke hingen positiv zusammen, r(18) = ,60, 95 %-KI [,22; ,83], p = ,005.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Prüfung in JASP | Ergebnis im Beispiel | Bei Verletzung |
| :-- | :-- | :-- | :-- |
| Linearität | Streudiagramm | annähernd linear ➜ erfüllt | Spearman-Korrelation |
| Normalverteilung | Shapiro-Wilk | <i>p</i> = ,426 bzw. ,408 ➜ erfüllt | Spearman-Korrelation |
| Keine starken Ausreißer | Streudiagramm, Boxplot | keine auffälligen Werte ➜ erfüllt | Ausreißer prüfen, ggf. Spearman |

</details>

**Frage 1:** Eine Korrelation von r = ,60 bedeutet, dass …

- [( )] das Tempo die Strecke verursacht
- [(X)] höheres Tempo mit größerer Strecke einhergeht
- [( )] 60 % der Personen weiter laufen
- [( )] es keinen Zusammenhang gibt

<details>
<summary><b>👉 Erklärung</b></summary>

Korrelationen zeigen Zusammenhänge, aber keine Kausalität.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring &amp; Bortz (2016); Eid, Gollwitzer &amp; Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## 📶 Spearman-Korrelation

<!-- class="animate__animated animate__bounceInRight" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Wann nutze ich den Spearman-Korrelation und wie werte ich ihn aus?</i></span>
</div>

<div style="height: 15px;"></div>

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Wie stark hängen zwei <b>Rangordnungen</b> zusammen?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Mindestens <b>ordinale</b> Variablen (oder metrisch ohne Normalverteilung).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;">Jede Person liefert <b>beide Werte</b>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Monotoner Zusammenhang, ordinale Daten.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
20 Personen geben ihre <b>Trainingshäufigkeit</b> (1 = nie bis 5 = täglich) und nach dem Lauf ihren <b>Borg-Wert</b> an. Gehen höhere Trainingshäufigkeiten mit niedrigeren Borg-Werten einher?
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Es gibt keinen monotonen Zusammenhang zwischen Trainingshäufigkeit und Borg-Wert (ρ = 0). |
| **H1 (ungerichtet)** | Es gibt einen monotonen Zusammenhang (ρ ≠ 0). |
| **H1 (gerichtet)** | Je häufiger das Training, desto niedriger der Borg-Wert (ρ &lt; 0). |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Trainingshäufigkeit und Borg-Wert jeweils als ordinal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Regression ➜ Classical ➜ Correlation.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Beide Variablen ins Feld „Variables“ ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Koeffizient</b></div>
<div style="font-size: 0.9em;"><b>Spearman’s rho</b> anhaken, Pearson abwählen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Report significance“ und „Sample size“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📈</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Streudiagramm</b></div>
<div style="font-size: 0.9em;">Scatter plot anfordern, um Monotonie und Bindungen zu sehen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Regression ➜ Classical ➜ Correlation ➜ Spearman’s rho</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Spearman-Korrelation -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Spearman Correlations</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Spearman’s rho</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">n</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Trainingshäufigkeit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg-Wert</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−,57</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,009</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">20</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Stärke und Richtung:</b> ρ = −,57 ➜ mittlerer bis starker <b>negativer</b> Zusammenhang.</li>
<li><b>Deutung:</b> Je häufiger trainiert wird, desto niedriger ist der Borg-Wert, die Anstrengung wird also geringer empfunden.</li>
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,009 ➜ signifikant.</li>
<li><b>Bindungen:</b> Viele Personen haben dieselben Werte (z. B. mehrere mit Trainingsstufe 3). Spearman korrigiert das mit mittleren Rängen.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

|ρ| wird wie <i>r</i> eingeordnet: ab ,1 klein, ab ,3 mittel, ab ,5 groß (Cohen, 1988).

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Je häufiger Personen trainierten, desto niedriger war ihr Borg-Wert, ρ(18) = −,57, p = ,009.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal |
| Monotonie | der Zusammenhang steigt oder fällt durchgängig, muss aber nicht linear sein |
| Viele Bindungen | bei vielen gleichen Werten ist Kendall-Tau oft zuverlässiger |

</details>

**Frage 1:** Wann wählst du Spearman statt Pearson?

- [( )] Wenn beide Variablen nominal sind
- [(X)] Wenn die Variablen ordinal sind oder der Zusammenhang nicht linear ist
- [( )] Wenn du Gruppen vergleichen willst
- [( )] Wenn die Stichprobe sehr groß ist

<details>
<summary><b>👉 Erklärung</b></summary>

Spearman rechnet mit Rängen und braucht nur ordinale Daten.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Cohen (1988); Döring &amp; Bortz (2016); JASP Team (2024)
</div>

</section>

---

## 📶 Kendall-Tau

<!-- class="animate__animated animate__bounceInRight" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Wann nutze ich den Kendall-Tau und wie werte ich ihn aus?</i></span>
</div>

<div style="height: 15px;"></div>

<span style="font-size: 1.1em;"><b>Wann passt der Test?</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🎯</div>
<div style="text-align: center; font-size: 1.1em;"><b>Fragestellung</b></div>
<div style="font-size: 0.9em;">Wie stark hängen zwei Rangordnungen zusammen, besonders bei <b>vielen Bindungen</b>?</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📏</div>
<div style="text-align: center; font-size: 1.1em;"><b>Daten</b></div>
<div style="font-size: 0.9em;">Mindestens <b>ordinale</b> Variablen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">👥</div>
<div style="text-align: center; font-size: 1.1em;"><b>Stichprobe</b></div>
<div style="font-size: 0.9em;">Jede Person liefert <b>beide Werte</b>.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">✅</div>
<div style="text-align: center; font-size: 1.1em;"><b>Voraussetzungen</b></div>
<div style="font-size: 0.9em;">Ordinale Daten, monotoner Zusammenhang.</div>
</div>

</div>

<div style="border: 2px solid #2a9a50; border-radius: 12px; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
📋 <span style="background: linear-gradient(transparent 55%, rgba(66, 162, 61, 0.55) 60%);"><b>Wirkung auf das Anstrengungsempfinden</b></span> 📋<br>
Dieselben Daten wie bei Spearman: Trainingshäufigkeit (1 bis 5) und Borg-Wert von 20 Personen. Kendall-Tau ist besonders geeignet, weil viele gleiche Werte vorkommen.
</div>

<span style="font-size: 1.1em;"><b>Hypothesen</b></span>

| Hypothese | Formulierung im Musikbeispiel |
| :-- | :-- |
| **H0** | Es gibt keinen monotonen Zusammenhang (τ = 0). |
| **H1 (ungerichtet)** | Es gibt einen monotonen Zusammenhang (τ ≠ 0). |
| **H1 (gerichtet)** | Je häufiger das Training, desto niedriger der Borg-Wert (τ &lt; 0). |

{{1}} <section>

<span style="font-size: 1.1em;"><b>Durchführung in JASP</b></span>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 20px 0;">

<!-- class="animate__animated animate__fadeInUp" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🏷️</div>
<div style="text-align: center; font-size: 1.1em;"><b>1. Variablen einstellen</b></div>
<div style="font-size: 0.9em;">Beide Variablen als ordinal.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-1s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🧪</div>
<div style="text-align: center; font-size: 1.1em;"><b>2. Analyse öffnen</b></div>
<div style="font-size: 0.9em;">Regression ➜ Classical ➜ Correlation.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-2s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">🔗</div>
<div style="text-align: center; font-size: 1.1em;"><b>3. Variablen zuweisen</b></div>
<div style="font-size: 0.9em;">Beide Variablen ins Feld „Variables“ ziehen.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-3s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">☑️</div>
<div style="text-align: center; font-size: 1.1em;"><b>4. Koeffizient</b></div>
<div style="font-size: 0.9em;"><b>Kendall’s tau-b</b> anhaken (korrigiert für Bindungen).</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">➕</div>
<div style="text-align: center; font-size: 1.1em;"><b>5. Zusatzangaben</b></div>
<div style="font-size: 0.9em;">„Report significance“ anhaken.</div>
</div>

<!-- class="animate__animated animate__fadeInUp animate__delay-4s" -->
<div style="background: #f6f1fa; border: 2px solid #a74ebd; border-radius: 12px; padding: 15px; color: #1f2933;">
<div style="font-size: 2em; text-align: center;">📈</div>
<div style="text-align: center; font-size: 1.1em;"><b>6. Vergleich</b></div>
<div style="font-size: 0.9em;">Spearman und Kendall gleichzeitig anhaken, um beide Werte zu vergleichen.</div>
</div>

</div>

<div style="margin-top: 10px; padding: 8px 10px; background: #1f2933; color: #ffffff; border-radius: 8px; font-size: 0.8em;">🖥️ <b>JASP:</b> Regression ➜ Classical ➜ Correlation ➜ Kendall’s tau-b</div>
<div style="height: 10px;"></div>

<!-- TODO: Screenshot JASP: Kendall-Tau -->

</section>

{{2}} <section>

<span style="font-size: 1.1em;"><b>Ergebnis lesen</b></span>

<div style="overflow-x: auto; background: #ffffff; border: 1px solid #cbd5e1; border-radius: 8px; padding: 10px; margin: 10px 0; color: #1f2933; font-size: 0.85em;">
<div style="font-weight: bold; margin-bottom: 6px;">Kendall’s tau Correlations</div>
<table style="border-collapse: collapse; width: 100%; font-variant-numeric: tabular-nums;">
<tr><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 1</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Variable 2</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">Kendall’s tau B</th><th style="padding: 6px 10px; text-align: right; border-bottom: 2px solid #94a3b8;">p</th></tr>
<tr><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Trainingshäufigkeit</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">Borg-Wert</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">−,47</td><td style="padding: 6px 10px; text-align: right; border-bottom: 1px solid #e2e8f0;">,009</td></tr>
</table>
</div>

<div style="font-size: 0.8em; opacity: 0.7; margin-bottom: 10px;">Fiktive Daten, nachgebaut im Stil der JASP-Ausgabe.</div>

<ul style="font-size: 0.95em;">
<li><b>Stärke und Richtung:</b> τ<sub>b</sub> = −,47 ➜ negativer Zusammenhang.</li>
<li><b>Vergleich mit Spearman:</b> τ ist betragsmäßig kleiner als ρ (−,47 gegenüber −,57). Das ist normal, die Werte sind nicht direkt vergleichbar.</li>
<li><b><i>p</i>-Wert:</b> <i>p</i> = ,009 ➜ signifikant.</li>
<li><b>τb:</b> Das „b“ steht für die Variante, die Bindungen berücksichtigt.</li>
</ul>

<span style="font-size: 1.1em;"><b>Effektstärke einordnen</b></span>

Für τ gibt es keine einheitlichen Grenzwerte. Als grobe Orientierung wird oft wie bei <i>r</i> eingeordnet, τ fällt aber bei gleichem Zusammenhang kleiner aus als ρ.

</section>

{{3}} <section>

<span style="font-size: 1.1em;"><b>So berichtest du das Ergebnis</b></span>

<div style="border-left: 6px solid #a74ebd; background: #f6f1fa; border-radius: 0 12px 12px 0; padding: 0.8rem 1.3rem; margin: 10px 0; color: #1f2933;">
✍️ <b>Musterbericht (APA):</b><br>
<i>Trainingshäufigkeit und Borg-Wert hingen negativ zusammen, τ<sub>b</sub> = −,47, p = ,009.</i>
</div>

<details>
<summary><b>👉 Voraussetzungen prüfen und was du bei Verletzung tust</b></summary>

| Voraussetzung | Hinweis |
| :-- | :-- |
| Skalenniveau | mindestens ordinal |
| Monotonie | der Zusammenhang steigt oder fällt durchgängig |
| Stichprobengröße | auch bei kleinen Stichproben geeignet |

</details>

**Frage 1:** Wann ist Kendall-Tau eine gute Wahl?

- [( )] Bei nominalen Daten
- [(X)] Bei ordinalen Daten mit vielen gleichen Werten
- [( )] Bei Gruppenvergleichen
- [( )] Bei normalverteilten Daten

<details>
<summary><b>👉 Erklärung</b></summary>

Kendall-Tau-b korrigiert Bindungen und eignet sich besonders bei kurzen Skalen mit vielen gleichen Werten.

</details>

<div style="text-align: right; font-size: 0.85em; opacity: 0.8;">
📚 Döring &amp; Bortz (2016); Eid, Gollwitzer &amp; Schmitt (2017); JASP Team (2024)
</div>

</section>

---

## Check-Up: Zusammenhänge testen

<!-- class="animate__animated animate__fadeIn" -->
<div style="border-left: 6px solid #a74ebd; background: rgba(185, 145, 215, 0.12); border-radius: 8px; padding: 0.7rem 1.2rem;">
<span style="font-size: 1.3em;"><i>Welcher Test passt zu welcher Situation? Teste dein Wissen.</i></span>
</div>

<div style="height: 15px;"></div>

**Frage 1:** Du willst prüfen, ob Bedingung (mit/ohne Musik) und Gehpause (ja/nein) zusammenhängen. Beide Variablen sind nominal. Welcher Test passt?

- [( )] Pearson-Korrelation
- [( )] t-Test
- [(X)] Chi-Quadrat-Test
- [( )] ANOVA

[[?]] Beide Variablen sind Kategorien.

<details>
<summary><b>👉 Erklärung</b></summary>

Zwei nominale Variablen ➜ Chi-Quadrat-Test.

</details>

**Frage 2:** Tempo der Musik (BPM) und Strecke (m) sind beide metrisch und annähernd normalverteilt. Welcher Test passt?

- [( )] Chi-Quadrat-Test
- [(X)] Pearson-Korrelation
- [( )] Kruskal-Wallis-Test
- [( )] Mann-Whitney-U-Test

<details>
<summary><b>👉 Erklärung</b></summary>

Zusammenhang zweier metrischer Variablen ➜ Pearson-Korrelation.

</details>

**Frage 3:** Trainingshäufigkeit (Stufen 1 bis 5) und Borg-Wert sind ordinal. Welche Tests passen?

- [( )] Pearson-Korrelation
- [(X)] Spearman-Korrelation oder Kendall-Tau
- [( )] t-Test
- [( )] Chi-Quadrat-Test

<details>
<summary><b>👉 Erklärung</b></summary>

Ordinale Variablen ➜ Spearman oder Kendall.

</details>

**Frage 4:** Welche Aussage über Korrelationen ist richtig?

- [( )] Eine hohe Korrelation beweist Ursache und Wirkung
- [(X)] Ein Zusammenhang kann auch durch eine dritte Variable entstehen
- [( )] Korrelationen gibt es nur bei metrischen Daten
- [( )] Das Vorzeichen zeigt die Stärke

<details>
<summary><b>👉 Erklärung</b></summary>

Korrelation ist nicht Kausalität. Das Vorzeichen zeigt die Richtung, der Betrag die Stärke.

</details>

**Frage 5:** Eine Korrelation von r = −,45 bedeutet …

- [(X)] einen mittleren negativen Zusammenhang
- [( )] keinen Zusammenhang
- [( )] einen starken positiven Zusammenhang
- [( )] einen Fehler in den Daten

<details>
<summary><b>👉 Erklärung</b></summary>

Das Minus zeigt die Richtung (gegenläufig), der Betrag ,45 einen mittleren Zusammenhang.

</details>

---

## Literatur

* Cohen, J. (1988). <i>Statistical power analysis for the behavioral sciences</i> (2nd ed.). Lawrence Erlbaum.
* Döring, N. &amp; Bortz, J. (2016). <i>Forschungsmethoden und Evaluation in den Sozial- und Humanwissenschaften</i> (5. Aufl.). Springer.
* Eid, M., Gollwitzer, M. &amp; Schmitt, M. (2017). <i>Statistik und Forschungsmethoden</i> (5. Aufl.). Beltz.
* JASP Team (2024). <i>JASP</i> (Version 0.19) [Computer software]. https://jasp-stats.org/
* Tomczak, M. &amp; Tomczak, E. (2014). The need to report effect size estimates revisited. <i>Trends in Sport Sciences, 21</i>(1), 19–25.
