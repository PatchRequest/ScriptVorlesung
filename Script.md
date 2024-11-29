Vorläufiger Entwurf des Skripts zur Vorlesung

Achtung: Dieser Entwurf befindet sich noch in Bearbeitung!

Dieses Dokument ist der aktuelle Ansatz für das Vorlesungsskript, aber es ist noch stark in Arbeit. Es handelt sich um eine stark gekürzte Version und enthält noch nicht alle Informationen. Einige Teile wurden mithilfe von LLMs aus Video-Transkripten generiert, daher könnten auch Fehler enthalten sein.

Das Skript wird aktiv weiterentwickelt. Falls dir Fehler oder Verbesserungsmöglichkeiten auffallen oder dir wichtige Inhalte fehlen, würde ich mich sehr über deinen Beitrag freuen – gerne per Pull Request.



# Table of Contents

1. Rahmbedingungen
   - 1.1 Relevante Paragraphen und rechtliche Grundlagen
   - 1.2 Ablauf und Herausforderungen bei Responsible Disclosure
   - 1.4 Verhaltenstipps, Lernressourcen, Zertifizierungen und Knowledge-Base
2. OSINT (Open Source Intelligence)
   - 2.1 Definition und Anwendungsbereiche
   - 2.2 Datenquellen und Datenpunkte
   - 2.3 Verknüpfung und Analyse von Datenpunkten
   - 2.4 Aufbau von Informationsnetzwerken und Communities
3. Active Directory
   - 3.1 Aufbau und Komponenten (Kerberos, LDAP, DNS, SMB)
   - 3.2 Domain Controller, Domänenobjekte
   - 3.3 Authentifizierungsprozesse (NTLM, Kerberos)
   - 3.4 Angriffe: Enumeration, Pass-the-Hash, Credential Dumping, etc.
4. Web-Sicherheit
   - 4.1 Aufbau von Web-Apps und HTTP
   - 4.2 Beispielhafte Angriffe: XSS, SQL-Injection, CSRF, etc.
5. Cybercrime
   - 5.1 Täterprofile und Motivationen
   - 5.2 Struktur von Cybercrime-Netzwerken



# 1. Rahmbedingungen
## 1.1 Relevante Paragraphen und rechtliche Grundlagen
### §202a: Ausspähen von Daten (Absatz a und b)

Absatz 1 besagt, dass unbefugtes Verschaffen von Zugang zu geschützten Daten mit Freiheitsstrafe bis zu 3 Jahren oder mit Geldstrafe bestraft wird. Wichtig ist hier das Wort "unbefugt", das die Intention des Handelnden berücksichtigt. Die Überwindung von Zugangssicherungen, auch wenn diese ineffektiv sind, ist ebenfalls strafbar. Absatz 2 stellt klar, dass nur elektronisch oder magnetisch gespeicherte oder übermittelte Daten betroffen sind.

### §202b: Abfangen von Daten (Absatz a und b)

Dieser Paragraf bestraft das unbefugte Erlangen von Daten aus nicht-öffentlichen Übermittlungen oder elektromagnetischer Strahlung mit Freiheitsstrafe bis zu 2 Jahren oder Geldstrafe. Der Einsatz technischer Mittel, um an nicht für einen bestimmte Daten zu gelangen, ist strafbar. Dies gilt auch für das Abhören von drahtlosen und drahtgebundenen Übertragungen.

### §202c: Vorbereitung des Ausspähens und Abfangens von Daten (Fortsetzung)

Hacking-Tools können darunter fallen, wenn sie explizit für das unbefugte Eindringen oder Abfangen von Daten verwendet werden sollen. Die Verwendung von Tools zu Testzwecken, wie etwa bei einem legitimen Pentest mit vorheriger Zustimmung des Eigentümer der Systeme, fällt normalerweise nicht unter diesen Paragrafen, da hier keine Straftat beabsichtigt ist. Eine wichtige Abgrenzung besteht also darin, ob das Werkzeug zu legalen Zwecken eingesetzt wird oder eine böswillige Absicht dahintersteht.

