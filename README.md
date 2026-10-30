# Lucerne: law history in git

The law of the canton of Lucerne (Kanton Luzern, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-lu/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

466 acts with 1352 versions so far: the cantonal constitution, the cantonal laws (Gesetze) in force and 344 Verordnungen and Reglemente in force, in the order of the systematic collection, added in parts. Other decrees and decisions, intercantonal agreements and repealed acts are not included yet.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `1-kv/` | Verfassung des Kantons Luzern (SRL Nr. 1) | 1 | one version (the oldest available), 1 July 2014 |
| `2-kbug/` | Kantonales Bürgerrechtsgesetz (SRL Nr. 2) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2018 |
| `5-ng/` | Gesetz über die Niederlassung und den Aufenthalt (SRL Nr. 5) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 September 2021 |
| `7/` | Einführungsgesetz zum Bundesgesetz über die Ausländerinnen und Ausländer (SRL Nr. 7) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2020 |
| `10-strg/` | Stimmrechtsgesetz (SRL Nr. 10) | 7 | oldest version available, then each consolidated version: 1 September 2015 to 1 September 2026 |
| `20-organisationsgesetz-og/` | Gesetz über die Organisation von Regierung und Verwaltung (SRL Nr. 20) | 6 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2026 |
| `21/` | Gesetz über Konflikte zwischen den administrativen und richterlichen Behörden (SRL Nr. 21) | 1 | one version (the oldest available), 1 June 2013 |
| `23-hg/` | Haftungsgesetz (SRL Nr. 23) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `24/` | Gesetz über die Förderung der Gleichstellung von Frau und Mann (SRL Nr. 24) | 1 | as enacted, 1 July 2007 |
| `25-registergesetz/` | Gesetz über die Harmonisierung amtlicher Register (SRL Nr. 25) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2021 |
| `25b-owg/` | Gesetz über die Datendrehscheibe und das Informationssystem Objektwesen (SRL Nr. 25b) | 1 | as enacted, 1 January 2026 |
| `26/` | Informatikgesetz (SRL Nr. 26) | 2 | oldest version available, then each consolidated version: 1 August 2013 to 1 September 2021 |
| `27-publikationsgesetz/` | Gesetz über die amtlichen Veröffentlichungen (SRL Nr. 27) | 1 | one version (the oldest available), 1 July 2015 |
| `28a/` | Statistikgesetz (SRL Nr. 28a) | 2 | oldest version available, then each consolidated version: 1 August 2009 to 1 September 2021 |
| `29-geoinformationsgesetz-gig/` | Gesetz über die Geoinformation und die amtliche Vermessung (SRL Nr. 29) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 September 2021 |
| `30-kantonsratsgesetz-krg/` | Gesetz über die Organisation und Geschäftsführung des Kantonsrates (SRL Nr. 30) | 3 | oldest version available, then each consolidated version: 1 June 2015 to 1 June 2023 |
| `38-kantonales-datenschutzgesetz-kdsg/` | Kantonales Gesetz über den Schutz von Personendaten (SRL Nr. 38) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 June 2025 |
| `39/` | Gesetz über die Videoüberwachung (SRL Nr. 39) | 3 | as enacted, then each consolidated version: 1 January 2012 to 1 September 2021 |
| `40-vrg/` | Gesetz über die Verwaltungsrechtspflege (SRL Nr. 40) | 4 | oldest version available, then each consolidated version: 1 September 2015 to 1 September 2021 |
| `50-behordengesetz-behg/` | Gesetz über die Rechtsstellung der obersten Verwaltungs- und Gerichtsbehörden (SRL Nr. 50) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 June 2023 |
| `51-personalgesetz-pg/` | Gesetz über das öffentlich-rechtliche Arbeitsverhältnis (SRL Nr. 51) | 8 | oldest version available, then each consolidated version: 1 July 2015 to 1 January 2026 |
| `150-gg/` | Gemeindegesetz (SRL Nr. 150) | 5 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `160-fhgg/` | Gesetz über den Finanzhaushalt der Gemeinden (SRL Nr. 160) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 March 2023 |
| `170/` | Gesetz über die Korporationen (SRL Nr. 170) | 3 | as enacted, then each consolidated version: 1 July 2014 to 1 March 2023 |
| `177a/` | Gesetz über die Vereinigung der Korporationsgemeinden Wetzwil/Schlierbach (SRL Nr. 177a) | 1 | one version (the oldest available), 1 August 2008 |
| `178/` | Gesetz über die Aufhebung der Realkorporationsgemeinde Mauensee (SRL Nr. 178) | 1 | one version (the oldest available), 1 August 2008 |
| `178a/` | Gesetz über die Aufhebung der Realkorporationsgemeinde Langnau (SRL Nr. 178a) | 1 | one version (the oldest available), 1 August 2008 |
| `178b/` | Gesetz über die Aufhebung der Realkorporationsgemeinde Ottenhusen (SRL Nr. 178b) | 1 | one version (the oldest available), 1 August 2008 |
| `178c/` | Gesetz über die Aufhebung der Realkorporationsgemeinde Hochdorf (SRL Nr. 178c) | 1 | one version (the oldest available), 1 August 2008 |
| `179/` | Gesetz über die Aufhebung der Personalkorporationsgemeinde Honau (SRL Nr. 179) | 1 | one version (the oldest available), 1 August 2008 |
| `179a/` | Gesetz über die Aufhebung der Hintersässenkorporation Root (SRL Nr. 179a) | 1 | as enacted, 1 September 2012 |
| `180/` | Gesetz über die Vereinigung der Reinen Korporationsgemeinde Ermensee und der Gemischten Korporationsgemeinde Ermensee (SRL Nr. 180) | 1 | one version (the oldest available), 1 August 2008 |
| `180a/` | Gesetz über die Aufhebung der Realkorporationsgemeinde Richensee (SRL Nr. 180a) | 1 | as enacted, 1 September 2009 |
| `181/` | Gesetz über die Aufhebung der Personalkorporationsgemeinde Adligenswil (SRL Nr. 181) | 1 | one version (the oldest available), 1 August 2008 |
| `182/` | Gesetz über die Aufhebung der Personalkorporationsgemeinde Meggen (SRL Nr. 182) | 1 | one version (the oldest available), 1 August 2008 |
| `185/` | Gesetz betreffend Abtretung von Kollaturrechten an die Kirchgemeinden (SRL Nr. 185) | 1 | one version (the oldest available), 1 June 2013 |
| `187/` | Gesetz über die Kirchenverfassung (Einführung und Organisation kirchlicher Synoden) (SRL Nr. 187) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 March 2018 |
| `200-egzgb/` | Einführungsgesetz zum Schweizerischen Zivilgesetzbuch (SRL Nr. 200) | 9 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2026 |
| `215/` | Gesetz über das Handänderungs- und Hypothekarwesen (SRL Nr. 215) | 1 | one version (the oldest available), 1 June 2013 |
| `218/` | Gesetz zur Einführung des Bundesgesetzes über den Erwerb von Grundstücken durch Personen im Ausland (SRL Nr. 218) | 1 | one version (the oldest available), 1 July 2014 |
| `255-beurkundungsgesetz-beurkg/` | Gesetz über die öffentlichen Beurkundungen (SRL Nr. 255) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2022 |
| `260-justizgesetz-jusg/` | Gesetz über die Organisation der Gerichte und Behörden in Zivil-, Straf- und verwaltungsgerichtlichen Verfahren (SRL Nr. 260) | 8 | oldest version available, then each consolidated version: 1 July 2015 to 1 January 2026 |
| `280-anwaltsgesetz-anwg/` | Gesetz über das Anwaltspatent und die Parteivertretung (SRL Nr. 280) | 1 | one version (the oldest available), 1 June 2013 |
| `290-egschkg/` | Einführungsgesetz zum Bundesgesetz über Schuldbetreibung und Konkurs (SRL Nr. 290) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 July 2023 |
| `300-uestg/` | Übertretungsstrafgesetz (SRL Nr. 300) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2025 |
| `305-jvg/` | Gesetz über den Justizvollzug (SRL Nr. 305) | 2 | as enacted, then each consolidated version: 1 July 2016 to 1 September 2021 |
| `350-polg/` | Gesetz über die Luzerner Polizei (SRL Nr. 350) | 8 | oldest version available, then each consolidated version: 1 October 2013 to 17 October 2024 |
| `370-bsg/` | Gesetz über den Bevölkerungsschutz (SRL Nr. 370) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2023 |
| `372-zsg/` | Gesetz über den Zivilschutz (SRL Nr. 372) | 2 | oldest version available, then each consolidated version: 1 March 2015 to 1 January 2023 |
| `395-kantonales-landesversorgungsgesetz/` | Einführungsgesetz zum Bundesgesetz über die wirtschaftliche Landesversorgung (SRL Nr. 395) | 2 | as enacted, then each consolidated version: 1 November 2005 to 1 January 2023 |
| `400a-vbg/` | Gesetz über die Volksschulbildung (SRL Nr. 400a) | 9 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2026 |
| `402/` | Kulturförderungsgesetz (SRL Nr. 402) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2027 |
| `420/` | Bibliotheksgesetz (SRL Nr. 420) | 1 | one version (the oldest available), 1 January 2014 |
| `430-bwg/` | Gesetz über die Berufsbildung und die Weiterbildung (SRL Nr. 430) | 3 | oldest version available, then each consolidated version: 1 August 2013 to 1 September 2021 |
| `501-gymbg/` | Gesetz über die Gymnasialbildung (SRL Nr. 501) | 5 | oldest version available, then each consolidated version: 1 August 2013 to 1 January 2026 |
| `515-ph-gesetz/` | Gesetz über die Lehrerinnen- und Lehrerbildung und die Pädagogische Hochschule Luzern (SRL Nr. 515) | 2 | oldest version available, then each consolidated version: 30 November 2014 to 1 January 2026 |
| `539-universitatsgesetz-unig/` | Gesetz über die universitäre Hochschulbildung (SRL Nr. 539) | 2 | oldest version available, then each consolidated version: 30 November 2014 to 1 February 2023 |
| `575-stipendiengesetz/` | Gesetz über Ausbildungsbeiträge (SRL Nr. 575) | 1 | as enacted, 18 May 2014 |
| `585-archivgesetz/` | Gesetz über das Archivwesen (SRL Nr. 585) | 4 | as enacted, then each consolidated version: 1 June 2013 to 1 June 2025 |
| `595-dschg/` | Gesetz über den Schutz der Kulturdenkmäler (SRL Nr. 595) | 1 | one version (the oldest available), 1 July 2014 |
| `600-flg/` | Gesetz über die Steuerung der Finanzen und Leistungen (SRL Nr. 600) | 5 | oldest version available, then each consolidated version: 1 August 2013 to 1 January 2024 |
| `601/` | Staatsbeitragsgesetz (SRL Nr. 601) | 1 | one version (the oldest available), 1 January 2013 |
| `610-fag/` | Gesetz über den Finanzausgleich (SRL Nr. 610) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `615/` | Finanzkontrollgesetz (SRL Nr. 615) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 June 2025 |
| `620-stg/` | Steuergesetz (SRL Nr. 620) | 14 | oldest version available, then each consolidated version: 1 January 2016 to 1 October 2026 |
| `630-estg/` | Gesetz betreffend die Erbschaftssteuern (SRL Nr. 630) | 5 | oldest version available, then each consolidated version: 1 July 2014 to 1 June 2025 |
| `645-hstg/` | Gesetz über die Handänderungssteuer (SRL Nr. 645) | 4 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2025 |
| `647-ggstg/` | Gesetz über die Grundstückgewinnsteuer (SRL Nr. 647) | 3 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2025 |
| `650-tourismusgesetz/` | Gesetz über Abgaben und Beiträge im Tourismus (SRL Nr. 650) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `652/` | Gesetz betreffend die teilweise Abänderung des Steuergesetzes vom 30. November 1892 (SRL Nr. 652) | 1 | one version (the oldest available), 1 June 2013 |
| `670/` | Gesetz über die Gewinnung von Bodenschätzen und die Nutzung des Untergrunds (SRL Nr. 670) | 1 | as enacted, 1 January 2014 |
| `677/` | Gesetz über das Salzregal (SRL Nr. 677) | 1 | as enacted, 1 December 1975 |
| `680-gebg/` | Gebührengesetz (SRL Nr. 680) | 1 | one version (the oldest available), 1 June 2013 |
| `690-umwandlungsgesetz/` | Gesetz über die Umwandlung der Luzerner Kantonalbank in eine Aktiengesellschaft (SRL Nr. 690) | 1 | one version (the oldest available), 1 January 2011 |
| `700-egusg/` | Einführungsgesetz zum Bundesgesetz über den Umweltschutz (SRL Nr. 700) | 5 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2025 |
| `702-eggschg/` | Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (SRL Nr. 702) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 February 2018 |
| `709a-nlg/` | Gesetz über den Natur- und Landschaftsschutz (SRL Nr. 709a) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2020 |
| `720-fig/` | Fischereigesetz (SRL Nr. 720) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `725-kantonales-jagdgesetz-kjsg/` | Kantonales Gesetz über die Jagd und den Schutz wildlebender Säugetiere und Vögel (SRL Nr. 725) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2020 |
| `730-entg/` | Enteignungsgesetz (SRL Nr. 730) | 4 | oldest version available, then each consolidated version: 1 January 2016 to 1 March 2024 |
| `735-pbg/` | Planungs- und Baugesetz (SRL Nr. 735) | 7 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2025 |
| `740-fsg/` | Gesetz über den Feuerschutz (SRL Nr. 740) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 July 2022 |
| `750-gvg/` | Gebäudeversicherungsgesetz (SRL Nr. 750) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 March 2017 |
| `755-strg/` | Strassengesetz (SRL Nr. 755) | 7 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2025 |
| `758a-wegg/` | Weggesetz (SRL Nr. 758a) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2020 |
| `760-wbg/` | Wasserbaugesetz (SRL Nr. 760) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 March 2024 |
| `770-wnvg/` | Wassernutzungs- und Wasserversorgungsgesetz (SRL Nr. 770) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2020 |
| `772/` | Kantonales Stromversorgungsgesetz (SRL Nr. 772) | 1 | as enacted, 1 June 2013 |
| `773-keng/` | Kantonales Energiegesetz (SRL Nr. 773) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 March 2025 |
| `775-ovg/` | Gesetz über den öffentlichen Verkehr (SRL Nr. 775) | 5 | oldest version available, then each consolidated version: 1 July 2015 to 1 January 2026 |
| `776/` | Gesetz über die Verkehrsabgaben und den Vollzug des eidgenössischen Strassenverkehrsrechtes (SRL Nr. 776) | 4 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2025 |
| `783-gvm/` | Gesetz über die Verwendung von Motorfahrzeugen ausserhalb der öffentlichen Strassen und Wege (SRL Nr. 783) | 1 | one version (the oldest available), 1 January 2010 |
| `788a/` | Gesetz über die Schiffssteuer (SRL Nr. 788a) | 1 | one version (the oldest available), 1 January 2005 |
| `800-gesg/` | Gesundheitsgesetz (SRL Nr. 800) | 9 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `800a/` | Spitalgesetz (SRL Nr. 800a) | 8 | oldest version available, then each consolidated version: 1 June 2013 to 1 July 2025 |
| `804a-kantonales-sportforderungsgesetz/` | Gesetz über die Förderung von Sport und Bewegung (SRL Nr. 804a) | 1 | as enacted, 1 July 2014 |
| `810-egfapg/` | Einführungsgesetz zum Bundesgesetz über die Förderung der Ausbildung im Bereich der Pflege (SRL Nr. 810) | 1 | as enacted, 1 July 2024 |
| `847/` | Gesetz über die Tierseuchenkasse (SRL Nr. 847) | 1 | one version (the oldest available), 1 January 2010 |
| `848-hug/` | Gesetz über das Halten von Hunden (SRL Nr. 848) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2025 |
| `851/` | Gesetz betreffend die Einführung des eidgenössischen Fabrikgesetzes vom 18. Juni 1914 (Verfahren für Zivilstreitigkeiten aus dem Dienstverhältnis und kantonales Einigungsamt) (SRL Nr. 851) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2016 |
| `855/` | Gesetz über die Ruhetage und die Öffnungs- und Schliessungszeiten der Verkaufsgeschäfte (SRL Nr. 855) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 27 September 2026 |
| `861/` | Gesetz über die steuerbegünstigten Arbeitsbeschaffungsreserven (SRL Nr. 861) | 1 | one version (the oldest available), 1 January 2010 |
| `865-egkvg/` | Einführungsgesetz zum Bundesgesetz über die Krankenversicherung (SRL Nr. 865) | 5 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `866-pramienverbilligungsgesetz/` | Gesetz über die Verbilligung von Prämien der Krankenversicherung (SRL Nr. 866) | 6 | oldest version available, then each consolidated version: 1 January 2014 to 1 July 2021 |
| `867-bpg/` | Betreuungs- und Pflegegesetz (SRL Nr. 867) | 5 | oldest version available, then each consolidated version: 1 July 2015 to 1 July 2024 |
| `880-gesetz-uber-das-sozialversicherungszentrum-sovzg/` | Einführungsgesetz zu den Bundesgesetzen über die Alters- und Hinterlassenenversicherung und über die Invalidenversicherung (SRL Nr. 880) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `881/` | Gesetz über die Ergänzungsleistungen zur AHV/IV (SRL Nr. 881) | 7 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2023 |
| `885-kantonales-familienzulagengesetz-fzg/` | Gesetz über die Familienzulagen (SRL Nr. 885) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `887-kinderbetreuungsgesetz-kibeg/` | Gesetz über die familienergänzende Kinderbetreuung (SRL Nr. 887) | 2 | as enacted, then each consolidated version: 1 January 2026 to 1 August 2026 |
| `890-avahg/` | Gesetz über die Arbeitslosenversicherung und den Arbeitslosenhilfsfonds (SRL Nr. 890) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2023 |
| `892-shg/` | Sozialhilfegesetz (SRL Nr. 892) | 5 | as enacted, then each consolidated version: 1 January 2016 to 1 January 2024 |
| `893c-egohg/` | Einführungsgesetz zum Opferhilfegesetz des Bundes (SRL Nr. 893c) | 1 | as enacted, 1 June 2013 |
| `894-seg/` | Gesetz über soziale Einrichtungen (SRL Nr. 894) | 3 | oldest version available, then each consolidated version: 1 July 2015 to 1 January 2020 |
| `897/` | Gesetz über Wohnbau- und Eigentumsförderung (SRL Nr. 897) | 2 | oldest version available, then each consolidated version: 1 August 2008 to 1 March 2017 |
| `898/` | Gesetz über die Erhaltung von Wohnraum (SRL Nr. 898) | 1 | one version (the oldest available), 1 June 2015 |
| `900-stareg/` | Gesetz über die Standortförderung und die Regionalpolitik (SRL Nr. 900) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 October 2026 |
| `902-klwg/` | Kantonales Landwirtschaftsgesetz (SRL Nr. 902) | 4 | oldest version available, then each consolidated version: 1 June 2015 to 1 September 2021 |
| `938/` | Gesetz über die Viehversicherung (SRL Nr. 938) | 1 | one version (the oldest available), 1 July 2003 |
| `945-kwag/` | Kantonales Waldgesetz (SRL Nr. 945) | 3 | oldest version available, then each consolidated version: 1 March 2014 to 1 January 2020 |
| `955-gpg/` | Gewerbepolizeigesetz (SRL Nr. 955) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2020 |
| `980-gastgewerbegesetz-gag/` | Gesetz über das Gastgewerbe, den Handel mit alkoholischen Getränken und die Fasnacht (SRL Nr. 980) | 3 | oldest version available, then each consolidated version: 1 September 2010 to 27 September 2026 |
| `991-egbgs/` | Einführungsgesetz zum Bundesgesetz über Geldspiele (SRL Nr. 991) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 July 2020 |
| `3-kbuv/` | Kantonale Bürgerrechtsverordnung (SRL Nr. 3) | 3 | oldest version available, then each consolidated version: 1 August 2008 to 1 January 2018 |
| `6/` | Vollziehungsverordnung zum Gesetz über die Niederlassung und den Aufenthalt (SRL Nr. 6) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2021 |
| `8/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Ausländerinnen und Ausländer und zum Asylgesetz (SRL Nr. 8) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2022 |
| `9/` | Verordnung über den Vollzug der Bundesgesetzgebung über die Ausweise für Schweizer Staatsangehörige (SRL Nr. 9) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `12-e-voting-verordnung/` | Verordnung über die versuchsweise Einführung der elektronischen Stimmabgabe (SRL Nr. 12) | 2 | as enacted, then each consolidated version: 1 August 2010 to 1 January 2026 |
| `13/` | Verordnung über die elektronische Erfassung und Auszählung von Stimmzetteln bei Abstimmungen (SRL Nr. 13) | 1 | as enacted, 15 April 2018 |
| `25a-registerverordnung/` | Verordnung zum Registergesetz (SRL Nr. 25a) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 September 2021 |
| `25c-owv/` | Verordnung zum Gesetz über die Datendrehscheibe und das Informationssystem Objektwesen (SRL Nr. 25c) | 1 | as enacted, 1 January 2026 |
| `26a/` | Informatikverordnung (SRL Nr. 26a) | 4 | oldest version available, then each consolidated version: 1 July 2014 to 1 September 2021 |
| `26b-informatiksicherheitsverordnung/` | Verordnung über die Informatiksicherheit und über die Nutzung von Informatikmitteln (SRL Nr. 26b) | 7 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2025 |
| `26d-e-id-verordnung/` | Verordnung über den Testbetrieb eines elektronischen Identitätsverwaltungssystems und eines Service-Portals (SRL Nr. 26d) | 1 | as enacted, 1 April 2024 |
| `28b/` | Statistikverordnung (SRL Nr. 28b) | 2 | oldest version available, then each consolidated version: 1 February 2015 to 1 January 2019 |
| `28c-gebuhrenverordnung-lustat/` | Verordnung über die Gebühren für individuelle statistische Dienstleistungen von Lustat Statistik Luzern (SRL Nr. 28c) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2026 |
| `28d/` | Verordnung über die Bevölkerungsstatistik (SRL Nr. 28d) | 1 | as enacted, 1 January 2011 |
| `28e/` | Verordnung über die kantonalen Bevölkerungsbefragungen (SRL Nr. 28e) | 3 | as enacted, then each consolidated version: 1 April 2013 to 1 February 2019 |
| `28f/` | Verordnung über die Gemeindefinanzstatistik (SRL Nr. 28f) | 2 | as enacted, then each consolidated version: 1 April 2009 to 1 January 2018 |
| `28g/` | Verordnung über die Steuerstatistik (SRL Nr. 28g) | 1 | as enacted, 1 April 2009 |
| `28h/` | Verordnung über die Spitex-Statistik (SRL Nr. 28h) | 1 | as enacted, 1 April 2009 |
| `28m/` | Verordnung über die Errichtung, Organisation und Finanzierung der zentralen Statistikstelle (SRL Nr. 28m) | 6 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `29a-giv/` | Geoinformationsverordnung (SRL Nr. 29a) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2022 |
| `36-organisationsverordnung-ov/` | Verordnung über die Organisation, die Führung und die Kontrolle der kantonalen Verwaltung (SRL Nr. 36) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 March 2023 |
| `36a-informationsverordnung-infov/` | Verordnung über die Information der Öffentlichkeit durch den Regierungsrat und die Verwaltung (SRL Nr. 36a) | 2 | as enacted, then each consolidated version: 1 September 2017 to 1 June 2025 |
| `36b-vvv/` | Verordnung über das Vernehmlassungsverfahren (SRL Nr. 36b) | 1 | as enacted, 1 September 2017 |
| `36c-organisationsreglement/` | Reglement über die Aufbau- und Ablauforganisation interdepartementaler Gremien (SRL Nr. 36c) | 1 | as enacted, 1 March 2015 |
| `37/` | Verordnung über die Aufgaben der Departemente und der Staatskanzlei sowie die Gliederung der Departemente in Dienststellen (SRL Nr. 37) | 11 | oldest version available, then each consolidated version: 1 October 2015 to 1 January 2027 |
| `37a/` | Verordnung über die Zuordnung der Anstalten zu den Departementen (SRL Nr. 37a) | 2 | oldest version available, then each consolidated version: 1 August 2013 to 1 January 2019 |
| `38b-kdsv/` | Kantonale Datenschutzverordnung (SRL Nr. 38b) | 3 | oldest version available, then each consolidated version: 1 August 2013 to 1 June 2025 |
| `39a/` | Verordnung zum Gesetz über die Videoüberwachung (SRL Nr. 39a) | 2 | oldest version available, then each consolidated version: 1 August 2013 to 1 September 2021 |
| `52-personalverordnung-pvo/` | Verordnung zum Personalgesetz (SRL Nr. 52) | 22 | oldest version available, then each consolidated version: 1 August 2015 to 1 August 2026 |
| `52a/` | Verordnung über die Wahlen und die übrigen personalrechtlichen Entscheide im Zuständigkeitsbereich des Kantonsgerichtes (SRL Nr. 52a) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `53/` | Verordnung über die Beschäftigung der persönlichen Mitarbeiter und Mitarbeiterinnen (SRL Nr. 53) | 1 | one version (the oldest available), 1 July 2007 |
| `54-sozialplan/` | Verordnung über die Massnahmen bei einem grösseren Stellenabbau (SRL Nr. 54) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2019 |
| `55/` | Verordnung über die Eides- und Gelübdeformel (SRL Nr. 55) | 1 | as enacted, 1 August 2008 |
| `60/` | Verordnung über die Erteilung des Fähigkeitszeugnisses als Gemeindeschreiber oder als Gemeindeschreiberin (SRL Nr. 60) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2023 |
| `61/` | Verordnung über die Prüfung der Grundbuchverwalterinnen und -verwalter und ihrer Stellvertretungen (SRL Nr. 61) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `64/` | Verordnung über die Prüfung der Betreibungs- und Konkursbeamten sowie der Sachwalter (SRL Nr. 64) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `73a-bvo/` | Besoldungsverordnung für das Staatspersonal (SRL Nr. 73a) | 7 | oldest version available, then each consolidated version: 1 July 2015 to 1 January 2026 |
| `75-bvol/` | Besoldungsverordnung für die Lehrpersonen und die Fachpersonen der schulischen Dienste (SRL Nr. 75) | 9 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2026 |
| `91/` | Verordnung über Vergütungen im Bildungswesen (SRL Nr. 91) | 3 | oldest version available, then each consolidated version: 1 August 2013 to 1 January 2018 |
| `104/` | Verordnung über die Entschädigung der Amtsärzte und deren Stellvertreter (SRL Nr. 104) | 1 | one version (the oldest available), 1 January 2004 |
| `123/` | Verordnung über Entschädigungen an die Mitglieder vom Kantonsgericht bestellter Prüfungskommissionen und Aufsichtsbehörden (SRL Nr. 123) | 1 | one version (the oldest available), 1 June 2015 |
| `131-volupk/` | Verordnung über die Luzerner Pensionskasse (SRL Nr. 131) | 1 | one version (the oldest available), 1 January 2014 |
| `135-lupk-reglement/` | Reglement der Luzerner Pensionskasse (SRL Nr. 135) | 9 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2026 |
| `151-gv/` | Verordnung über die Gemeinden im Kanton Luzern (SRL Nr. 151) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `152/` | Verordnung über die Gemeindeaufsicht (SRL Nr. 152) | 2 | as enacted, then each consolidated version: 1 July 2014 to 1 April 2017 |
| `155/` | Verordnung über die Schreibweise der Ortsnamen (SRL Nr. 155) | 1 | one version (the oldest available), 1 June 2015 |
| `161-fhgv/` | Verordnung zum Gesetz über den Finanzhaushalt der Gemeinden (SRL Nr. 161) | 3 | as enacted, then each consolidated version: 1 January 2018 to 1 June 2023 |
| `201/` | Verordnung über das Zivilstandswesen (SRL Nr. 201) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 April 2017 |
| `202/` | Verordnung über die Stiftungsaufsicht (SRL Nr. 202) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 April 2017 |
| `203/` | Kantonale Verordnung über die Adoption (SRL Nr. 203) | 2 | as enacted, then each consolidated version: 1 July 2014 to 1 January 2018 |
| `203a/` | Verordnung über den Vollzug zivilgerichtlicher Anordnungen der elektronischen Überwachung zum Schutz vor Gewalt, Drohungen oder Nachstellungen (SRL Nr. 203a) | 1 | as enacted, 1 January 2022 |
| `204/` | Verordnung über die Aufnahme von Pflegekindern (SRL Nr. 204) | 4 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `205/` | Verordnung über die Zuständigkeiten gemäss dem Bundesgesetz über internationale Kindesentführung und die Haager Übereinkommen zum Schutz von Kindern und Erwachsenen (SRL Nr. 205) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 April 2017 |
| `206/` | Verordnung über den Kindes- und Erwachsenenschutz (SRL Nr. 206) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 April 2017 |
| `210/` | Verordnung über das Verfahren in Erbschaftsfällen (SRL Nr. 210) | 1 | one version (the oldest available), 1 January 2013 |
| `216/` | Verordnung über die freiwilligen öffentlichen Versteigerungen (SRL Nr. 216) | 1 | one version (the oldest available), 1 January 2002 |
| `218a/` | Vollzugsverordnung zum Gesetz zur Einführung des Bundesgesetzes über den Erwerb von Grundstücken durch Personen im Ausland (SRL Nr. 218a) | 2 | as enacted, then each consolidated version: 1 July 2014 to 1 April 2017 |
| `219b/` | Verordnung über die Anzeige eines Tierfundes (SRL Nr. 219b) | 1 | as enacted, 1 April 2003 |
| `222/` | Verordnung betreffend die Viehverpfändung (SRL Nr. 222) | 1 | one version (the oldest available), 1 July 2003 |
| `226-kantonale-grundbuchverordnung/` | Verordnung über die Organisation des Grundbuchwesens (SRL Nr. 226) | 1 | one version (the oldest available), 1 June 2015 |
| `226a-it-grundbuch-verordnung/` | Verordnung über die Führung des Grundbuchs mittels Informatik (SRL Nr. 226a) | 3 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2023 |
| `228-grundbuchgebuhrentarif-gbgt/` | Verordnung über die Grundbuchgebühren (SRL Nr. 228) | 4 | as enacted, then each consolidated version: 1 June 2015 to 1 January 2026 |
| `256-beurkundungsverordnung-beurkv/` | Verordnung über die öffentlichen Beurkundungen (SRL Nr. 256) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2023 |
| `257/` | Verordnung über die Prüfung der Notare (SRL Nr. 257) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2024 |
| `258-beurkgebv/` | Verordnung über die Beurkundungsgebühren (SRL Nr. 258) | 2 | oldest version available, then each consolidated version: 1 July 2012 to 1 January 2022 |
| `262-justizverordnung-jusv/` | Verordnung zum Gesetz über die Organisation der Gerichte und Behörden in Zivil-, Straf- und verwaltungsgerichtlichen Verfahren (SRL Nr. 262) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `265-justiz-kostenverordnung-juskv/` | Verordnung über die Kosten in Zivil-, Straf- und verwaltungsgerichtlichen Verfahren (SRL Nr. 265) | 6 | as enacted, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `271/` | Verordnung über die Mediation im Jugendstrafverfahren (SRL Nr. 271) | 1 | as enacted, 1 January 2011 |
| `275/` | Verordnung über die Staatsanwaltschaft (SRL Nr. 275) | 7 | oldest version available, then each consolidated version: 1 November 2015 to 1 January 2025 |
| `281-aav/` | Verordnung betreffend die Aufsicht über die Anwältinnen und Anwälte (SRL Nr. 281) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 January 2026 |
| `282-apv/` | Verordnung über das Anwaltspraktikum und die für die Ausübung des Anwaltsberufes erforderlichen Prüfungen (SRL Nr. 282) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 April 2024 |
| `290a/` | Vollzugsverordnung zum Einführungsgesetz zum Bundesgesetz über Schuldbetreibung und Konkurs (SRL Nr. 290a) | 3 | oldest version available, then each consolidated version: 1 June 2013 to 1 February 2026 |
| `314-kobv/` | Kantonale Ordnungsbussenverordnung (SRL Nr. 314) | 6 | oldest version available, then each consolidated version: 1 October 2013 to 1 April 2025 |
| `327-jvv/` | Verordnung über den Justizvollzug (SRL Nr. 327) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `351-polv/` | Verordnung über die Luzerner Polizei (SRL Nr. 351) | 18 | oldest version available, then each consolidated version: 1 September 2014 to 1 July 2026 |
| `356-ksmsv/` | Kantonale Verordnung über Massnahmen zur Unterstützung der Sicherheit von Minderheiten mit besonderen Schutzbedürfnissen (SRL Nr. 356) | 1 | as enacted, 1 August 2025 |
| `364/` | Verordnung über die Zuständigkeit im militärischen Disziplinarstrafrecht (SRL Nr. 364) | 2 | as enacted, then each consolidated version: 1 July 2007 to 1 October 2024 |
| `371/` | Verordnung über den Bevölkerungsschutz (SRL Nr. 371) | 3 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `372a/` | Verordnung über den Zivilschutz (SRL Nr. 372a) | 3 | oldest version available, then each consolidated version: 1 March 2015 to 1 January 2026 |
| `372c/` | Verordnung zur Einführung des am 20. Dezember 2019 geänderten Bundesgesetzes über den Bevölkerungsschutz und den Zivilschutz (SRL Nr. 372c) | 1 | as enacted, 1 January 2021 |
| `373/` | Verordnung über den Gebührenbezug im Zivilschutz (SRL Nr. 373) | 4 | oldest version available, then each consolidated version: 1 January 2004 to 1 January 2025 |
| `385/` | Vollzugsverordnung zum Bundesgesetz über die Wehrpflichtersatzabgabe (SRL Nr. 385) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 November 2022 |
| `390-erwerbsersatzordnung/` | Verordnung über die Einführung des Bundesgesetzes über die Erwerbsausfallentschädigungen an Wehrpflichtige (SRL Nr. 390) | 1 | one version (the oldest available), 15 July 1980 |
| `396-kantonale-landesversorgungsverordnung/` | Verordnung über die wirtschaftliche Landesversorgung (SRL Nr. 396) | 1 | as enacted, 1 July 2007 |
| `405-volksschulbildungsverordnung-vbv/` | Verordnung zum Gesetz über die Volksschulbildung (SRL Nr. 405) | 12 | oldest version available, then each consolidated version: 1 January 2015 to 1 August 2025 |
| `405a/` | Verordnung über die Beurteilung der Lernenden in der Volksschule (SRL Nr. 405a) | 4 | oldest version available, then each consolidated version: 1 August 2012 to 1 November 2023 |
| `405b/` | Verordnung über die Übertrittsverfahren in der Volksschule (SRL Nr. 405b) | 5 | oldest version available, then each consolidated version: 1 August 2012 to 1 November 2023 |
| `406/` | Verordnung über die Förderangebote der Volksschule (SRL Nr. 406) | 2 | oldest version available, then each consolidated version: 1 August 2015 to 1 August 2025 |
| `408/` | Verordnung über die Schuldienste (SRL Nr. 408) | 4 | oldest version available, then each consolidated version: 1 August 2011 to 1 January 2024 |
| `409/` | Verordnung über die Sonderschulung (SRL Nr. 409) | 7 | oldest version available, then each consolidated version: 1 August 2015 to 1 January 2026 |
| `415/` | Verordnung über die kommunalen Musikschulen und die ausserschulische musikalische Talentförderung (SRL Nr. 415) | 5 | as enacted, then each consolidated version: 1 August 2010 to 1 January 2024 |
| `421/` | Verordnung über das kantonale Bibliotheksangebot (SRL Nr. 421) | 4 | oldest version available, then each consolidated version: 1 August 2014 to 1 January 2025 |
| `432/` | Verordnung zum Gesetz über die Berufsbildung und die Weiterbildung (SRL Nr. 432) | 11 | oldest version available, then each consolidated version: 1 September 2014 to 1 August 2026 |
| `438/` | Reglement über die Aufnahme, die Promotion und die Abschlussprüfungen an den Fachmittelschulen des Kantons Luzern (SRL Nr. 438) | 9 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2026 |
| `444/` | Reglement über die Berufsmaturität (SRL Nr. 444) | 12 | oldest version available, then each consolidated version: 1 February 2015 to 1 August 2026 |
| `502-gymbv/` | Verordnung zum Gesetz über die Gymnasialbildung (SRL Nr. 502) | 9 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2027 |
| `503/` | Verordnung über die Benützung kantonaler Schulanlagen durch Dritte (SRL Nr. 503) | 2 | oldest version available, then each consolidated version: 1 September 2014 to 1 August 2025 |
| `506/` | Reglement für die Maturitätsprüfungen im Kanton Luzern (SRL Nr. 506) | 8 | as enacted, then each consolidated version: 1 August 2008 to 1 August 2031 |
| `506a/` | Reglement über die Maturitätsprüfungen am Gymnasium der RIS Swiss Section, Deutschsprachige Schule Bangkok (SRL Nr. 506a) | 3 | as enacted, then each consolidated version: 1 August 2008 to 1 August 2031 |
| `506b/` | Reglement über den Passerellen-Lehrgang und die Ergänzungsprüfungen für die Zulassung zu den universitären Hochschulen (SRL Nr. 506b) | 4 | oldest version available, then each consolidated version: 1 July 2012 to 1 August 2026 |
| `515a-pvo-ph-luzern/` | Personalverordnung der Pädagogischen Hochschule Luzern (SRL Nr. 515a) | 2 | as enacted, then each consolidated version: 1 August 2022 to 1 January 2026 |
| `516a-ph-ausbildungsreglement/` | Studienreglement über die Ausbildung der Pädagogischen Hochschule Luzern (SRL Nr. 516a) | 7 | oldest version available, then each consolidated version: 1 February 2015 to 1 August 2025 |
| `516b-ph-weiterbildungsreglement/` | Studienreglement über die Weiterbildung der Pädagogischen Hochschule Luzern (SRL Nr. 516b) | 4 | as enacted, then each consolidated version: 1 August 2013 to 1 August 2026 |
| `516c-ph-berufsbildungsreglement/` | Studienreglement über die Ausbildung der Pädagogischen Hochschule Luzern im Bereich der Berufsbildung (SRL Nr. 516c) | 4 | as enacted, then each consolidated version: 1 August 2014 to 1 August 2024 |
| `518/` | Reglement für die Verwendung von Drittmitteln an der Pädagogischen Hochschule Luzern (SRL Nr. 518) | 1 | as enacted, 1 February 2015 |
| `518a/` | Verordnung über die Offenlegung von Drittmitteln der Pädagogischen Hochschule Luzern (SRL Nr. 518a) | 1 | as enacted, 1 January 2018 |
| `520c/` | Personalverordnung der Hochschule Luzern, FH Zentralschweiz (SRL Nr. 520c) | 3 | oldest version available, then each consolidated version: 1 October 2021 to 1 January 2026 |
| `520e-gebuhrenverordnung-hslu-gebvo-hslu/` | Verordnung über die Gebühren an der Hochschule Luzern, FH Zentralschweiz (SRL Nr. 520e) | 2 | oldest version available, then each consolidated version: 1 September 2013 to 1 March 2025 |
| `520f/` | Reglement zum Fundraising der Hochschule Luzern, FH Zentralschweiz (SRL Nr. 520f) | 1 | one version (the oldest available), 1 January 2019 |
| `524/` | Reglement zur wissenschaftlichen Integrität und zur guten wissenschaftlichen Praxis der Hochschule Luzern, FH Zentralschweiz (SRL Nr. 524) | 1 | as enacted, 1 September 2015 |
| `539a/` | Personalverordnung der Universität Luzern (SRL Nr. 539a) | 6 | oldest version available, then each consolidated version: 1 December 2013 to 1 January 2026 |
| `539d/` | Berufungsreglement der Universität Luzern (SRL Nr. 539d) | 5 | oldest version available, then each consolidated version: 1 August 2013 to 1 February 2027 |
| `539e/` | Rahmenreglement für die Institute, Zentren und Akademien der Fakultäten der Universität Luzern (SRL Nr. 539e) | 3 | oldest version available, then each consolidated version: 1 October 2006 to 1 April 2024 |
| `539g/` | Reglement über die wissenschaftlichen Assistentinnen und Assistenten an der Universität Luzern (SRL Nr. 539g) | 2 | as enacted, then each consolidated version: 1 August 2013 to 1 February 2024 |
| `539h/` | Reglement über die Anstellung von Assistenzprofessorinnen und Assistenzprofessoren (SRL Nr. 539h) | 2 | oldest version available, then each consolidated version: 1 June 2006 to 1 August 2018 |
| `539i/` | Rahmenreglement für die Weiterbildung an der Universität Luzern (SRL Nr. 539i) | 4 | as enacted, then each consolidated version: 1 February 2014 to 1 August 2025 |
| `539j/` | Reglement betreffend die Weiterbeschäftigung an der Universität Luzern nach der Erfüllung des 65. Altersjahres (SRL Nr. 539j) | 1 | as enacted, 1 August 2023 |
| `539k-integritatsreglement-unilu/` | Reglement über die wissenschaftliche Integrität in der Forschung und die gute wissenschaftliche Praxis an der Universität Luzern (SRL Nr. 539k) | 2 | as enacted, then each consolidated version: 1 January 2016 to 1 August 2023 |
| `539l/` | Verordnung über die Offenlegung von Drittmitteln der Universität Luzern (SRL Nr. 539l) | 1 | as enacted, 1 January 2018 |
| `539m/` | Organisationsreglement für die Weiterbildungsakademie der Universität Luzern (SRL Nr. 539m) | 2 | as enacted, then each consolidated version: 30 June 2022 to 1 August 2024 |
| `539n-rsb-unilu/` | Reglement zum Schutz vor sexueller Belästigung an der Universität Luzern (SRL Nr. 539n) | 2 | as enacted, then each consolidated version: 1 February 2023 to 1 April 2024 |
| `539o-fundraising-policy-unilu/` | Reglement über die Einwerbung und Entgegennahme von Spenden und Sponsoringbeiträgen (Fundraising) an der Universität Luzern (SRL Nr. 539o) | 2 | as enacted, then each consolidated version: 1 August 2023 to 1 February 2025 |
| `539p-ethik-board-reglement/` | Reglement zur Gewährleistung der Integrität von Studienteilnehmenden (SRL Nr. 539p) | 2 | as enacted, then each consolidated version: 1 August 2023 to 1 February 2026 |
| `539q/` | Organisationsreglement zur Ermittlung des Antrages für die Wahl der Rektorin oder des Rektors (SRL Nr. 539q) | 1 | as enacted, 1 February 2024 |
| `539s/` | Reglement zur Verleihung von Titeln an der Universität Luzern (SRL Nr. 539s) | 3 | as enacted, then each consolidated version: 1 April 2024 to 1 December 2025 |
| `539u-reglement-ausstand-unilu/` | Reglement betreffend Ausstand in Berufungs- und Beförderungsverfahren sowie in Verfahren auf Verleihung von Titeln (SRL Nr. 539u) | 2 | as enacted, then each consolidated version: 1 August 2024 to 1 February 2026 |
| `540a-fakultatsreglement-rf/` | Reglement der Rechtswissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 540a) | 2 | oldest version available, then each consolidated version: 1 August 2007 to 1 August 2024 |
| `540d/` | Reglement über den Zertifikatslehrgang «Judikative» (SRL Nr. 540d) | 1 | as enacted, 1 January 2009 |
| `540e/` | Reglement zum Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Agrarrecht» der Universität Luzern (SRL Nr. 540e) | 2 | as enacted, then each consolidated version: 1 February 2011 to 1 September 2025 |
| `540i/` | Reglement über den Zertifikatsstudiengang «Arbitration» (SRL Nr. 540i) | 1 | as enacted, 1 January 2013 |
| `540k/` | Reglement über den Zertifikatslehrgang «Forensics I» an der Rechtswissenschaftlichen Fakultät der Universität Luzern (Certificate of Advanced Studies [CAS] in Forensics I der Universität Luzern); CAS Forensics I (SRL Nr. 540k) | 3 | as enacted, then each consolidated version: 1 January 2014 to 1 November 2020 |
| `540l/` | Reglement über den Zertifikatslehrgang «Wirtschaftsstrafrecht» an der Rechtswissenschaftlichen Fakultät der Universität Luzern (Certificate of Advanced Studies [CAS] in Wirtschaftsstrafrecht der Universität Luzern); CAS WISTRA (SRL Nr. 540l) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 November 2020 |
| `540m/` | Reglement über den Zertifikatslehrgang «CAS Forensics II» an der Rechtswissenschaftlichen Fakultät der Universität Luzern (Certificate of Advanced Studies [CAS] in Forensics II der Universität Luzern); CAS Forensics II (SRL Nr. 540m) | 3 | as enacted, then each consolidated version: 1 January 2014 to 1 November 2020 |
| `540o/` | Reglement über den Zertifikatslehrgang «Forensische Psychiatrie und Psychologie» an der Rechtswissenschaftlichen Fakultät der Universität Luzern (Certificate of Advanced Studies [CAS] in Forensischer Psychiatrie und Psychologie der Universität Luzern); CAS Forensische Psychiatrie und Psychologie (SRL Nr. 540o) | 2 | as enacted, then each consolidated version: 1 August 2016 to 1 November 2020 |
| `540p/` | Reglement über den Zertifikatslehrgang «Certificate of Advanced Studies (CAS) in Krankenversicherungsrecht an der Rechtswissenschaftlichen Fakultät der Universität Luzern» (CAS Krankenversicherungsrecht) (SRL Nr. 540p) | 1 | as enacted, 1 January 2022 |
| `540q/` | Reglement über den Zertifikatslehrgang «Certificate of Advanced Studies (CAS) in Privatversicherungsrecht an der Rechtswissenschaftlichen Fakultät der Universität Luzern» (CAS Privatversicherungsrecht) (SRL Nr. 540q) | 1 | as enacted, 1 January 2022 |
| `540r-organisationsreglement-ccr/` | Organisationsreglement Zentrum für Konflikt und Verfahren (SRL Nr. 540r) | 1 | as enacted, 1 December 2024 |
| `540s-organisationsreglement-cls/` | Organisationsreglement Center for Law and Sustainability CLS (Zentrum für Recht und Nachhaltigkeit) (SRL Nr. 540s) | 1 | as enacted, 1 June 2025 |
| `540t/` | Organisationsreglement Institut für Justizforschung (IJF) (SRL Nr. 540t) | 1 | as enacted, 1 January 2026 |
| `541-fakultatsreglement-tf/` | Reglement der Theologischen Fakultät der Universität Luzern (SRL Nr. 541) | 3 | as enacted, then each consolidated version: 1 October 2013 to 1 August 2024 |
| `541aa-cas-as/` | Reglement über das Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Aufsuchender Seelsorge mit Schwerpunkt Armeeseelsorge» der Universität Luzern in Kooperation mit der Höheren Kaderausbildung der Armee (SRL Nr. 541aa) | 1 | as enacted, 1 August 2025 |
| `541ab/` | Reglement zum Weiterbildungsangebot «CAS in Werteorientierter Führung – Kloster auf Zeit» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541ab) | 1 | as enacted, 1 December 2025 |
| `541ac-reglement-cas-leadsustain/` | Reglement zum Weiterbildungsangebot «CAS in Leadership & Sustainability: Purpose in Action» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541ac) | 1 | as enacted, 1 December 2025 |
| `541b/` | Reglement über das Nachdiplomstudium Berufseinführung an der Fakultät I für Römisch-katholische Theologie an der Hochschule Luzern (SRL Nr. 541b) | 1 | one version (the oldest available), 1 January 2009 |
| `541c/` | Reglement für das Institut für Liturgiewissenschaft (SRL Nr. 541c) | 1 | as enacted, 30 September 2000 |
| `541e/` | Reglement über den Zertifikatslehrgang Lebensweltorientierte Seelsorge an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541e) | 1 | one version (the oldest available), 1 January 2009 |
| `541f/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies) «Partnerschafts-, Ehe- und Familienpastoral» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541f) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2019 |
| `541l/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies) «Religionspädagogische Leitungsfunktionen» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541l) | 1 | as enacted, 1 August 2017 |
| `541m/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies) «Katechese» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541m) | 2 | as enacted, then each consolidated version: 1 August 2017 to 1 April 2021 |
| `541n/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies) «Religionsunterricht» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541n) | 2 | as enacted, then each consolidated version: 1 August 2017 to 1 April 2021 |
| `541p-cas-kirchliche-jugendarbeit-und-gemeindeanimation/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies, CAS) «Kirchliche Jugendarbeit und Gemeindeanimation» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541p) | 2 | as enacted, then each consolidated version: 1 April 2021 to 1 February 2023 |
| `541q-cas-lebens-und-glaubensfragen-spirituell-begleiten/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies, CAS) «Lebens- und Glaubensfragen spirituell begleiten» an der Theologischen Fakultät der Universität Luzern (SRL Nr. 541q) | 2 | as enacted, then each consolidated version: 1 July 2021 to 1 June 2023 |
| `541r/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies, CAS) «Philosophy, Theology and Christianity» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541r) | 1 | as enacted, 1 June 2023 |
| `541s/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies, CAS) «Philosophy, Theology and Islam» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541s) | 1 | as enacted, 1 June 2023 |
| `541t/` | Reglement über den Zertifikatslehrgang (Certificate of Advanced Studies, CAS) «Philosophy, Theology and Judaism» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541t) | 1 | as enacted, 1 June 2023 |
| `541u-reglement-cas-refllead/` | Reglement zum Weiterbildungsangebot «CAS Reflective Leadership» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541u) | 1 | as enacted, 1 August 2024 |
| `541v-reglement-cas-leadpurp/` | Reglement zum Weiterbildungsangebot «CAS Leadership & Purpose» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541v) | 1 | as enacted, 1 August 2024 |
| `541w-reglement-mas-leadpurp/` | Reglement zum Weiterbildungsangebot «MAS Leadership & Purpose» der Theologischen Fakultät der Universität Luzern (SRL Nr. 541w) | 2 | as enacted, then each consolidated version: 1 August 2024 to 1 December 2025 |
| `541x-institutsreglement-ise/` | Organisationsreglement des Instituts für Sozialethik ISE (SRL Nr. 541x) | 1 | as enacted, 1 February 2025 |
| `541y-institutsreglement-rpi/` | Organisationsreglement des Religionspädagogischen Instituts der Theologischen Fakultät der Universität Luzern (SRL Nr. 541y) | 1 | as enacted, 1 February 2025 |
| `541z/` | Organisationsreglement des Instituts für Jüdisch-Christliche Forschung (IJCF) der Universität Luzern (SRL Nr. 541z) | 1 | as enacted, 1 August 2025 |
| `542-fakultatsreglement-ksf/` | Reglement der Kultur- und Sozialwissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 542) | 2 | oldest version available, then each consolidated version: 1 October 2013 to 1 August 2024 |
| `542f-wbr-unilu-mas-philosophy-management/` | Reglement über den Master of Advanced Studies in Philosophy + Management an der Kultur- und Sozialwissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 542f) | 4 | oldest version available, then each consolidated version: 1 February 2015 to 1 August 2024 |
| `542l/` | Reglement über den Zertifikatsstudiengang (Certificate of Advanced Studies) Philosophie + Medizin an der Kultur- und Sozialwissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 542l) | 3 | oldest version available, then each consolidated version: 1 February 2015 to 1 August 2021 |
| `542o/` | Reglement über den Master of Advanced Studies in Philosophie + Medizin an der Kultur- und Sozialwissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 542o) | 2 | as enacted, then each consolidated version: 1 February 2013 to 1 August 2018 |
| `542q-wbr-unilu-cas-lead/` | Reglement über das Weiterbildungsangebot «CAS Leadership & Excellence in Argumentation + Diskurs (LEAD)» der Universität Luzern (SRL Nr. 542q) | 2 | as enacted, then each consolidated version: 1 August 2021 to 1 August 2024 |
| `542r-or-c-cpel/` | Organisationsreglement Center for Climate Politics, Economics and Law - C‑CPEL (SRL Nr. 542r) | 1 | as enacted, 1 August 2024 |
| `542s-organisationsreglement-zrf/` | Organisationsreglement des Zentrums Religionsforschung der Kultur- und Sozialwissenschaftlichen Fakultät und der Theologischen Fakultät (SRL Nr. 542s) | 1 | as enacted, 1 June 2025 |
| `543c-reglement-cas-hsd/` | Reglement zum Weiterbildungsangebot «CAS in Hochschuldidaktik» des Zentrums Lehre der Universität Luzern (SRL Nr. 543c) | 1 | as enacted, 1 June 2025 |
| `544-schulgeldverordnung/` | Verordnung über die Schul- und Studiengelder sowie die Gebühren an kantonalen Schulen, privaten Berufsfachschulen und den Hochschulen des Kantons Luzern (SRL Nr. 544) | 14 | oldest version available, then each consolidated version: 1 August 2015 to 1 August 2026 |
| `545-fakultatsreglement-wf/` | Organisationsreglement der Wirtschaftswissenschaftlichen Fakultät der Universität Luzern (SRL Nr. 545) | 3 | as enacted, then each consolidated version: 1 July 2016 to 1 December 2025 |
| `545c-reglement-mas-in-humanitarian-leadership/` | Reglement über die Weiterbildungsangebote «MAS in Humanitarian Leadership» der Universität Luzern in Kooperation mit dem Internationalen Komitee vom Roten Kreuz, «CAS in Leading by Example», «CAS in Leading High Performing and Multidisciplinary Teams» und «CAS in Leading Complex Operations and Transformations» (SRL Nr. 545c) | 3 | as enacted, then each consolidated version: 1 January 2018 to 1 December 2024 |
| `545d/` | Reglement über die Weiterbildungsangebote «MAS in Effective Leadership» der Universität Luzern in Kooperation mit der Höheren Kaderausbildung der Armee, «CAS in Decision Making and Leadership», «CAS in Information Management and Leadership», «CAS in Human Factors and Leadership», «CAS in Decisive Leadership» und «CAS in Human Potential and Leadership» (SRL Nr. 545d) | 4 | as enacted, then each consolidated version: 1 January 2018 to 1 June 2026 |
| `545f/` | Reglement zum Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Growth and Transformation» des Instituts für Marketing and Analytics der Universität Luzern (IMA) (SRL Nr. 545f) | 2 | as enacted, then each consolidated version: 1 January 2021 to 1 February 2025 |
| `545g/` | Reglement zum Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Ecosystem Management» des Instituts für Marketing and Analytics der Universität Luzern (IMA) (SRL Nr. 545g) | 2 | as enacted, then each consolidated version: 1 April 2021 to 1 February 2025 |
| `545h/` | Reglement zum Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Innovation Implementation» des Instituts für Marketing and Analytics der Universität Luzern (IMA) (SRL Nr. 545h) | 2 | as enacted, then each consolidated version: 1 April 2021 to 1 February 2025 |
| `545j-cas-artificial-intelligence-management-for-business-value/` | Reglement über den Zertifikatslehrgang «Certificate of Advanced Studies (CAS) in Artificial Intelligence Management for Business Value an der Wirtschaftswissenschaftlichen Fakultät der Universität Luzern» (SRL Nr. 545j) | 1 | as enacted, 1 February 2023 |
| `545k-reglement-mas-moit/` | Reglement zum Weiterbildungsangebot «MAS in Management of Innovative Technologies» des Instituts für Marketing und Analytics der Universität Luzern (IMA) in Kooperation mit der Hochschule Luzern (HSLU) (SRL Nr. 545k) | 2 | as enacted, then each consolidated version: 1 August 2023 to 1 February 2025 |
| `545l-reglement-mas-modi/` | Reglement zum Weiterbildungsangebot «MAS in Management of Digital Innovation» des Instituts für Marketing und Analytics der Universität Luzern (SRL Nr. 545l) | 1 | as enacted, 1 August 2023 |
| `545m/` | Reglement über das Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Innovation Management» des Instituts für Marketing und Analytics der Universität Luzern (IMA) (SRL Nr. 545m) | 1 | as enacted, 1 February 2025 |
| `545n/` | Organisationsreglement Institut für Marketing und Analytics (IMA) (SRL Nr. 545n) | 1 | as enacted, 1 June 2026 |
| `546-fakultatsreglement-gmf/` | Reglement der Fakultät für Gesundheitswissenschaften und Medizin der Universität Luzern (SRL Nr. 546) | 4 | as enacted, then each consolidated version: 1 August 2019 to 1 August 2024 |
| `546a/` | Reglement über das Weiterbildungsangebot CAS in «Spezialisierter Palliative Care» der Universität Luzern und des Luzerner Kantonsspitals (SRL Nr. 546a) | 6 | as enacted, then each consolidated version: 1 January 2019 to 1 February 2026 |
| `546d/` | Verordnung über die Zuteilung der Studienplätze im Masterstudiengang Joint Medical Master der Universitäten Luzern und Zürich (SRL Nr. 546d) | 4 | as enacted, then each consolidated version: 1 February 2020 to 1 January 2025 |
| `546h/` | Reglement über den Zertifikatslehrgang CAS «Rehabilitationsmanagement» der Universität Luzern in Zusammenarbeit mit dem Schweizer Paraplegiker Zentrum, der Schweizerischen Unfallversicherungsanstalt und dem Luzerner Kantonsspital (SRL Nr. 546h) | 2 | as enacted, then each consolidated version: 1 August 2023 to 1 February 2025 |
| `546i-organisationsreglement-chpe/` | Organisationsreglement für das Zentrum für Gesundheit, Politik und Ökonomie bzw. Center for Health, Policy, and Economics (CHPE) (SRL Nr. 546i) | 1 | as enacted, 1 February 2025 |
| `546j/` | Organisationsreglement für das Zentrum für Rehabilitation in globalen Gesundheitssystemen (SRL Nr. 546j) | 1 | as enacted, 1 February 2025 |
| `546k/` | Organisationsreglement für das Zentrum für Hausarztmedizin und Community Care (SRL Nr. 546k) | 1 | as enacted, 1 February 2025 |
| `546l/` | Organisationsreglement für das Competence Center for Health Data Science (SRL Nr. 546l) | 1 | as enacted, 1 February 2025 |
| `546m/` | Organisationsreglement für das Competence Center for Learning Health Systems (SRL Nr. 546m) | 1 | as enacted, 1 February 2025 |
| `547-fakultatsreglement-vpf/` | Reglement der Fakultät für Verhaltenswissenschaften und Psychologie an der Universität Luzern (SRL Nr. 547) | 1 | as enacted, 1 August 2024 |
| `547c/` | Reglement zum Weiterbildungsangebot «Master of Advanced Studies (MAS) in Prozessbasierter Psychotherapie» der Universität Luzern (SRL Nr. 547c) | 1 | as enacted, 1 June 2024 |
| `547d-reglement-cas-tgt/` | Reglement zum Weiterbildungsangebot «Certificate of Advanced Studies (CAS) in Tiergestützter Therapie» der Universität Luzern (SRL Nr. 547d) | 1 | as enacted, 1 February 2025 |
| `547e/` | Organisationsreglement Institut für Verhaltensforschung (Institute for Behavioural Research) (SRL Nr. 547e) | 1 | as enacted, 1 June 2025 |
| `547f/` | Organisationsreglement Zentrum für Psychotherapie (Center for Psychotherapy) (SRL Nr. 547f) | 1 | as enacted, 1 February 2026 |
| `547g-reglement-mas-kvt/` | Reglement zum Weiterbildungsangebot «Master of Advanced Studies (MAS) in Kognitiver Verhaltenstherapie mit Schwerpunkt Kinder, Jugendliche und junge Erwachsene der Universitäten Freiburg, Bern, Luzern und Zürich» (SRL Nr. 547g) | 1 | as enacted, 1 June 2026 |
| `575a-stipendienverordnung/` | Verordnung zum Gesetz über Ausbildungsbeiträge (SRL Nr. 575a) | 9 | as enacted, then each consolidated version: 19 May 2014 to 1 June 2025 |
| `586-archivverordnung/` | Verordnung zum Archivgesetz (SRL Nr. 586) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2021 |
| `595a/` | Verordnung zum Gesetz über den Schutz der Kulturdenkmäler (SRL Nr. 595a) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2023 |
| `597-museumsreglement/` | Reglement für das Museum Luzern (SRL Nr. 597) | 2 | oldest version available, then each consolidated version: 1 July 2003 to 1 March 2025 |
| `597a/` | Reglement über die Benützung des Schlachtfeldes von Sempach (SRL Nr. 597a) | 1 | one version (the oldest available), 1 June 2013 |
| `598-kulturforderungsverordnung/` | Verordnung zum Kulturförderungsgesetz (SRL Nr. 598) | 2 | as enacted, then each consolidated version: 1 September 2011 to 1 May 2017 |
| `600a-flv/` | Verordnung zum Gesetz über die Steuerung der Finanzen und Leistungen (SRL Nr. 600a) | 12 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2026 |
| `611-fav/` | Verordnung über den Finanzausgleich (SRL Nr. 611) | 7 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `621-stv/` | Steuerverordnung (SRL Nr. 621) | 9 | oldest version available, then each consolidated version: 1 January 2016 to 1 January 2026 |
| `624-qstv/` | Verordnung über die Quellensteuer (SRL Nr. 624) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2021 |
| `665/` | Verordnung zum Bundesgesetz über die direkte Bundessteuer (SRL Nr. 665) | 1 | one version (the oldest available), 1 July 2013 |
| `666/` | Verordnung zum Bundesgesetz über die Verrechnungssteuer (SRL Nr. 666) | 2 | oldest version available, then each consolidated version: 1 July 2013 to 1 January 2023 |
| `667/` | Verordnung über die pauschale Steueranrechnung (SRL Nr. 667) | 1 | one version (the oldest available), 1 July 2013 |
| `682/` | Verordnung über den Gebührenbezug der Luzerner Polizei (SRL Nr. 682) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2027 |
| `687/` | Verordnung über den Gebührenbezug der Gemeinden (SRL Nr. 687) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `688/` | Verordnung über die Entschädigung im Steuerwesen (SRL Nr. 688) | 2 | oldest version available, then each consolidated version: 1 August 2008 to 1 January 2018 |
| `701-usv/` | Umweltschutzverordnung (SRL Nr. 701) | 7 | oldest version available, then each consolidated version: 1 October 2014 to 1 January 2025 |
| `701a/` | Smog-Verordnung (SRL Nr. 701a) | 1 | as enacted, 1 January 2010 |
| `703-kantonale-gewasserschutzverordnung-kgschv/` | Vollzugsverordnung zum Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (SRL Nr. 703) | 7 | oldest version available, then each consolidated version: 1 July 2014 to 1 December 2022 |
| `703a/` | Verordnung über die Verminderung der Phosphorbelastung der Mittellandseen durch die Landwirtschaft (SRL Nr. 703a) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2021 |
| `705/` | Verordnung über die Gebühren im Bereich des Umweltschutzes und des Gewässerschutzes (SRL Nr. 705) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `711/` | Verordnung zum Schutz des Baldegger- und des Hallwilersees und ihrer Ufer (SRL Nr. 711) | 1 | one version (the oldest available), 1 January 2014 |
| `711b/` | Verordnung zum Schutze des Mauensees und seiner Ufer (SRL Nr. 711b) | 1 | one version (the oldest available), 1 January 2014 |
| `711c/` | Verordnung zum Schutz des Sempachersees und seiner Ufer (SRL Nr. 711c) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 September 2026 |
| `711d/` | Verordnung zum Schutz des Rotsees und seiner Ufer (SRL Nr. 711d) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2020 |
| `711e/` | Verordnung zum Schutze des Soppensees und seiner Umgebung (SRL Nr. 711e) | 1 | one version (the oldest available), 1 January 2014 |
| `711g/` | Verordnung zum Schutz des Tuetensees und seiner Umgebung (SRL Nr. 711g) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2020 |
| `712/` | Verordnung zum Schutz des Steinibachriedes in der Gemeinde Horw (SRL Nr. 712) | 1 | one version (the oldest available), 1 January 2014 |
| `712a/` | Verordnung zum Schutze des Breitenacherriedes in der Gemeinde Greppen (SRL Nr. 712a) | 1 | one version (the oldest available), 1 January 2014 |
| `712b/` | Verordnung zum Schutz der Wässermatten an der Rot in den Gemeinden Grossdietwil, Altbüron und Pfaffnau (SRL Nr. 712b) | 1 | one version (the oldest available), 1 April 2014 |
| `712c/` | Verordnung zum Schutz der Moore (SRL Nr. 712c) | 1 | one version (the oldest available), 1 January 2014 |
| `712d/` | Verordnung zum Schutz des Mettlenmooses in der Gemeinde Eschenbach (SRL Nr. 712d) | 1 | one version (the oldest available), 1 January 2014 |
| `713/` | Verordnung zum Schutz der Weiherlandschaft Ostergau (SRL Nr. 713) | 1 | as enacted, 1 January 2014 |
| `713a/` | Verordnung zum Schutz der Weiherlandschaft im Uffikoner-Buchser Moos (SRL Nr. 713a) | 1 | one version (the oldest available), 1 January 2014 |
| `713b/` | Verordnung zum Schutz der Weiherlandschaft Hagimoos in den Gemeinden Ettiswil und Mauensee (SRL Nr. 713b) | 1 | one version (the oldest available), 1 January 2014 |
| `713c/` | Verordnung zum Schutze der Schrattenflue (SRL Nr. 713c) | 1 | one version (the oldest available), 1 January 2014 |
| `714a/` | Verordnung zum Schutze des Hangmoors im Gitzitobel, Gemeinde Schongau (SRL Nr. 714a) | 1 | one version (the oldest available), 1 January 2014 |
| `714b/` | Verordnung zum Schutze des Wauwilermooses (SRL Nr. 714b) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2020 |
| `714c/` | Verordnung zum Schutze der Chestenenweid in der Gemeinde Weggis (SRL Nr. 714c) | 1 | one version (the oldest available), 1 January 2014 |
| `715/` | Verordnung über den Pflanzenschutz (SRL Nr. 715) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2020 |
| `715c/` | Verordnung zum Schutz der Pilze (SRL Nr. 715c) | 1 | one version (the oldest available), 1 January 2010 |
| `716/` | Verordnung über den Pflanzenschutz im Pilatusgebiet (SRL Nr. 716) | 1 | one version (the oldest available), 1 January 2010 |
| `716a/` | Verordnung über den Pflanzenschutz im Rigigebiet (SRL Nr. 716a) | 1 | one version (the oldest available), 1 January 2010 |
| `717/` | Verordnung zum Schutz der Hecken, Feldgehölze und Uferbestockungen (SRL Nr. 717) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2020 |
| `721-fiv/` | Fischereiverordnung (SRL Nr. 721) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2021 |
| `725a-kantonale-jagdverordnung-kjsv/` | Kantonale Verordnung über die Jagd und den Schutz wildlebender Säugetiere und Vögel (SRL Nr. 725a) | 2 | oldest version available, then each consolidated version: 1 April 2014 to 1 April 2018 |
| `726/` | Reglement über die Jagdprüfung (SRL Nr. 726) | 2 | oldest version available, then each consolidated version: 1 June 2015 to 1 April 2018 |
| `727/` | Verordnung über die Abschätzung von Wildschaden (SRL Nr. 727) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 April 2018 |
| `728/` | Kantonale Tierschutzverordnung (SRL Nr. 728) | 1 | one version (the oldest available), 1 January 2014 |
| `732-perimeterverordnung-pv/` | Verordnung über Grundeigentümer-Beiträge an öffentliche Werke (SRL Nr. 732) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 June 2025 |
| `734-vivob/` | Verordnung zur Interkantonalen Vereinbarung über das öffentliche Beschaffungswesen (SRL Nr. 734) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `736b/` | Verordnung zur Einführung des am 29. September 2023 geänderten Bundesgesetzes über die Raumplanung (SRL Nr. 736b) | 1 | as enacted, 1 July 2026 |
| `739/` | Reklameverordnung (SRL Nr. 739) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 December 2025 |
| `740a/` | Verordnung zum Gesetz über den Feuerschutz (SRL Nr. 740a) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `750a-gvv/` | Gebäudeversicherungsverordnung (SRL Nr. 750a) | 6 | oldest version available, then each consolidated version: 1 June 2015 to 1 January 2026 |
| `750b/` | Verordnung über die Versicherung von Erdbebenschäden (SRL Nr. 750b) | 1 | as enacted, 1 January 1979 |
| `756-strv/` | Strassenverordnung (SRL Nr. 756) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 June 2025 |
| `758b-wegv/` | Wegverordnung (SRL Nr. 758b) | 1 | one version (the oldest available), 1 January 2014 |
| `760a-wbv/` | Wasserbauverordnung (SRL Nr. 760a) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 June 2025 |
| `764-wehrreglement/` | Reglement für die Regulierung des Vierwaldstättersees an der Reusswehranlage in Luzern (SRL Nr. 764) | 2 | as enacted, then each consolidated version: 22 November 1867 to 20 May 2011 |
| `774-kenv/` | Kantonale Energieverordnung (SRL Nr. 774) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 March 2025 |
| `775a-ovv/` | Verordnung über den öffentlichen Verkehr (SRL Nr. 775a) | 4 | oldest version available, then each consolidated version: 1 June 2013 to 1 June 2025 |
| `775b/` | Reglement für den Verkehrsverbund Luzern (SRL Nr. 775b) | 3 | as enacted, then each consolidated version: 1 January 2010 to 1 June 2022 |
| `777-strassenverkehrsverordnung/` | Verordnung zum Gesetz über die Verkehrsabgaben und den Vollzug des eidgenössischen Strassenverkehrsrechtes (SRL Nr. 777) | 8 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2027 |
| `778/` | Verordnung über den Gebührenbezug des Strassenverkehrsamtes (SRL Nr. 778) | 7 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `787/` | Verordnung über die Schifffahrt (SRL Nr. 787) | 6 | oldest version available, then each consolidated version: 1 January 2014 to 1 April 2026 |
| `787a-schiffsmelde-und-reinigungsverordnung-smrv/` | Verordnung über die Schiffsmelde- und -reinigungspflicht (SRL Nr. 787a) | 1 | as enacted, 1 April 2026 |
| `788b/` | Verordnung zum Gesetz über die Schiffssteuer (SRL Nr. 788b) | 2 | as enacted, then each consolidated version: 1 July 2003 to 1 January 2025 |
| `798/` | Verordnung über die Bezeichnung der zuständigen Behörden beim Vollzug des Bundesgesetzes über die Luftfahrt vom 21. Dezember 1948 und der eidgenössischen Vollziehungsverordnung vom 5. Juni 1950 (SRL Nr. 798) | 1 | one version (the oldest available), 1 June 2013 |
| `800b/` | Verordnung zum Spitalgesetz (SRL Nr. 800b) | 6 | as enacted, then each consolidated version: 1 January 2015 to 1 July 2022 |
| `801a/` | Vollzugsverordnung zur Durchführung des straflosen Schwangerschaftsabbruchs (SRL Nr. 801a) | 1 | one version (the oldest available), 1 January 2015 |
| `803/` | Verordnung über den schulärztlichen Dienst und die Schulzahnpflege an den kantonalen Schulen und an den Privatschulen (SRL Nr. 803) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 August 2020 |
| `804b-kantonale-sportforderungsverordnung/` | Verordnung zum Gesetz über die Förderung von Sport und Bewegung (SRL Nr. 804b) | 1 | as enacted, 1 January 2015 |
| `805-mbv/` | Medizinalberufeverordnung (SRL Nr. 805) | 11 | oldest version available, then each consolidated version: 1 January 2015 to 1 May 2025 |
| `806-gbv/` | Gesundheitsberufeverordnung (SRL Nr. 806) | 6 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2022 |
| `806a/` | Psychotherapeutenverordnung (SRL Nr. 806a) | 4 | oldest version available, then each consolidated version: 1 January 2015 to 1 July 2022 |
| `806b-nbtv/` | Verordnung über nicht bewilligungspflichtige Tätigkeiten im Gesundheitswesen (SRL Nr. 806b) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 July 2021 |
| `810a-pflegeausbildungsforderverordnung-fapv/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Förderung der Ausbildung im Bereich der Pflege (SRL Nr. 810a) | 1 | as enacted, 1 July 2024 |
| `830/` | Heilmittelverordnung (SRL Nr. 830) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2021 |
| `833/` | Kantonale Betäubungsmittelverordnung (SRL Nr. 833) | 2 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2020 |
| `834/` | Vollzugsverordnung zur eidgenössischen Chemikaliengesetzgebung (SRL Nr. 834) | 4 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2025 |
| `835-kepv/` | Kantonale Epidemienverordnung (SRL Nr. 835) | 4 | as enacted, then each consolidated version: 1 July 1995 to 1 January 2021 |
| `837/` | Vollzugsverordnung zum Bundesgesetz zum Schutz vor Passivrauchen (SRL Nr. 837) | 2 | as enacted, then each consolidated version: 1 May 2010 to 1 January 2020 |
| `838/` | Vollzugsverordnung zur eidgenössischen Verordnung über den Strahlenschutz (SRL Nr. 838) | 2 | as enacted, then each consolidated version: 1 April 2004 to 1 January 2019 |
| `840/` | Verordnung über das Bestattungswesen (SRL Nr. 840) | 1 | one version (the oldest available), 1 June 2013 |
| `843-klmv/` | Kantonale Lebensmittelverordnung (SRL Nr. 843) | 4 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2025 |
| `844/` | Kantonale Fleischhygieneverordnung (SRL Nr. 844) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2026 |
| `844a-ktabpv/` | Kantonale Tabakprodukteverordnung (SRL Nr. 844a) | 1 | as enacted, 1 May 2026 |
| `845/` | Kantonale Tierseuchenverordnung (SRL Nr. 845) | 6 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2026 |
| `849-huv/` | Verordnung über das Halten von Hunden (SRL Nr. 849) | 5 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2025 |
| `850/` | Vollzugsverordnung zum Bundesgesetz über die Arbeit in Industrie, Gewerbe und Handel (SRL Nr. 850) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2019 |
| `852/` | Vollzugsverordnung zum Bundesgesetz über die Heimarbeit (SRL Nr. 852) | 2 | oldest version available, then each consolidated version: 1 April 2004 to 1 January 2019 |
| `853/` | Vollziehungsverordnung zum Bundesgesetz über die Allgemeinverbindlicherklärung von Gesamtarbeitsverträgen vom 28. September 1956 (SRL Nr. 853) | 1 | as enacted, 1 January 2008 |
| `857/` | Vollzugsverordnung zur Bundesgesetzgebung über die in die Schweiz entsandten Arbeitnehmerinnen und Arbeitnehmer (SRL Nr. 857) | 3 | as enacted, then each consolidated version: 1 January 2008 to 1 June 2025 |
| `857a/` | Geschäftsreglement der tripartiten Arbeitsmarktkommission (SRL Nr. 857a) | 2 | as enacted, then each consolidated version: 1 June 2004 to 1 January 2019 |
| `860/` | Verordnung zum Bundesgesetz über die Arbeitsvermittlung und den Personalverleih (SRL Nr. 860) | 2 | as enacted, then each consolidated version: 1 April 2004 to 1 January 2019 |
| `863/` | Verordnung über die steuerbegünstigten Arbeitsbeschaffungsreserven (SRL Nr. 863) | 1 | as enacted, 1 July 2003 |
| `864/` | Vollzugsverordnung zum Bundesgesetz über Massnahmen zur Bekämpfung der Schwarzarbeit (SRL Nr. 864) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2019 |
| `865a/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Krankenversicherung (SRL Nr. 865a) | 3 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `865b/` | Verordnung zum Bundesgesetz über die Unfallversicherung (SRL Nr. 865b) | 2 | oldest version available, then each consolidated version: 1 June 2013 to 1 January 2019 |
| `865c-kantonale-zulassungsverordnung-vzl/` | Verordnung über die Zulassung von Leistungserbringern zur Tätigkeit zulasten der obligatorischen Krankenpflegeversicherung (SRL Nr. 865c) | 5 | as enacted, then each consolidated version: 15 July 2013 to 1 January 2026 |
| `866a-pramienverbilligungsverordnung/` | Verordnung zum Gesetz über die Verbilligung von Prämien der Krankenversicherung (SRL Nr. 866a) | 12 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `867a-bpv/` | Verordnung zum Betreuungs- und Pflegegesetz (SRL Nr. 867a) | 8 | oldest version available, then each consolidated version: 1 June 2014 to 1 January 2026 |
| `869/` | Verordnung über das Schiedsverfahren nach den Bestimmungen des eidgenössischen Sozialversicherungsrechts (SRL Nr. 869) | 1 | one version (the oldest available), 1 June 2013 |
| `880a/` | Verordnung über die Bestellung des Verwaltungsrates des Sozialversicherungszentrums (SRL Nr. 880a) | 1 | as enacted, 20 November 2018 |
| `880b/` | Geschäftsreglement des Sozialversicherungszentrums (SRL Nr. 880b) | 3 | as enacted, then each consolidated version: 1 January 2019 to 20 May 2025 |
| `880c/` | Personalreglement des Sozialversicherungszentrums (SRL Nr. 880c) | 1 | as enacted, 1 January 2019 |
| `880d/` | Reglement über Organisation, Aufgaben, Kompetenzen und Verantwortlichkeiten der Kommissionen des Verwaltungsrates des Sozialversicherungszentrums (WAS) (SRL Nr. 880d) | 3 | as enacted, then each consolidated version: 1 January 2019 to 20 May 2025 |
| `880e-personalkommissionsreglement/` | Reglement über die paritätische Personalkommission des Sozialversicherungszentrums WAS (SRL Nr. 880e) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 July 2022 |
| `880f-anlagereglement-ak/` | Reglement über die Anlagen von finanziellen Mitteln der Ausgleichskasse Luzern (SRL Nr. 880f) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 March 2026 |
| `880g-anlagereglement-fak/` | Reglement über die Anlagen von finanziellen Mitteln der Familienausgleichskasse Luzern (SRL Nr. 880g) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 March 2026 |
| `880h-organisationsreglement-alk/` | Reglement über die Organisation der Arbeitslosenkasse des Kantons Luzern (SRL Nr. 880h) | 1 | as enacted, 1 July 2022 |
| `881a/` | Verordnung über die Ergänzungsleistungen zur AHV/IV (SRL Nr. 881a) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `881b/` | Verordnung über die Vergütung von Krankheits- und Behinderungskosten bei den Ergänzungsleistungen (SRL Nr. 881b) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2025 |
| `885a-kantonale-familienzulagenverordnung-fzv/` | Verordnung zum Kantonalen Familienzulagengesetz (SRL Nr. 885a) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2019 |
| `886/` | Vollziehungsverordnung zum Bundesgesetz über die Familienzulagen für landwirtschaftliche Arbeitnehmer und Bergbauern (SRL Nr. 886) | 1 | one version (the oldest available), 1 January 1967 |
| `887a-kinderbetreuungsverordnung-kibev/` | Verordnung zum Gesetz über die familienergänzende Kinderbetreuung (SRL Nr. 887a) | 2 | as enacted, then each consolidated version: 1 January 2026 to 1 August 2026 |
| `890a/` | Verordnung über die Arbeitslosenversicherung und den Arbeitslosenhilfsfonds (SRL Nr. 890a) | 8 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2025 |
| `890b/` | Geschäftsreglement der tripartiten Kommission (SRL Nr. 890b) | 3 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2023 |
| `892a-shv/` | Sozialhilfeverordnung (SRL Nr. 892a) | 6 | as enacted, then each consolidated version: 1 January 2016 to 1 January 2024 |
| `892b-kasylv/` | Kantonale Asylverordnung (SRL Nr. 892b) | 9 | as enacted, then each consolidated version: 1 January 2016 to 1 January 2026 |
| `893/` | Reglement über den Unterstützungsfonds für Lungen- und Aidskranke (SRL Nr. 893) | 1 | as enacted, 1 July 2007 |
| `893d/` | Verordnung zum Einführungsgesetz zum Opferhilfegesetz des Bundes (SRL Nr. 893d) | 1 | as enacted, 1 January 2010 |
| `894b-sev/` | Verordnung zum Gesetz über soziale Einrichtungen (SRL Nr. 894b) | 5 | oldest version available, then each consolidated version: 1 January 2015 to 1 January 2024 |
| `897a-verordnung-i-zum-gesetz-uber-wohnbau-und-eigentumsforderung/` | Verordnung über die Förderung des preisgünstigen Wohnungsbaus, der Erneuerung bestehender Wohnungen und des Erwerbs von Wohnungs- und Hauseigentum (SRL Nr. 897a) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 March 2017 |
| `897b-vwbv/` | Verordnung über die Verbesserung der Wohnverhältnisse in Berggebieten (SRL Nr. 897b) | 1 | as enacted, 1 January 2008 |
| `897c-verordnung-iii-zum-gesetz-uber-wohnbau-und-eigentumsforderung/` | Verordnung über die Förderung des Erwerbs und der Erschliessung von Land für den Wohnungsbau (SRL Nr. 897c) | 1 | one version (the oldest available), 1 July 2007 |
| `897d/` | Vollziehungsverordnung zum Dekret über Massnahmen zur Förderung des sozialen Wohnungsbaues (SRL Nr. 897d) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 March 2017 |
| `897f-allgemeiner-wohnungsbau-und-bau-von-alterswohnungen/` | Vollziehungsverordnung zum Dekret über die zusätzliche Förderung des Wohnungsbaues (SRL Nr. 897f) | 1 | one version (the oldest available), 1 January 2008 |
| `897h/` | Vollziehungsverordnung zum Dekret über Massnahmen zur Förderung des Wohnungsbaues (SRL Nr. 897h) | 1 | one version (the oldest available), 1 January 2010 |
| `897k/` | Vollziehungsverordnung zum Dekret über Massnahmen zur Förderung des Wohnungsbaues (SRL Nr. 897k) | 1 | one version (the oldest available), 1 January 2010 |
| `900a-starev/` | Verordnung zum Gesetz über die Standortförderung und die Regionalpolitik (SRL Nr. 900a) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 October 2026 |
| `900b-kantonale-hartefallverordnung-covid-19/` | Verordnung über Härtefallmassnahmen für Luzerner Unternehmen im Zusammenhang mit der Covid-19-Epidemie (SRL Nr. 900b) | 12 | as enacted, then each consolidated version: 1 December 2020 to 1 August 2025 |
| `903-klwv/` | Kantonale Landwirtschaftsverordnung (SRL Nr. 903) | 1 | one version (the oldest available), 1 June 2015 |
| `903a/` | Verordnung über die Gebühren für Beratungen und Weiterbildungskurse in der Landwirtschaft (SRL Nr. 903a) | 1 | one version (the oldest available), 1 February 2015 |
| `903b/` | Reglement über die milchwirtschaftlichen Fachschulen (SRL Nr. 903b) | 1 | one version (the oldest available), 1 August 2006 |
| `916/` | Verordnung über den Gebirgshilfefonds für Strukturverbesserungen (SRL Nr. 916) | 1 | one version (the oldest available), 1 January 2008 |
| `917/` | Verordnung über die kontrollierte Ursprungsbezeichnung für Weine (SRL Nr. 917) | 2 | oldest version available, then each consolidated version: 1 January 2015 to 1 June 2025 |
| `938a/` | Vollziehungsverordnung zum Gesetz über die Viehversicherung (SRL Nr. 938a) | 1 | one version (the oldest available), 1 July 2003 |
| `946-kwav/` | Kantonale Waldverordnung (SRL Nr. 946) | 3 | oldest version available, then each consolidated version: 1 March 2014 to 1 January 2020 |
| `950/` | Verordnung zum Bundesgesetz über das Messwesen (SRL Nr. 950) | 6 | oldest version available, then each consolidated version: 1 July 2014 to 1 January 2026 |
| `956-gpv/` | Gewerbepolizeiverordnung (SRL Nr. 956) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 July 2020 |
| `958a-sammelverordnung/` | Verordnung über das Sammeln von Gaben und den Verkauf von Abzeichen (SRL Nr. 958a) | 3 | as enacted, then each consolidated version: 1 January 2010 to 1 April 2025 |
| `976-wavo/` | Vollzugsverordnung zum Bundesgesetz über Waffen, Waffenzubehör und Munition (SRL Nr. 976) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2020 |
| `977/` | Vollzugsverordnung zur eidgenössischen Sprengstoffgesetzgebung (SRL Nr. 977) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 May 2023 |
| `981-gastgewerbeverordnung-gav/` | Verordnung zum Gesetz über das Gastgewerbe, den Handel mit alkoholischen Getränken und die Fasnacht (SRL Nr. 981) | 3 | oldest version available, then each consolidated version: 1 January 2014 to 1 July 2018 |
| `993-kgsv/` | Kantonale Geldspielverordnung (SRL Nr. 993) | 3 | oldest version available, then each consolidated version: 1 March 2013 to 1 November 2022 |
| `994-lotteriegelderverordnung/` | Verordnung über die Verwendung der Reingewinne von Lotterien, Sportwetten und Geschicklichkeitsspielen (SRL Nr. 994) | 2 | oldest version available, then each consolidated version: 1 July 2014 to 1 July 2020 |

## Source

The SRL Nr. (systematic collection) of the canton, published by the canton at <https://srl.lu.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (G). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (G), with an e-mail address that cannot exist (`<act key>@srl.lu.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