### §303a: Datenveränderung (Absatz a und b)

Das unbefugte Löschen, Unterdrücken, Verändern oder Unbrauchbarmachen von Daten wird mit Freiheitsstrafe bis zu 2 Jahren oder mit Geldstrafe bestraft. Eine Ausnahme bildet hier der Fall, wenn der Betroffene die ausdrückliche Erlaubnis des Dateneigentümer hat, beispielsweise im Rahmen eines geplanten Stresstests.

### §303b: Computersabotage (Absatz a und b)

Absatz 1 definiert Computersabotage als Eingriffe in Datenverarbeitungsvorgänge, die den Betrieb eines Unternehmens oder einer Behörde stören. Dies umfasst auch den Angriff auf IT-Systeme, die zum Beispiel in Krankenhäusern, Kraftwerken oder anderen kritischen Infrastrukturen verwendet werden. Strafen reichen hier bis zu 5 Jahren Freiheitsentzug, was die Schwere von Angriffen auf kritische Systeme betont.

### §206: Verletzung des Fernmeldegeheimnisses

Das Abhören und das Zugänglichmachen von Inhalten einer nicht öffentlichen Telekommunikation an Dritte ist strafbar. Ein Penetrationstester, der in Kommunikationssysteme eindringt, könnte sich schnell strafbar machen, wenn er keine explizite Zustimmung von den Kommunikationsparteien hat. Auch der Zugriff auf Metadaten fällt unter das Fernmeldegeheimnis.

### Fazit zur Rechtslage im Pentesting

Der rechtliche Rahmen macht klar, dass Pentests ohne klare und schriftliche Zustimmung des Eigentümer oder Betreibers der IT-Infrastruktur strafrechtlich verfolgt werden können. Ein umfassender Vertrag und die Zustimmung aller Beteiligten sind entscheidend, um die Legalität der Aktivitäten zu gewährleisten. Der Unterschied zwischen einem ethischen Hacker und einem Cyberkriminellen ist hier im Wesentlichen der rechtliche Rahmen und die Einwilligung.

## 1.2 Ablauf und Herausforderungen bei Responsible Disclosure


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

## 1.3 Verhaltenstipps, Lernressourcen, Zertifizierung und Knowledgebase

### Verhaltenstipps
Als Security Researcher ist es entscheidend, immer vorsichtig und verantwortungsvoll vorzugehen. Obwohl die Neugier ein starker Antrieb ist, sollte man sich bewusst sein, dass gefundene Schwachstellen im Internet reale Auswirkungen haben können. Ein Beispiel dafür ereignete sich auf der DEFCON, als Bluetooth-Spam-Angriffe mit einem Flipper Zero dazu führten, dass eine Insulinpumpe abstürzte – eine Situation, die ernsthafte gesundheitliche Risiken verursachen kann. Es ist daher von großer Bedeutung, Zurückhaltung zu zeigen, um unbeabsichtigte Schäden zu vermeiden.

### Lernressourcen
Die kontinuierliche Weiterbildung ist essenziell für die Entwicklung von Fähigkeiten als Security Researcher. Hier sind einige empfohlene Ressourcen:

- **Websites zum Übung von Angriffen**:
  - **HackTheBox**: Ermöglicht das Training von realistischen Angriffsszenarien in isolierten Umgebungen.
  - **TryHackMe**: Ideal für Einsteiger bis Fortgeschrittene mit interaktiven Tutorials.
  - **VulnHub**: Bietet kostenlose VMs zum Download, um Schwachstellen in einem eigenen Lab zu üben.
  - **BurpSuite Academy**: Ein hervorragender Ort, um Web-Exploitation zu lernen.

- **Einrichtung eines eigenen Labs**: Um praktische Übungen durchzuführen, empfiehlt es sich, ein eigenes Lab einzurichten. Dies ermöglicht, verschiedene Tools auszuprobieren und sich in einer sicheren Umgebung mit Schwachstellen zu befassen.

- **Nützliche YouTube-Kanäle**: Diese Kanäle bieten exzellente Lerninhalte, die praxisorientierte Techniken vermitteln:
  - **John Hammond**
  - **LiveOverflow**
  - **IppSec**
  - **NahamSec**
  - **HackerSploit**

### Zertifizierungen
Zertifizierungen sind wichtig, um potenziellen Arbeitgebern oder Kunden die eigenen Kompetenzen nachzuweisen. Zu den bekanntesten Zertifikaten gehören:

- **OSCP** (Offensive Security Certified Professional): Gilt als der Goldstandard unter den Zertifikaten im Bereich Penetration Testing.
- **CEH** (Certified Ethical Hacker): Ein weiteres populäres Zertifikat, das Grundlagen abdeckt.
- **CRTP** (Certified Red Team Professional): Eine ausgezeichnete Zertifizierung für Red Teaming und Active Directory Angriffe.

Weitere Informationen zu Zertifizierungen und eine Roadmap, die einen Überblick über den Zertifizierungsweg gibt, sind [hier online verfügbar](https://pauljerimy.com/security-certification-roadmap/).

### Knowledgebase
Eine gut strukturierte Knowledgebase ist ein wertvolles Werkzeug für jeden Security Researcher. Sie ermöglicht es, erprobte Techniken, Angriffe und exakte Kommandos zentral zu speichern, sodass man im Ernstfall sofort auf relevante Informationen zugreifen kann, ohne erst langwierige Internetrecherchen durchführen zu müssen. Dies erhöht die Effizienz und reduziert Fehler in kritischen Situationen.


# 2. OSINT

### Was ist OSINT?

Open-Source Intelligence (OSINT) ist das Sammeln und Analysieren von Daten aus öffentlich zugänglichen Quellen, auch verdeckte Quellen und öffentlich verfügbare Informationen (PAI), um verwertbare Erkenntnisse zu gewinnen. OSINT umfasst verschiedene Techniken und Methoden, um aus einer Vielzahl von Datenquellen die relevanten Informationen herauszufiltern und zu verarbeiten.

Im Wesentlichen werden öffentlich zugängliche Daten gesammelt und in verwertbare Informationen umgewandelt, die z. B. für Sicherheitszwecke, Marktanalysen oder zur Profilbildung genutzt werden können. Diese Informationen sind oft verstreut, müssen jedoch durch systematische Analyse zusammengeführt werden, um umfassende und nutzbare Erkenntnisse zu gewinnen.

### Von Daten zu Wissen

OSINT sammelt Datenpunkte, verknüpft sie und schafft daraus verwertbare Erkenntnisse ("actionable knowledge"). Ein gutes Beispiel sind Verknüpfungen von Freundschaften – das sind oft nicht gewollte, aber öffentlich zugängliche Informationen. Wenn wir genug Datenpunkte sammeln, können wir mit hoher Wahrscheinlichkeit auf die sozialen Beziehungen, den Lebensstil und die Interessen einer Person schließen.

Ein umfassendes Wissen über eine Person oder ein Ziel kann dann genutzt werden, um Entscheidungen zu beeinflussen, wie etwa die Planung einer Marketingstrategie, die Strafverfolgung oder sogar die Vorbereitung eines gezielten Angriffs.

### Grundlagen von Datenpunkten

Ein **Datenpunkt** ist eine einzelne Information, die für sich steht, beispielsweise ein Name, eine E-Mail-Adresse oder ein Standort. Diese Datenpunkte können über verschiedene Quellen abgeglichen werden, um mehr über eine Person zu erfahren. Einzelne Datenpunkte können wie Puzzleteile wirken, die kombiniert ein klares Bild ergeben.

Datenpunkte können sichtbar sein (wie ein Profilbild) oder versteckt (wie Metadaten in Bildern). Versteckte Datenpunkte wie Metadaten sind oft unbewusst veröffentlicht und können wertvolle Hinweise liefern. Es ist wichtig, Datenpunkte nicht isoliert zu betrachten, sondern sie zu verknüpfen, um neue Erkenntnisse zu gewinnen.

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

Das Kerberos-Protokoll arbeitet Ticket-basiert und verwendet drei Entitäten:

1. **AS-REQ (Authentication Service Request)**: Der Benutzer sendet eine Anfrage an den KDC, die seinen Benutzernamen und einen verschlüsselten Authenticator enthält.
2. **AS-REP (Authentication Service Response)**: Der KDC sendet dem Benutzer ein Ticket-Granting Ticket (TGT) zurück, das einen Session Key enthält.
3. **TGS-REQ (Ticket-Granting Service Request)**: Der Benutzer sendet das TGT, um auf einen bestimmten Service zuzugreifen.
4. **TGS-REP (Ticket-Granting Service Response)**: Der KDC erstellt ein Service Ticket (TGS) und sendet es an den Benutzer.
5. **AP-REQ (Application Request)**: Der Benutzer sendet das TGS an den Service.
6. **AP-REP (Application Response)**: Der Service gewährt dem Benutzer Zugriff.

Dieses Verfahren stellt sicher, dass die Anmeldeinformationen des Benutzers nicht im Netzwerk übertragen werden und somit vor Abhörangriffen geschützt sind.

## Angriffe auf Active Directory

Obwohl Active Directory ein robustes System ist, gibt es verschiedene Angriffsvektoren, die von Angreifern ausgenutzt werden können. Diese reichen von **Kerberoasting** über **Golden und Silver Tickets** bis hin zu **Pass-the-Hash-Angriffen**. Es ist wichtig, zwischen **Abuses** und **Exploits** zu unterscheiden:

- **Abuses**: Nutzung bestehender Funktionen für schädliche Zwecke.
- **Exploits**: Ausnutzen von Sicherheitslücken, die durch Patches behoben werden können.

Exploits können durch Patches behoben werden, Abuses erfordern jedoch oft komplexere Maßnahmen, da sie die Funktionalität des Systems selbst betreffen.

## Zwischen Fazit

Im Alltag dient Active Directory zur Authentifizierung von Benutzern und Admins gegenüber Objekten, Systemen und der Domäne selbst. Dies geschieht über die Protokolle **Kerberos** und **NTLM**. DNS-Anfragen werden über Active Directory abgewickelt, um die richtigen Systeme zu finden und Load Balancing zu ermöglichen. Das Directory dient auch zur zentralen Speicherung und zum Abruf von Informationen. Die Konfiguration des gesamten Systems erfolgt zentral und kann durch **GPOs** automatisiert und an einzelne Gruppen oder Benutzer angepasst werden.

# Angriffsszenario gegen Active Directory

In diesem Abschnitt der Vorlesung werden beispielhafte Angriffe gegen Active Directory dargestellt, die als eine potenzielle Kill Chain beschrieben werden. Die Reihenfolge der Schritte kann dabei variieren oder wiederholt werden. Die vorgestellten Angriffe sind nur ein kleiner Ausschnitt aus dem breiten Spektrum an möglichen Angriffen.

## 1. Lokale Privilegieneskalation
Der erste Schritt einer solchen Kill Chain ist oft die lokale Privilegieneskalation, um lokale Administratorrechte zu erlangen. Dies kann auf verschiedene Weise erfolgen, wobei Tools wie **WinPEAS** zur automatisierten Prüfung genutzt werden. Zwei wichtige Methoden sind:

- **Unquoted Service Paths**: Bei einigen Diensten kann der Pfad zur ausführbaren Datei Leerzeichen enthalten. Durch die Art, wie Windows die Suchreihenfolge bei der Pfadangabe handhabt, kann der Angreifer eine eigene Datei erstellen, die anstelle der eigentlichen Datei vom Dienst ausgeführt wird. Dieser Dienst läuft typischerweise mit hohen Rechten.

- **Modifiable Service Files**: Hierbei wird die Datei, die von einem Dienst ausgeführt wird, durch eine manipulierte Version ersetzt, die dem Angreifer Administratorrechte oder eine Shell mit höheren Rechten verschafft.

## 2. Netzwerkaufklärung (Enumeration)
Nach der lokalen Privilegieneskalation erfolgt die Netzwerkaufklärung. Ein allgemeiner Scan, z.B. mit **nmap**, dient dazu, vorhandene Dienste und Geräte im Netzwerk zu identifizieren. Weitere Informationen über das Active Directory, wie z.B. den Domänencontroller, Child Domains oder andere Dienste, können ebenfalls gesammelt werden.

Zusätzlich kann eine **Interaktion über SMB** erfolgen. Da Active Directory oft mit SMB arbeitet, können hier Informationen über Geräte und Domänen gesammelt werden. Mit **enum4linux** lassen sich neben Benutzerlisten auch Gruppen und Passwortrichtlinien ermitteln.

Falls anonyme Abfragen nicht möglich sind, kann **Brute-Forcing** verwendet werden, um valide Benutzernamen zu identifizieren. Oftmals ermöglichen schlecht konfigurierte Shares eine anonyme Auflistung von Dateien, die sensible Informationen enthalten können.

## 3. AS-REP Roasting
Beim **AS-REP Roasting** wird ein Ticket Granting Ticket (TGT) ohne vorherige Authentifizierung angefordert, was aus Kompatibilitätsgründen von Microsoft ermöglicht wurde. Der verschlüsselte Session Key im TGT kann mit Tools wie **Hashcat** geknackt werden, um das Benutzerpasswort herauszufinden.

## 4. Password Spraying
**Password Spraying** ist besonders effektiv gegen Active Directory, da normale Benutzerkonten oft schwache Passwörter verwenden. Hierbei wird ein Passwort für alle Benutzer getestet, wodurch die Lockout-Mechanismen umgangen werden. Häufig wird die Kombination **Passwort = Benutzername** verwendet, oder typische Passwörter wie "Sommer25!" oder "Welcome1!".

## 5. Bloodhound
Bei großen Active Directory-Instanzen bietet sich **Bloodhound** an, um die vielen Informationen aus der Enumeration effizient zu verarbeiten. Mit dem Tool **SharpHound** werden Daten gesammelt, die dann in **Bloodhound** importiert und visualisiert werden. So lassen sich Angriffswege im Active Directory identifizieren.

- **Datensammlung durch SharpHound**:
  - Direkt vom Domänencontroller: Informationen über Gruppen, Trusts und Benutzer werden abgefragt.
  - Von einzelnen PCs: Hierbei werden Informationen zu lokalen Administrationsrechten und Anmeldungen gesammelt.

## 6. Kerberoasting
Verfügt der Angreifer über ein gültiges Benutzerkonto, kann **Kerberoasting** durchgeführt werden. Hierbei wird ein Ticket Granting Service (TGS) angefordert, das mit dem Passwort des Dienstes verschlüsselt ist. Der Angriff erfolgt offline und bleibt oft unbemerkt.

## 7. Enumeration von Shares mit Credentials
Nachdem Zugangsdaten erlangt wurden, sollten **Shares erneut** auf Zugriffsrechte und sensible Dateien untersucht werden, da diese wertvolle Informationen enthalten können.

## 8. Broadcast Poisoning
**Broadcast Poisoning** nutzt aus, dass Windows-Geräte verschiedene Broadcasts senden, z.B. zur Namensauflösung über den **NetBIOS Name Service (NBT-NS)**. Der Angreifer kann diese Broadcasts abfangen und mit gefälschten Antworten reagieren, um **NTLM-Anmeldeinformationen** zu erlangen.

## 9. NTLM Relaying
Wenn **SMB Signing** deaktiviert ist, können Anfragen abgefangen und an andere Server weitergeleitet werden. Der Angreifer agiert als Vermittler und baut im Namen des Clients eine Session auf.

## 10. Credential Dumping
Mit **Credential Dumping** werden Keys und Tickets, die auf einem PC gespeichert sind, extrahiert. Tools wie **Mimikatz** oder **LaZagne** können dazu verwendet werden. Auch ohne lokale Administratorrechte können gespeicherte Passwörter, z.B. aus **Chrome**, mit Tools wie **DonPapi** extrahiert werden.

Credential Dumping kann mit **NTLM Relaying** kombiniert werden, um automatisiert Credentials von verschiedenen Systemen zu erhalten, was zu einem Totalausfall des Active Directory führen kann.

## 11. DC Sync
**DC Sync** ist eine Technik, bei der ein Angreifer die Funktionalität der Active Directory-Replikation ausnutzt, um Anmeldeinformationen direkt von einem Domain Controller zu extrahieren. Ein Angreifer, der über ausreichende Rechte (z.B. replizierende Directory-Änderungen) verfügt, kann die Datenbank des Domain Controllers nachbilden, einschließlich aller Passwort-Hashes. Tools wie **Mimikatz** ermöglichen es, diese Informationen abzufragen und somit Zugang zu hochprivilegierten Accounts, einschließlich des Domain Admins, zu erhalten. Dies macht DC Sync zu einem äußerst gefährlichen Angriff, der das gesamte Netzwerk kompromittieren kann.

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
- **Job-Queue**: Stellt Aufgaben für die Job-Server bereit.
- **Full-Text-Search-Service**: Ermöglicht die Suche nach Inhalten.
- **Cloud Storage**: Speichert Daten langfristig.
- **CDN (Content Delivery Network)**: Liefert statische Inhalte schnell aus.
- **Data Warehouse**: Speichert große Datenmengen für Analysen.

Diese vielschichtige Architektur bietet zahlreiche Angriffspunkte für das Pentesting.

## Häufige Angriffsarten
Sobald wir die Möglichkeit haben, Systeme zu steuern und eigene Eingaben zu machen, ergeben sich potenzielle Angriffsvektoren. Hier sind einige der häufigsten Schwachstellen:

### Cross-Site Scripting (XSS)
Einschleusen von JavaScript-Code in die Webseite eines anderen Benutzers. Es gibt drei Arten von XSS:

1. **Stored XSS**: Der Code wird persistent in einer Datenbank gespeichert.
2. **Reflected XSS**: Der Code wird nicht persistent gespeichert, sondern als Parameter in der URL übergeben.
3. **DOM-based XSS**: Der Code wird durch Manipulation des DOM-Baums eingeschleust.

### SQL Injection (SQLI)
Manipulation von SQL-Queries, um die Datenbank anzugreifen. Es gibt drei Arten von SQLI:

1. **In-Band SQLI**: Der Output der manipulierten Query wird direkt angezeigt.
2. **Inferential SQLI**: Der Output wird nicht direkt angezeigt, sondern durch Timing- und boolesche Logik ermittelt.
3. **Out-of-Band SQLI**: Der Output wird an eine externe Ressource gesendet.

### Command Injection
Manipulation von Daten, um Systembefehle auszuführen.

### Insecure Direct Object Reference (IDOR)
Direkter Zugriff auf Ressourcen anderer Benutzer durch Manipulation von IDs.

### Cross-Site Request Forgery (CSRF)
Ausnutzen der Tatsache, dass Browser Cookies für das Ziel und nicht für die Quelle einer Anfrage verwenden.

### HTTP Request Smuggling
Manipulation von HTTP-Anfragen, um Daten in die Anfragen anderer Benutzer einzuschleusen.

### Clickjacking
Einbetten der angegriffenen Seite in einen unsichtbaren `iframe`, um den Benutzer zum Klicken auf versteckte Elemente zu verleiten.

