# Glarus: law history in git

The law of the canton of Glarus (Kanton Glarus, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-gl/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

319 acts with 950 versions so far: the cantonal constitution, the cantonal laws (Gesetze) in force and 232 Verordnungen and Reglemente in force, in the order of the systematic collection, added in parts. Other decrees and decisions, intercantonal agreements and repealed acts are not included yet.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `i-a-1-1/` | Verfassung des Kantons Glarus (GS I A/1/1) | 9 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `i-a-3-1/` | Gesetz betreffend die Feier der Näfelser Fahrt (GS I A/3/1) | 1 | as enacted, 24 May 1835 |
| `i-c-12-2-kantonales-burgerrechtsgesetz-kbug/` | Gesetz über das Kantons- und Gemeindebürgerrecht (GS I C/12/2) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `i-c-21-2-einfuhrungsgesetz-zum-registerharmonisierungsgesetz-eg-rhg/` | Einführungsgesetz zum Bundesgesetz über die Harmonisierung der Einwohnerregister und anderer amtlicher Personenregister (GS I C/21/2) | 3 | as enacted, then each consolidated version: 3 May 2009 to 1 January 2023 |
| `i-c-23-2/` | Einführungsgesetz zum Bundesgesetz über die Ausländerinnen und Ausländer und zum Asylgesetz (GS I C/23/2) | 2 | as enacted, then each consolidated version: 1 January 2009 to 1 September 2014 |
| `i-d-22-2-gpr/` | Gesetz über die politischen Rechte (GS I D/22/2) | 4 | oldest version available, then each consolidated version: 1 May 2011 to 1 January 2026 |
| `i-d-23-1/` | Gesetz über die Eidesformeln (GS I D/23/1) | 2 | oldest version available, then each consolidated version: 1 July 2002 to 1 September 2014 |
| `i-d-24-1-pubg/` | Publikationsgesetz (GS I D/24/1) | 3 | as enacted, then each consolidated version: 6 May 1973 to 1 January 2021 |
| `i-e-1-1-kantonales-gleichstellungsgesetz/` | Einführungsgesetz zum Bundesgesetz über die Gleichstellung von Frau und Mann (GS I E/1/1) | 4 | oldest version available, then each consolidated version: 7 May 2006 to 1 July 2022 |
| `i-f-1-idag/` | Gesetz über die Information der Öffentlichkeit, den Datenschutz und das Archivwesen (GS I F/1) | 4 | oldest version available, then each consolidated version: 4 May 2008 to 1 January 2023 |
| `ii-a-3-2-regierungs-und-verwaltungsorganisationsgesetz-rvog/` | Gesetz über die Organisation des Regierungsrates und der Verwaltung (GS II A/3/2) | 5 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2023 |
| `ii-a-5-1/` | Gesetz über die kantonale Schatzungskommission (GS II A/5/1) | 1 | one version (the oldest available), 1 October 1987 |
| `ii-a-6-1-personalgesetz-pg/` | Gesetz über das Personalwesen (GS II A/6/1) | 8 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `ii-e-2-gg/` | Gemeindegesetz (GS II E/2) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `ii-f-2-staatshaftungsgesetz/` | Gesetz über die Haftung der Gemeinwesen und ihrer Amtsträger (GS II F/2) | 3 | oldest version available, then each consolidated version: 1 January 2009 to 1 September 2014 |
| `ii-h-1-dvg/` | Gesetz über die digitale Verwaltung (GS II H/1) | 2 | as enacted, then each consolidated version: 1 January 2023 to 1 January 2026 |
| `iii-a-2-gog/` | Gerichtsorganisationsgesetz (GS III A/2) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 July 2022 |
| `iii-b-1-1-einfuhrungsgesetz-zum-zivilgesetzbuch-eg-zgb/` | Gesetz über die Einführung des Schweizerischen Zivilgesetzbuches im Kanton Glarus (GS III B/1/1) | 10 | oldest version available, then each consolidated version: 1 January 2013 to 1 July 2025 |
| `iii-b-1-2/` | Gesetz über die Freihaltung des Geländes zur Ausübung des Skisportes (GS III B/1/2) | 1 | one version (the oldest available), 7 May 2006 |
| `iii-b-1-4/` | Vollziehungsgesetz zum Bundesgesetz über den Erwerb von Grundstücken durch Personen im Ausland (GS III B/1/4) | 3 | oldest version available, then each consolidated version: 1 December 2009 to 1 January 2026 |
| `iii-b-2-1-einfuhrungsgesetz-zum-obligationenrecht-eg-or/` | Gesetz über die Einführung des Schweizerischen Obligationenrechtes (Zivilgesetzbuch V. Teil) im Kanton Glarus (GS III B/2/1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2022 |
| `iii-b-3-1-beurkundungsgesetz/` | Gesetz über Beurkundung und Beglaubigung (GS III B/3/1) | 4 | as enacted, then each consolidated version: 1 January 2008 to 1 July 2025 |
| `iii-d-1-eg-schkg/` | Gesetz über die Einführung des Bundesgesetzes über Schuldbetreibung und Konkurs (GS III D/1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2014 |
| `iii-e-1-einfuhrungsgesetz-zum-schweizerischen-strafgesetzbuch-eg-stgb/` | Gesetz über die Einführung des Schweizerischen Strafgesetzbuches im Kanton Glarus (GS III E/1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2022 |
| `iii-g-1-verwaltungsrechtspflegegesetz/` | Gesetz über die Verwaltungsrechtspflege (GS III G/1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `iii-i-1/` | Anwaltsgesetz des Kantons Glarus (GS III I/1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `iv-b-1-3-bildungsgesetz-big/` | Gesetz über Schule und Bildung (GS IV B/1/3) | 9 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2026 |
| `iv-b-1-13-kibg/` | Kinderbetreuungsgesetz (GS IV B/1/13) | 1 | as enacted, 1 January 2023 |
| `iv-b-6-1-musikschulgesetz-msg/` | Gesetz über die musikalische Bildung (GS IV B/6/1) | 2 | as enacted, then each consolidated version: 11 August 2008 to 1 August 2022 |
| `iv-b-51-1-eg-bbg/` | Einführungsgesetz zum Bundesgesetz über die Berufsbildung (GS IV B/51/1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2017 |
| `iv-d-1-1/` | Gesetz über die Förderung von Turnen und Sport (GS IV D/1/1) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2021 |
| `iv-e-1-1-stipendiengesetz/` | Gesetz über die Ausbildungs- und Schulgeldbeiträge (GS IV E/1/1) | 2 | as enacted, then each consolidated version: 1 August 2012 to 1 August 2026 |
| `iv-f-1/` | Gesetz über die Förderung des kulturellen Lebens (GS IV F/1) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2021 |
| `iv-g-1-1/` | Gesetz über den Natur- und Heimatschutz (GS IV G/1/1) | 4 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2023 |
| `iv-g-3-2-kantonales-tierschutz-und-tierseuchengesetz-eg-zum-tschg-und-tsg/` | Einführungsgesetz zum Tierschutzgesetz und zum Tierseuchengesetz (GS IV G/3/2) | 4 | as enacted, then each consolidated version: 1 July 2012 to 1 January 2026 |
| `ix-a-4-standortforderungsgesetz/` | Gesetz über die Standortförderung (GS IX A/4) | 4 | oldest version available, then each consolidated version: 1 July 2011 to 1 July 2023 |
| `ix-b-21-1-ruhetagsgesetz/` | Gesetz über die öffentlichen Ruhetage (GS IX B/21/1) | 4 | as enacted, then each consolidated version: 6 May 2012 to 1 July 2019 |
| `ix-b-22-1-gastgewerbegesetz-ggg/` | Gesetz über das Gastgewerbe und den Handel mit alkoholischen Getränken (GS IX B/22/1) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 February 2023 |
| `ix-b-24-1-kgg/` | Kantonales Geldspielgesetz (GS IX B/24/1) | 5 | oldest version available, then each consolidated version: 1 January 2009 to 5 September 2021 |
| `ix-b-25-1/` | Gesetz über die Handels- und Gewerbetätigkeiten (GS IX B/25/1) | 3 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2027 |
| `ix-b-31-1-kantonalbankgesetz/` | Gesetz über die Glarner Kantonalbank (GS IX B/31/1) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2021 |
| `ix-b-42-1/` | Gesetz über den Bergbau (GS IX B/42/1) | 1 | as enacted, 7 May 1893 |
| `ix-c-1-1-tourismusentwicklungsgesetz-teg/` | Gesetz zur Entwicklung des Tourismus (GS IX C/1/1) | 4 | oldest version available, then each consolidated version: 1 July 2011 to 7 May 2023 |
| `ix-d-1-1-eg-lwg/` | Einführungsgesetz zu den Bundesgesetzen über die Landwirtschaft, über das bäuerliche Bodenrecht und über die landwirtschaftliche Pacht (GS IX D/1/1) | 4 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2027 |
| `ix-d-631-5/` | Gesetz über die Bienenzucht und Bienenhaltung (GS IX D/631/5) | 1 | as enacted, 1 May 1977 |
| `ix-e-1-1/` | Einführungsgesetz zum Bundesgesetz über den Wald (GS IX E/1/1) | 3 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2018 |
| `v-a-11-1-polg/` | Polizeigesetz (GS V A/11/1) | 7 | oldest version available, then each consolidated version: 1 January 2013 to 1 October 2025 |
| `v-c-1-1-brandschutzgesetz/` | Gesetz über den Brandschutz und die Feuerwehr (GS V C/1/1) | 5 | oldest version available, then each consolidated version: 1 July 2011 to 1 December 2023 |
| `v-d-1-1-sachversicherungsgesetz-sachvg/` | Gesetz über die Kantonale Sachversicherung Glarus (GS V D/1/1) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 March 2024 |
| `v-f-1/` | Gesetz über den Zivilschutz (GS V F/1) | 4 | oldest version available, then each consolidated version: 1 July 2011 to 16 December 2020 |
| `v-g-1-bevolkerungsschutzgesetz-bevg-gl/` | Gesetz über den Bevölkerungsschutz (GS V G/1) | 3 | as enacted, then each consolidated version: 1 September 2013 to 1 September 2014 |
| `v-h-1-kantonales-landesversorgungsgesetz-lvg/` | Einführungsgesetz zum Bundesgesetz über die wirtschaftliche Landesversorgung (GS V H/1) | 1 | as enacted, 1 September 2013 |
| `vi-a-1-2-finanzhaushaltgesetz-fhg/` | Gesetz über den Finanzhaushalt des Kantons Glarus und seiner Gemeinden (GS VI A/1/2) | 6 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `vi-a-2-1-finanzausgleichsgesetz-fag/` | Gesetz über den Finanzausgleich zwischen dem Kanton und den Gemeinden (GS VI A/2/1) | 6 | as enacted, then each consolidated version: 1 January 2011 to 1 July 2026 |
| `vi-c-1-1-stg/` | Steuergesetz (GS VI C/1/1) | 13 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `vi-e-31-1-kantonales-fischereigesetz/` | Einführungsgesetz zum Bundesgesetz über die Fischerei (GS VI E/31/1) | 4 | oldest version available, then each consolidated version: 1 July 2010 to 1 January 2027 |
| `vi-e-211-1-kantonales-jagdgesetz/` | Gesetz über die Jagd und den Schutz wildlebender Säugetiere und Vögel (GS VI E/211/1) | 4 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2027 |
| `vii-a-2-1-eg-geoinformationsgesetz-eg-geoig/` | Einführungsgesetz zum Geoinformationsgesetz (GS VII A/2/1) | 3 | as enacted, then each consolidated version: 1 September 2012 to 1 January 2023 |
| `vii-b-1-1-rbg/` | Raumentwicklungs- und Baugesetz (GS VII B/1/1) | 5 | as enacted, then each consolidated version: 1 July 2011 to 1 January 2026 |
| `vii-b-6-1-walenseegesetz/` | Gesetz über die öffentlich-rechtlichen Verhältnisse am Walensee (GS VII B/6/1) | 1 | one version (the oldest available), 7 May 2006 |
| `vii-c-11-1/` | Strassengesetz (GS VII C/11/1) | 2 | oldest version available, then each consolidated version: 1 July 2011 to 1 July 2018 |
| `vii-c-11-8-kvwg/` | Kantonales Veloweggesetz (GS VII C/11/8) | 2 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2025 |
| `vii-d-3-1/` | Gesetz über die nicht eidgenössisch konzessionierten Transportanlagen (GS VII D/3/1) | 1 | one version (the oldest available), 7 May 2006 |
| `vii-d-4-1-kantonales-schifffahrtsgesetz/` | Einführungsgesetz zum Bundesgesetz über die Binnenschifffahrt (GS VII D/4/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-d-6-1-ovg/` | Gesetz über den öffentlichen Verkehr (GS VII D/6/1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `vii-d-11-1-eg-svg/` | Einführungsgesetz zum Bundesgesetz über den Strassenverkehr (GS VII D/11/1) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `vii-d-11-3/` | Gesetz über die Verwendung von Motorfahrzeugen ausserhalb der öffentlichen Strassen und Wege (GS VII D/11/3) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-d-43-1/` | Gesetz über die Besteuerung der Wasserfahrzeuge (GS VII D/43/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-e-1-1-eng/` | Energiegesetz (GS VII E/1/1) | 5 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2023 |
| `viii-a-1-1-gesundheitsgesetz-gesg/` | Gesetz über das Gesundheitswesen (GS VIII A/1/1) | 9 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `viii-a-1-5-pbg/` | Pflege- und Betreuungsgesetz (GS VIII A/1/5) | 1 | as enacted, 1 January 2023 |
| `viii-b-1-3-kantonales-umweltschutzgesetz-eg-usg/` | Einführungsgesetz zum Bundesgesetz über den Umweltschutz (GS VIII B/1/3) | 3 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2024 |
| `viii-b-21-1-einfuhrungsgesetz-zum-gewasserschutzgesetz-eg-gschg/` | Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (GS VIII B/21/1) | 3 | oldest version available, then each consolidated version: 1 July 2011 to 1 January 2027 |
| `viii-c-13-1/` | Gesetz über die Einigungsstelle (GS VIII C/13/1) | 1 | one version (the oldest available), 1 October 1987 |
| `viii-c-21-1/` | Einführungsgesetz zu den bundesrechtlichen Bestimmungen in den Bereichen Arbeit, Unfallverhütung und Sicherheit von technischen Einrichtungen und Geräten (GS VIII C/21/1) | 1 | one version (the oldest available), 1 July 2011 |
| `viii-c-33-2/` | Gesetz über die steuerbegünstigten Arbeitsbeschaffungsreserven (GS VIII C/33/2) | 1 | one version (the oldest available), 7 May 2006 |
| `viii-d-3-1/` | Einführungsgesetz zum Bundesgesetz über die Militärversicherung (GS VIII D/3/1) | 2 | as enacted, then each consolidated version: 1 May 2005 to 1 September 2014 |
| `viii-d-5-1/` | Einführungsgesetz zum Bundesgesetz über Familienzulagen (GS VIII D/5/1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2016 |
| `viii-d-6-1/` | Einführungsgesetz zum Bundesgesetz über die Arbeitsvermittlung und den Personalverleih (GS VIII D/6/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-d-6-4/` | Einführungsgesetz zum Bundesgesetz über die obligatorische Arbeitslosenversicherung und die Insolvenzentschädigung (GS VIII D/6/4) | 3 | oldest version available, then each consolidated version: 3 May 2009 to 1 July 2023 |
| `viii-d-7-1-geel/` | Gesetz über Erwerbsersatzleistungen für einkommensschwache Eltern (GS VIII D/7/1) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 July 2023 |
| `viii-d-12-1/` | Einführungsgesetz zum Bundesgesetz über die Invalidenversicherung (GS VIII D/12/1) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2023 |
| `viii-d-13-1/` | Einführungsgesetz zum Bundesgesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (GS VIII D/13/1) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2023 |
| `viii-d-21-1-eg-kvg/` | Einführungsgesetz zum Bundesgesetz über die Krankenversicherung (GS VIII D/21/1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2028 |
| `viii-d-22-1-eg-uvg/` | Einführungsgesetz zum Bundesgesetz über die Unfallversicherung (GS VIII D/22/1) | 2 | as enacted, then each consolidated version: 3 May 2009 to 1 September 2014 |
| `viii-d-112-1/` | Einführungsgesetz zum Bundesgesetz über die Alters- und Hinterlassenenversicherung (GS VIII D/112/1) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 September 2014 |
| `viii-e-21-3-sozialhilfegesetz-shg/` | Gesetz über die öffentliche Sozialhilfe (GS VIII E/21/3) | 7 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `i-c-3-2/` | Verordnung über den Vollzug des Bundesgesetzes über die Ausweise für Schweizer Staatsangehörige (GS I C/3/2) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `i-c-12-4-kantonale-burgerrechtsverordnung-kbuv/` | Verordnung zum Kantonalen Bürgerrechtsgesetz (GS I C/12/4) | 1 | as enacted, 1 January 2018 |
| `i-c-21-3/` | Verordnung zum Betrieb einer kantonalen Datenplattform gemäss dem Einführungsgesetz zum Registerharmonisierungsgesetz (GS I C/21/3) | 2 | as enacted, then each consolidated version: 1 September 2014 to 1 October 2015 |
| `i-c-23-3-vo-eg-aug-asylg/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Ausländerinnen und Ausländer und zum Asylgesetz (GS I C/23/3) | 4 | oldest version available, then each consolidated version: 1 February 2011 to 1 March 2019 |
| `i-d-22-3-vpr/` | Verordnung über die politischen Rechte (GS I D/22/3) | 3 | as enacted, then each consolidated version: 1 January 2018 to 1 January 2026 |
| `i-d-24-2-pubv/` | Publikationsverordnung (GS I D/24/2) | 3 | as enacted, then each consolidated version: 25 September 1974 to 1 January 2021 |
| `i-e-1-2/` | Verordnung zum kantonalen Gleichstellungsgesetz (GS I E/1/2) | 4 | oldest version available, then each consolidated version: 28 September 2005 to 1 July 2022 |
| `i-f-2-vidag/` | Verordnung zum Gesetz über die Information der Öffentlichkeit, den Datenschutz und das Archivwesen (GS I F/2) | 4 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2023 |
| `ii-a-2-3-lrv/` | Landratsverordnung (GS II A/2/3) | 6 | oldest version available, then each consolidated version: 30 June 2010 to 1 July 2026 |
| `ii-a-3-3-regierungs-und-verwaltungsorganisationsverordnung-rvov/` | Verordnung über die Organisation des Regierungsrates und der Verwaltung (GS II A/3/3) | 24 | oldest version available, then each consolidated version: 1 January 2013 to 1 May 2025 |
| `ii-a-6-2-pv/` | Personalverordnung (GS II A/6/2) | 12 | oldest version available, then each consolidated version: 1 January 2013 to 1 July 2026 |
| `ii-a-8-1-rathausplatzreglement-rpr/` | Reglement über die Nutzung des Rathausplatzes (GS II A/8/1) | 1 | as enacted, 1 September 2026 |
| `ii-c-1-1-lohnverordnung-lohnv/` | Verordnung über die Entlöhnung der Behördenmitglieder sowie des Staats- und Lehrpersonals (GS II C/1/1) | 10 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `ii-c-4-3-lehrpersoneneinreihungsverordnung-lpev/` | Verordnung über die Einreihung der Lehrpersonen in die Lohnbänder (GS II C/4/3) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 August 2026 |
| `ii-d-1-1/` | Verordnung über die Alterssicherung der Regierungsräte, der Gerichtspräsidenten und des Staatsanwaltes (GS II D/1/1) | 1 | one version (the oldest available), 2 December 1987 |
| `ii-d-1-2/` | Verordnung über die Alterssicherung der Behördenmitglieder (GS II D/1/2) | 1 | as enacted, 1 January 2002 |
| `ii-d-2-2/` | Verordnung über die Teuerungszulagen für die Rentner und Sparmitglieder der Pensionskasse (GS II D/2/2) | 2 | as enacted, then each consolidated version: 1 January 2001 to 1 September 2014 |
| `ii-e-2-1-korpv/` | Korporationsverordnung (GS II E/2/1) | 3 | as enacted, then each consolidated version: 1 July 2017 to 1 January 2023 |
| `ii-g-2-3-v-eg-ivob/` | Verordnung zum Einführungsgesetz zur Interkantonalen Vereinbarung über das öffentliche Beschaffungswesen (GS II G/2/3) | 1 | as enacted, 1 March 2024 |
| `ii-h-2-informatikverordnung-itv/` | Verordnung über die Informatik (GS II H/2) | 1 | as enacted, 1 January 2023 |
| `ii-h-3/` | Verordnung zur Förderung der digitalen Transformation (GS II H/3) | 1 | as enacted, 1 September 2024 |
| `ii-h-4-behordenportalverordnung-behopv/` | Verordnung über das Behördenportal (GS II H/4) | 1 | as enacted, 1 September 2024 |
| `ii-h-5-evrv/` | Verordnung über das elektronische Verwaltungsverfahren (GS II H/5) | 3 | as enacted, then each consolidated version: 1 September 2024 to 1 September 2026 |
| `iii-a-3-gerichtsverwaltungsreglement/` | Reglement über die Gerichtsverwaltung des Kantons Glarus (GS III A/3) | 2 | as enacted, then each consolidated version: 1 June 2005 to 1 July 2018 |
| `iii-a-3-2-orog/` | Reglement über die Organisation des Obergerichts des Kantons Glarus (GS III A/3/2) | 1 | as enacted, 1 July 2022 |
| `iii-a-3-3-orvg/` | Reglement über die Organisation des Verwaltungsgerichts des Kantons Glarus (GS III A/3/3) | 1 | as enacted, 1 July 2022 |
| `iii-a-3-4-orkg/` | Reglement über die Organisation des Kantonsgerichts des Kantons Glarus (GS III A/3/4) | 1 | as enacted, 1 July 2022 |
| `iii-a-5-zivil-und-strafprozesskostenverordnung/` | Verordnung zu den Kosten im Zivil- und Strafprozess (GS III A/5) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `iii-b-1-5-vo-eg-zgb-und-zum-vollziehungsgesetz-zum-bundesgesetz-uber-den-erwerb-von-grundstucken-durch-personen-im-ausland/` | Verordnung zum Einführungsgesetz zum Zivilgesetzbuch und zum Vollziehungsgesetz zum Bundesgesetz über den Erwerb von Grundstücken durch Personen im Ausland (GS III B/1/5) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 April 2025 |
| `iii-b-1-6-vo-kesb/` | Verordnung über die Kindes- und Erwachsenenschutzbehörde (GS III B/1/6) | 5 | as enacted, then each consolidated version: 1 January 2013 to 1 September 2024 |
| `iii-b-1-8-electronic-monitoring-verordnung-emv/` | Verordnung über die elektronische Überwachung zum Schutz gewaltbetroffener Personen (GS III B/1/8) | 1 | as enacted, 1 January 2022 |
| `iii-b-2-4/` | Verordnung zum Einführungsgesetz zum Obligationenrecht und zum Einführungsgesetz zur Schweizerischen Zivilprozessordnung (GS III B/2/4) | 1 | as enacted, 1 January 2011 |
| `iii-b-3-2/` | Verordnung über Beurkundung und Beglaubigung mit Gebührentarif (GS III B/3/2) | 1 | as enacted, 1 January 2009 |
| `iii-b-3-3/` | Reglement über die Eignungsprüfung über Beurkundung und Beglaubigung (GS III B/3/3) | 1 | as enacted, 1 February 2008 |
| `iii-b-4-1-stiftungsv/` | Stiftungsverordnung (GS III B/4/1) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 April 2022 |
| `iii-b-4-2-1-gebr-atioz/` | Gebührenreglement der BVG- und Stiftungsaufsicht Tessin, Ostschweiz und Zürich (GS III B/4/2/1) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `iii-b-5-2-kantonale-zivilstandsverordnung/` | Verordnung über den Vollzug der eidgenössischen Zivilstandsverordnung (GS III B/5/2) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2019 |
| `iii-b-6-4/` | Verordnung über die Führung des Grundbuchs mittels Informatik (GS III B/6/4) | 3 | oldest version available, then each consolidated version: 7 May 2006 to 1 March 2025 |
| `iii-b-7-1-gebuhrentarif-zgb-gebt-zgb/` | Verordnung über die Gebühren im Zivilrecht (GS III B/7/1) | 7 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `iii-d-1-1/` | Verordnung zum Gesetz über die Einführung des Bundesgesetzes über Schuldbetreibung und Konkurs (GS III D/1/1) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2026 |
| `iii-f-1-1/` | Kantonale Ordnungsbussenverordnung (GS III F/1/1) | 7 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2021 |
| `iii-f-1-2-vobg/` | Verordnung zur Ordnungsbussengesetzgebung des Bundes (GS III F/1/2) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 January 2024 |
| `iii-f-2/` | Verordnung über die Geschäftsführung und Organisation der Staats- und Jugendanwaltschaft (GS III F/2) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 July 2026 |
| `iii-f-3-gefangnisverordnung/` | Verordnung über das Kantonsgefängnis vom 14. Mai 1996 (GS III F/3) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2023 |
| `iii-f-5-bewahrungshilfeverordnung/` | Verordnung über die Bewährungshilfe (GS III F/5) | 3 | as enacted, then each consolidated version: 1 January 2007 to 1 March 2023 |
| `iii-f-6-kantonale-opferhilfeverordnung/` | Verordnung zum Bundesgesetz über die Hilfe an Opfer (GS III F/6) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 September 2014 |
| `iii-f-7-vsmo/` | Verordnung über den Vollzug in den Bereichen Strafprozess, Straf- und Massnahmenvollzug und Opferhilfe (GS III F/7) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 March 2023 |
| `iii-g-2-kostenverordnung/` | Verordnung über amtliche Kosten im Verwaltungsverfahren und in der Verwaltungsrechtspflege (GS III G/2) | 1 | as enacted, 1 October 1987 |
| `iii-i-3/` | Reglement über die Anwaltsprüfung (GS III I/3) | 1 | one version (the oldest available), 1 February 2008 |
| `iv-a-21-2/` | Geschäftsreglement der Synode (GS IV A/21/2) | 5 | as enacted, then each consolidated version: 1 January 1996 to 6 June 2024 |
| `iv-b-1-4-schulorganisationsverordnung-sov/` | Verordnung über die Organisation der kantonalen Schulen (GS IV B/1/4) | 2 | as enacted, then each consolidated version: 1 August 2019 to 1 August 2026 |
| `iv-b-1-5-bildungsangebotsverordnung-bav/` | Verordnung über das kantonale Bildungsangebot (GS IV B/1/5) | 2 | as enacted, then each consolidated version: 1 August 2019 to 1 August 2026 |
| `iv-b-1-6-privatbeschulungsverordnung-pschuv/` | Verordnung über den privaten Einzelunterricht und die Privatschulen (GS IV B/1/6) | 2 | as enacted, then each consolidated version: 1 January 2023 to 1 August 2026 |
| `iv-b-1-14-pauschalbeitragsverordnung-paubv/` | Verordnung über die Festsetzung der Pauschalbeiträge für die Kinderbetreuung (GS IV B/1/14) | 1 | as enacted, 1 January 2023 |
| `iv-b-1-15-kinderbetreuungsverordnung-kibv/` | Verordnung über den Vollzug des Kinderbetreuungsgesetzes (GS IV B/1/15) | 1 | as enacted, 1 January 2023 |
| `iv-b-4-1-organisationsreglement-kantonsschule-kor/` | Reglement über die Organisation der Kantonsschule (GS IV B/4/1) | 2 | as enacted, then each consolidated version: 1 June 2020 to 1 August 2026 |
| `iv-b-4-2-reglement-gymnasium-rgym/` | Reglement über den Bildungsgang Gymnasium der Kantonsschule Glarus (GS IV B/4/2) | 5 | oldest version available, then each consolidated version: 1 April 2006 to 1 August 2026 |
| `iv-b-4-3-reglement-fachmittelschule-rfms/` | Reglement über den Bildungsgang Fachmittelschule der Kantonsschule Glarus (GS IV B/4/3) | 4 | as enacted, then each consolidated version: 1 August 2020 to 1 August 2026 |
| `iv-b-4-6-sportschulreglement-rspsch/` | Reglement über den Bildungsgang Sportschule der Kantonsschule Glarus (GS IV B/4/6) | 2 | as enacted, then each consolidated version: 1 August 2020 to 1 August 2026 |
| `iv-b-6-2-musikschulverordnung-msv/` | Verordnung zum Gesetz über die musikalische Bildung (GS IV B/6/2) | 3 | oldest version available, then each consolidated version: 7 May 2006 to 1 January 2026 |
| `iv-b-11-1-schulgesundheits-und-zahnpflegeverordnung-sgzv/` | Verordnung über die Gesundheitspflege und die Zahnpflege während der obligatorischen Schulzeit (GS IV B/11/1) | 4 | as enacted, then each consolidated version: 1 August 2012 to 1 August 2025 |
| `iv-b-31-1-volksschulverordnung-vsv/` | Verordnung über die Volksschule (GS IV B/31/1) | 6 | as enacted, then each consolidated version: 1 August 2011 to 1 August 2026 |
| `iv-b-31-2-volksschulvollzugsverordnung-vsvv/` | Verordnung über den Vollzug der Gesetzgebung zur Volksschule (GS IV B/31/2) | 6 | oldest version available, then each consolidated version: 1 August 2011 to 1 August 2026 |
| `iv-b-31-3-promotionsverordnung-promv/` | Verordnung über die Beurteilung, die Promotion und den Übertritt der Lernenden an der Volksschule (GS IV B/31/3) | 1 | as enacted, 1 August 2021 |
| `iv-b-51-2-1-berufsbildungsverordnung-bbv/` | Verordnung über die Steuerung und die Aufgaben in der Berufsbildung (GS IV B/51/2/1) | 2 | as enacted, then each consolidated version: 1 September 2017 to 1 August 2019 |
| `iv-b-51-6/` | Reglement über die Qualifikationsverfahren in der beruflichen Grundbildung (GS IV B/51/6) | 2 | as enacted, then each consolidated version: 1 March 2009 to 1 January 2025 |
| `iv-b-51-8/` | Reglement über die Berufsmaturität (GS IV B/51/8) | 7 | oldest version available, then each consolidated version: 1 January 2011 to 1 February 2026 |
| `iv-c-1-3/` | Reglement über die Weiterbildung der Lehrpersonen (GS IV C/1/3) | 2 | as enacted, then each consolidated version: 1 August 2011 to 1 August 2026 |
| `iv-c-2-4/` | Verordnung zur Beurteilung und Förderung der Lehrpersonen (GS IV C/2/4) | 1 | as enacted, 1 August 2012 |
| `iv-c-2-6-intensivweiterbildungsverordnung-iwv/` | Verordnung über die Intensivweiterbildung der Lehrpersonen kantonaler Schulen (GS IV C/2/6) | 1 | as enacted, 1 August 2026 |
| `iv-d-1-2/` | Sportverordnung (GS IV D/1/2) | 3 | oldest version available, then each consolidated version: 1 March 1990 to 1 August 2015 |
| `iv-d-1-3/` | Sportfondsverordnung (GS IV D/1/3) | 2 | oldest version available, then each consolidated version: 1 July 2006 to 1 January 2014 |
| `iv-e-1-3-stipendienverordnung/` | Verordnung über die Ausbildungs- und Schulgeldbeiträge (GS IV E/1/3) | 2 | as enacted, then each consolidated version: 1 August 2012 to 1 August 2026 |
| `iv-e-5/` | Verordnung über den Marty’schen Stipendienfonds (GS IV E/5) | 2 | as enacted, then each consolidated version: 1 January 1992 to 1 September 2014 |
| `iv-e-6/` | Verordnung über den Stipendienfonds Friedrich Streiff-Thiriet (GS IV E/6) | 2 | as enacted, then each consolidated version: 14 October 1974 to 1 September 2014 |
| `iv-f-1-1/` | Kulturfondsverordnung (GS IV F/1/1) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2014 |
| `iv-f-2/` | Verordnung über die Landesbibliothek (GS IV F/2) | 1 | as enacted, 1 July 2006 |
| `iv-g-1-3/` | Verordnung über den Vollzug der Natur- und Heimatschutzgesetzgebung (GS IV G/1/3) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `iv-g-1-4/` | Verordnung über den Fonds für Natur- und Landschaftsschutz (GS IV G/1/4) | 2 | as enacted, then each consolidated version: 1 January 2009 to 1 September 2014 |
| `iv-g-1-7/` | Verordnung über die Naturschutzbewirtschaftungsbeiträge (GS IV G/1/7) | 1 | as enacted, 23 December 2014 |
| `iv-g-2-1/` | Verordnung über die Gewährung von Kantons- und Gemeindebeiträgen im Bereich Denkmalpflege und Ortsbildschutz (GS IV G/2/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 January 2023 |
| `iv-g-3-1/` | Verordnung über den Arten- und Biotopschutz (GS IV G/3/1) | 1 | one version (the oldest available), 7 May 2006 |
| `iv-g-3-3/` | Verordnung über den Schutz der Pilze (GS IV G/3/3) | 1 | one version (the oldest available), 7 May 2006 |
| `iv-g-4-1/` | Verordnung über Ausgrabungen und Funde (GS IV G/4/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `ix-a-4-1-vkef/` | Verordnung zu den Kriterien für die Entwicklung von Flächen und Immobilien (GS IX A/4/1) | 1 | as enacted, 1 January 2025 |
| `ix-b-21-3-ruhetagsverordnung/` | Verordnung über den Vollzug des Ruhetagsgesetzes (GS IX B/21/3) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `ix-b-22-2-gastgewerbeverordnung-ggv/` | Verordnung über das Gastgewerbe und den Handel mit alkoholischen Getränken (GS IX B/22/2) | 1 | as enacted, 1 February 2023 |
| `ix-b-24-2-vkgg/` | Verordnung zum Kantonalen Geldspielgesetz (GS IX B/24/2) | 3 | as enacted, then each consolidated version: 1 July 2006 to 1 January 2021 |
| `ix-b-25-2-hgv/` | Verordnung zum Gesetz über die Handels- und Gewerbetätigkeiten (GS IX B/25/2) | 1 | as enacted, 1 January 2014 |
| `ix-b-25-5-vollzugsverordnung-zum-waffengesetz/` | Verordnung über den Vollzug des Bundesgesetzes über Waffen, Waffenzubehör und Munition (GS IX B/25/5) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2014 |
| `ix-b-25-8/` | Verordnung über den Vollzug des Bundesgesetzes über explosionsgefährliche Stoffe (GS IX B/25/8) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `ix-b-26-1/` | Verordnung über den Vollzug des Bundesgesetzes über den Konsumkredit (GS IX B/26/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `ix-b-31-2/` | Verordnung über die Entschädigung der Staatsgarantie für die Kantonalbank (GS IX B/31/2) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `ix-c-1-2-tourismusentwicklungsverordnung-tev/` | Verordnung zum Tourismusentwicklungsgesetz (GS IX C/1/2) | 3 | as enacted, then each consolidated version: 1 January 2008 to 1 January 2025 |
| `ix-d-1-2-lwvo/` | Kantonale Landwirtschaftsverordnung (GS IX D/1/2) | 3 | oldest version available, then each consolidated version: 1 May 2009 to 1 July 2018 |
| `ix-d-1-4-gebuhrenverordnung-landwirtschaft/` | Verordnung über die Erhebung von Gebühren für landwirtschaftliche Beratungen des Kantons Glarus (GS IX D/1/4) | 2 | as enacted, then each consolidated version: 1 June 2015 to 1 July 2019 |
| `ix-d-3-1-pachtzins-verordnung/` | Verordnung über die Bemessung des höchstzulässigen Pachtzinszuschlags für Sömmerungsbetriebe (GS IX D/3/1) | 3 | as enacted, then each consolidated version: 1 January 2002 to 1 October 2018 |
| `ix-d-4-1-strukturverbesserungsverordnung-kant-svv/` | Verordnung über die landwirtschaftlichen Strukturverbesserungen und die sozialen Begleitmassnahmen (GS IX D/4/1) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `ix-d-621-1-kantonale-weinbauverordnung/` | Verordnung über den Weinbau (GS IX D/621/1) | 1 | as enacted, 1 January 2012 |
| `ix-d-621-2/` | Verordnung über die kontrollierten Ursprungsbezeichnungen für Weine (GS IX D/621/2) | 1 | as enacted, 1 January 2021 |
| `ix-d-631-6/` | Verordnung über die Bienenzucht und die Bienenhaltung (GS IX D/631/6) | 2 | oldest version available, then each consolidated version: 28 June 1989 to 1 September 2014 |
| `ix-d-633-2-veterinarverordnung-vetv/` | Verordnung zum kantonalen Tierschutz- und Tierseuchengesetz (GS IX D/633/2) | 9 | oldest version available, then each consolidated version: 1 January 2006 to 1 January 2024 |
| `ix-d-633-5-viehsteuerverordnung-viehstv/` | Verordnung über die Viehsteuer (GS IX D/633/5) | 6 | as enacted, then each consolidated version: 1 May 2014 to 1 January 2025 |
| `ix-e-1-2/` | Verordnung zum kantonalen Waldgesetz (GS IX E/1/2) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2013 |
| `ix-e-1-3-naturgefahrenverordnung-ngv/` | Verordnung zum Schutz vor Naturgefahren (GS IX E/1/3) | 1 | as enacted, 1 June 2016 |
| `ix-e-2-4/` | Verordnung für die forstliche Planung (GS IX E/2/4) | 1 | one version (the oldest available), 7 May 2006 |
| `v-a-11-2/` | Polizeiverordnung (GS V A/11/2) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 1 June 2022 |
| `v-a-11-4/` | Verordnung über die Vergütung von Inkonvenienzen bei der Kantonspolizei (GS V A/11/4) | 3 | as enacted, then each consolidated version: 1 January 2009 to 1 July 2026 |
| `v-c-1-2-brandschutzverordnung/` | Verordnung zum Gesetz über den Brandschutz und die Feuerwehr (GS V C/1/2) | 4 | as enacted, then each consolidated version: 1 January 2004 to 1 December 2023 |
| `v-c-1-4/` | Kantonales Feuerwehrreglement (GS V C/1/4) | 3 | as enacted, then each consolidated version: 1 April 2004 to 1 February 2025 |
| `v-c-1-7/` | Präventionsreglement (GS V C/1/7) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 May 2017 |
| `v-c-1-8/` | Gebührenreglement über den Brandschutz und das Kaminfegerwesen (GS V C/1/8) | 1 | as enacted, 1 December 2023 |
| `v-c-4-3/` | Kaminfegerreglement (GS V C/4/3) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 December 2023 |
| `v-d-1-2/` | Vollzugsreglement zum Sachversicherungsgesetz (GS V D/1/2) | 2 | as enacted, then each consolidated version: 1 January 2011 to 17 March 2021 |
| `v-d-2-1/` | Entschädigungsreglement für den Verwaltungsrat der Glarnersach (GS V D/2/1) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `v-d-2-2-aufsichtsverordnung-glarnersach-vagl/` | Verordnung über die Aufsicht des Regierungsrates bei der Kantonalen Sachversicherung (GS V D/2/2) | 1 | as enacted, 1 January 2011 |
| `v-d-2-3/` | Personalreglement Glarnersach (GS V D/2/3) | 1 | as enacted, 1 January 2017 |
| `v-e-2-militarverordnung-mv/` | Verordnung über das Militärwesen (GS V E/2) | 2 | oldest version available, then each consolidated version: 1 January 1988 to 1 October 2019 |
| `v-e-3/` | Verordnung über den Militärunterstützungsfonds (GS V E/3) | 2 | oldest version available, then each consolidated version: 8 April 2008 to 1 September 2014 |
| `v-f-2-zivilschutzverordnung-zsvo/` | Verordnung zum Gesetz über den Zivilschutz (GS V F/2) | 2 | as enacted, then each consolidated version: 1 April 2014 to 1 June 2021 |
| `v-g-2-bevolkerungsschutzverordnung-bevv/` | Verordnung zum Gesetz über den Bevölkerungsschutz (GS V G/2) | 2 | as enacted, then each consolidated version: 1 September 2013 to 1 January 2016 |
| `v-h-4-kantonale-landesversorgungsverordnung-lvv/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die wirtschaftliche Landesversorgung (GS V H/4) | 1 | as enacted, 1 September 2013 |
| `vi-a-1-2-1-finanzhaushaltverordnung-fhv/` | Verordnung über den Finanzhaushalt des Kantons Glarus und seiner Gemeinden (GS VI A/1/2/1) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `vi-c-1-1-1-kantonale-verordnung-uber-die-kalte-progression-kvkp/` | Verordnung über den Ausgleich der Folgen der kalten Progression für die natürlichen Personen bei den Kantons- und Gemeindesteuern (GS VI C/1/1/1) | 4 | as enacted, then each consolidated version: 1 January 2024 to 1 January 2027 |
| `vi-c-1-2-steuerverordnung-stv/` | Verordnung zum Steuergesetz (GS VI C/1/2) | 6 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `vi-c-1-3-berufskostenverordnung-bkv/` | Verordnung über die Pauschalierung von Berufsauslagen bei unselbstständiger Erwerbstätigkeit und Gewinnungskosten bei Nebenerwerbstätigkeit (GS VI C/1/3) | 4 | as enacted, then each consolidated version: 1 January 2001 to 1 January 2026 |
| `vi-c-1-4/` | Verordnung über die Bewertung der Grundstücke (GS VI C/1/4) | 1 | one version (the oldest available), 7 May 2006 |
| `vi-c-1-5/` | Verordnung über die Quellensteuer natürlicher und juristischer Personen (GS VI C/1/5) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2015 |
| `vi-c-1-6-liegenschaftskostenverordnung-klkv/` | Verordnung über den Abzug der Kosten von Liegenschaften des Privatvermögens (GS VI C/1/6) | 2 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2021 |
| `vi-c-1-7-steuerbezugsverordnung-stbv/` | Verordnung über den Steuerbezug (GS VI C/1/7) | 3 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2019 |
| `vi-c-1-7-1/` | Verordnung über Zinsen, Skonti und Bezugslimiten für die Kantons- und Gemeindesteuern (GS VI C/1/7/1) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2022 |
| `vi-c-1-8-etax-verordnung-etaxv/` | Verordnung über die elektronische Einreichung der Steuererklärung (GS VI C/1/8) | 1 | as enacted, 1 January 2022 |
| `vi-c-1-10/` | Verordnung über die Durchführung der pauschalen Steueranrechnung (GS VI C/1/10) | 1 | as enacted, 1 January 1976 |
| `vi-c-2-1/` | Verordnung zum Bundesgesetz über die direkte Bundessteuer (GS VI C/2/1) | 2 | as enacted, then each consolidated version: 1 January 2001 to 1 January 2016 |
| `vi-c-2-2/` | Verordnung zum Bundesgesetz über die Verrechnungssteuer (GS VI C/2/2) | 2 | as enacted, then each consolidated version: 1 January 2001 to 1 January 2015 |
| `vi-c-2-3/` | Verordnung über den Vollzug der Rückerstattung des zusätzlichen Steuerrückbehaltes USA (GS VI C/2/3) | 2 | as enacted, then each consolidated version: 1 January 1994 to 1 January 2015 |
| `vi-c-4-7/` | Verordnung über die Gebühren der Arbeitsmarktbehörde (GS VI C/4/7) | 4 | as enacted, then each consolidated version: 1 November 2011 to 1 November 2026 |
| `vi-e-22-7-wildruhezonenverordnung-wrzv/` | Verordnung über die Wildruhezonen (GS VI E/22/7) | 4 | as enacted, then each consolidated version: 1 July 2017 to 1 September 2024 |
| `vi-e-22-8/` | Verordnung über das Jagdverbot bei den Fabrikweihern in Niederurnen (GS VI E/22/8) | 1 | as enacted, 1 August 2018 |
| `vi-e-31-2/` | Verordnung über die Fischerei (GS VI E/31/2) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2027 |
| `vi-e-31-3/` | Verordnung über den Vollzug der Fischereigesetzgebung (GS VI E/31/3) | 6 | oldest version available, then each consolidated version: 1 January 2012 to 15 January 2019 |
| `vi-e-31-4/` | Verordnung über die Patenttaxen für die Fischerei im Walensee (GS VI E/31/4) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 September 2014 |
| `vi-e-211-2-jagdverordnung/` | Verordnung zum kantonalen Jagdgesetz (GS VI E/211/2) | 4 | oldest version available, then each consolidated version: 7 May 2006 to 1 January 2026 |
| `vi-e-211-3-wildschadenverordnung/` | Verordnung über die Verhütung und Vergütung von Wildschäden (GS VI E/211/3) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2027 |
| `vi-e-211-4/` | Verordnung über den Vollzug der Jagdgesetzgebung (GS VI E/211/4) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vi-e-211-6/` | Verordnung über den Vollzug der Gesetzgebung zur Regulierung von Steinwildbeständen (GS VI E/211/6) | 2 | oldest version available, then each consolidated version: 1 April 2011 to 1 September 2014 |
| `vi-e-211-7-gebuhrenverordnung-jagd-und-fischerei-gebvjf/` | Verordnung über die Gebühren für Dienstleistungen der Jagd- und Fischereibehörden (GS VI E/211/7) | 1 | as enacted, 1 January 2016 |
| `vi-e-211-8-jfaor/` | Reglement für die kantonalen Jagd- und Fischereiaufsichtsorgane (GS VI E/211/8) | 1 | as enacted, 1 March 2024 |
| `vi-e-211-9-vejw/` | Verordnung über den Einbezug von Jagdberechtigten im Umgang mit Wölfen (GS VI E/211/9) | 1 | as enacted, 15 July 2025 |
| `vi-e-212-2-jagdausbildungsverordnung-jav/` | Verordnung über die Jagdausbildung (GS VI E/212/2) | 3 | as enacted, then each consolidated version: 1 May 2013 to 1 January 2020 |
| `vi-e-212-3-jagdhundeverordnung/` | Verordnung über die Jagdhunde (GS VI E/212/3) | 1 | as enacted, 1 May 2013 |
| `vi-e-212-4-treffsicherheitsnachweisverordnung-tsnwv/` | Verordnung über den Nachweis der Treffsicherheit (GS VI E/212/4) | 2 | as enacted, then each consolidated version: 1 January 2016 to 1 June 2016 |
| `vii-a-2-3-kantonale-geoinformationsverordnung-kgeoiv/` | Verordnung zum Einführungsgesetz zum Geoinformationsgesetz (GS VII A/2/3) | 4 | as enacted, then each consolidated version: 1 September 2012 to 1 June 2018 |
| `vii-a-2-4-geodatengebuhrenverordnung-geogv/` | Verordnung über die Gebühren für Zugang, Abgabe und Nutzung von Geodaten und Geodiensten (GS VII A/2/4) | 1 | as enacted, 1 September 2012 |
| `vii-a-2-5/` | Kantonale Verordnung über die amtliche Vermessung (GS VII A/2/5) | 2 | as enacted, then each consolidated version: 1 September 2012 to 1 April 2014 |
| `vii-b-1-2/` | Bauverordnung (GS VII B/1/2) | 5 | as enacted, then each consolidated version: 1 July 2011 to 1 May 2025 |
| `vii-b-1-4-raumentwicklungs-und-baugesetzgebungsvollzugsverordnung-rbgvv/` | Verordnung über den Vollzug der Raumentwicklungs- und Baugesetzgebung (GS VII B/1/4) | 6 | as enacted, then each consolidated version: 1 July 2011 to 1 September 2026 |
| `vii-b-1-5/` | Verordnung über die Gebühren für die Bearbeitung der Baugesuche durch die kantonalen Instanzen (GS VII B/1/5) | 2 | as enacted, then each consolidated version: 1 July 2011 to 1 September 2014 |
| `vii-b-6-1-1/` | Verordnung zum Gesetz über die öffentlich-rechtlichen Verhältnisse am Walensee (GS VII B/6/1/1) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 April 2025 |
| `vii-c-11-1-1/` | Verordnung zum Strassengesetz (GS VII C/11/1/1) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 April 2025 |
| `vii-c-11-3-reklameverordnung/` | Verordnung über das Plakat- und Reklamewesen an öffentlichen Strassen (GS VII C/11/3) | 3 | oldest version available, then each consolidated version: 7 May 2006 to 23 November 2022 |
| `vii-c-11-3-1/` | Verordnung über den Vollzug der Reklameverordnung (GS VII C/11/3/1) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-c-11-6-vlk/` | Verordnung über den Lawinendienst für die Kantonsstrassen (GS VII C/11/6) | 1 | as enacted, 1 July 2025 |
| `vii-c-11-8-1-vv-kvwg/` | Verordnung über den Vollzug des kantonalen Veloweggesetzes (GS VII C/11/8/1) | 1 | as enacted, 1 January 2025 |
| `vii-c-11-9/` | Verordnung über die Fuss- und Wanderwege (GS VII C/11/9) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 January 2023 |
| `vii-c-11-9-1/` | Verordnung über den Vollzug der Verordnung über Fuss- und Wanderwege (GS VII C/11/9/1) | 3 | oldest version available, then each consolidated version: 24 March 2009 to 1 April 2025 |
| `vii-c-12-1/` | Kantonale Vollziehungsverordnung zum Bundesgesetz über die Nationalstrassen vom 8. März 1960 (GS VII C/12/1) | 1 | one version (the oldest available), 8 June 1988 |
| `vii-d-4-2/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Binnenschifffahrt und zum Gesetz über die Besteuerung der Wasserfahrzeuge (GS VII D/4/2) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-d-4-3-smerv/` | Verordnung über die Melde-, Einwasserungsbewilligungs- und Reinigungspflicht für Schiffe (GS VII D/4/3) | 1 | as enacted, 1 May 2025 |
| `vii-d-5-1/` | Verordnung über den Vollzug der Luftfahrtgesetzgebung des Bundes (GS VII D/5/1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 September 2014 |
| `vii-d-6-1-1-vv-ovg/` | Verordnung über den Vollzug des Gesetzes über den öffentlichen Verkehr (GS VII D/6/1/1) | 1 | as enacted, 1 January 2026 |
| `vii-d-6-3/` | Verordnung über das Bewilligungsverfahren nach Verordnung über die Personenbeförderung (GS VII D/6/3) | 2 | oldest version available, then each consolidated version: 24 February 2009 to 1 September 2014 |
| `vii-d-11-2/` | Verordnung über den Strassenverkehr (GS VII D/11/2) | 1 | one version (the oldest available), 7 May 2006 |
| `vii-d-11-4/` | Verordnung zum Strassenverkehrsrecht und zu den Strassenverkehrsabgaben (GS VII D/11/4) | 4 | oldest version available, then each consolidated version: 7 May 2006 to 1 April 2019 |
| `vii-d-11-7-vollzugsverordnung-fahrverbot-klontal/` | Verordnung über den Vollzug zum Fahrverbot im Klöntal (GS VII D/11/7) | 1 | as enacted, 1 January 2026 |
| `vii-d-12-3-strassen-und-schifffahrtsgebuhrenverordnung-strgebv/` | Verordnung über die Gebühren im Strassenverkehr und in der Schifffahrt (GS VII D/12/3) | 6 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2024 |
| `vii-d-12-4-verkehrssteuernrabattverordnung-vstrv/` | Verordnung über das ökologische Rabattsystem der Verkehrssteuern (GS VII D/12/4) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2016 |
| `vii-d-12-5/` | Verordnung über die Gebühren für die Bewilligung von Veranstaltungen auf öffentlichen Strassen und von Strassensignalisationen (GS VII D/12/5) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `vii-d-41-4/` | Verordnung über die Schifffahrt auf dem Linthkanal (GS VII D/41/4) | 3 | as enacted, then each consolidated version: 1 January 2004 to 1 June 2022 |
| `vii-d-43-2/` | Verordnung zum Gesetz über die Besteuerung der Wasserfahrzeuge (GS VII D/43/2) | 1 | one version (the oldest available), 1 January 2011 |
| `vii-e-1-2/` | Verordnung zum Energiegesetz (GS VII E/1/2) | 3 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2026 |
| `vii-e-1-2-1/` | Verordnung über den Vollzug der Energiegesetzgebung (GS VII E/1/2/1) | 4 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2026 |
| `vii-e-1-3/` | Verordnung über den Energiefonds (GS VII E/1/3) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 July 2014 |
| `vii-e-1-3-1-energiefondsvollzugsverordnung-vv-enf/` | Verordnung über den Vollzug der Verordnung über den Energiefonds (GS VII E/1/3/1) | 13 | oldest version available, then each consolidated version: 1 July 2012 to 1 January 2025 |
| `vii-e-3/` | Verordnung über Rohrleitungsanlagen (GS VII E/3) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-a-1-7-ausbildungspflichtverordnung-apv/` | Verordnung über die Ausbildungspflicht im Bereich der Pflege (GS VIII A/1/7) | 2 | as enacted, then each consolidated version: 1 July 2024 to 1 August 2026 |
| `viii-a-1-8-forderverordnung-pflege-fopv/` | Kantonale Verordnung für die Förderung der Ausbildung im Bereich der Pflege (GS VIII A/1/8) | 2 | as enacted, then each consolidated version: 1 July 2024 to 1 June 2025 |
| `viii-a-3-1-gesundheitsberufeverordnung-gesbv/` | Verordnung über Berufe und Einrichtungen der Gesundheitsversorgung (GS VIII A/3/1) | 7 | oldest version available, then each consolidated version: 1 September 2008 to 1 October 2024 |
| `viii-a-4-1-heil-und-betaubungsmittelvollzugsverordnung-hbvv/` | Verordnung über den Vollzug der eidgenössischen Heil- und Betäubungsmittelgesetzgebung (GS VIII A/4/1) | 5 | as enacted, then each consolidated version: 1 May 2009 to 1 November 2026 |
| `viii-a-51-2-lebensmittel-und-chemikalienvollzugsverordnung-lcvv/` | Verordnung über den Vollzug des eidgenössischen Lebensmittelgesetzes und des eidgenössischen Chemikaliengesetzes (GS VIII A/51/2) | 1 | as enacted, 1 January 2018 |
| `viii-a-61-2-epidemiengesetz-vollzugsverordnung-vv-epg/` | Verordnung über den Vollzug des Bundesgesetzes über die Bekämpfung übertragbarer Krankheiten des Menschen (GS VIII A/61/2) | 1 | as enacted, 1 January 2016 |
| `viii-a-61-5-kantonale-hartefallmassnahmenverordnung-khfmv/` | Verordnung zum Spezialfonds Härtefallunterstützungen für Unternehmen im Zusammenhang mit der Covid-19-Pandemie (GS VIII A/61/5) | 8 | as enacted, then each consolidated version: 1 January 2021 to 1 June 2024 |
| `viii-a-61-6-schutzschirm-verordnung-kssv/` | Kantonale Verordnung über Massnahmen für Publikumsanlässe von überkantonaler Bedeutung im Zusammenhang mit der Covid-19-Epidemie (GS VIII A/61/6) | 1 | as enacted, 1 June 2021 |
| `viii-a-211-1-spitalverordnung-spitalv/` | Verordnung über das Kantonsspital Glarus (GS VIII A/211/1) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2018 |
| `viii-b-1-4-umweltschutzverordnung-usv/` | Verordnung zum Kantonalen Umweltschutzgesetz (GS VIII B/1/4) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 November 2020 |
| `viii-b-1-4-1/` | Verordnung über den Vollzug der Umweltschutz- und der Gewässerschutzgesetzgebung (GS VIII B/1/4/1) | 4 | as enacted, then each consolidated version: 7 May 2006 to 1 April 2025 |
| `viii-b-1-4-2-neobiotaverordnung-nbv/` | Verordnung über die Meldung und Bekämpfung invasiver gebietsfremder Organismen (GS VIII B/1/4/2) | 2 | as enacted, then each consolidated version: 1 July 2022 to 1 January 2025 |
| `viii-b-1-5/` | Verordnung über die Durchführung der Umweltverträglichkeitsprüfung (UVP) (GS VIII B/1/5) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 29 April 2015 |
| `viii-b-1-6/` | Verordnung über die Mindesthöhe von Kaminen (GS VIII B/1/6) | 2 | as enacted, then each consolidated version: 1 January 1991 to 1 September 2014 |
| `viii-b-3-4-deponieabgabeverordnung-dav/` | Verordnung über die Erhebung einer Abgabe auf die Deponierung von Abfällen (GS VIII B/3/4) | 3 | oldest version available, then each consolidated version: 1 January 2007 to 1 January 2019 |
| `viii-b-3-5-nachsorgeverordnung-nasv/` | Verordnung über die Abgaben für die Nachsorge von Deponien (GS VIII B/3/5) | 1 | as enacted, 1 January 2024 |
| `viii-b-6-1/` | Verordnung über die Öl-, Chemie- und Strahlenwehr (GS VIII B/6/1) | 3 | oldest version available, then each consolidated version: 7 May 2006 to 1 July 2022 |
| `viii-b-21-4-gewasserschutzverordnung-gschv/` | Verordnung zum Einführungsgesetz zum Gewässerschutzgesetz (GS VIII B/21/4) | 4 | oldest version available, then each consolidated version: 28 June 2006 to 1 January 2027 |
| `viii-b-21-5/` | Verordnung über den Gewässerrenaturierungsfonds (GS VIII B/21/5) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2027 |
| `viii-b-21-6-dungerbelastungsverordnung-dbv/` | Verordnung über die zulässige Düngerbelastung in der Landwirtschaft (GS VIII B/21/6) | 2 | as enacted, then each consolidated version: 1 November 1996 to 1 July 2017 |
| `viii-c-21-1-1/` | Verordnung über den Vollzug der bundesrechtlichen Bestimmungen in den Bereichen Arbeit, Unfallverhütung und Produktesicherheit (GS VIII C/21/1/1) | 2 | as enacted, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-c-21-2/` | Verordnung über die Gebühren des kantonalen Arbeitsinspektorats (GS VIII C/21/2) | 3 | as enacted, then each consolidated version: 1 April 2003 to 1 November 2026 |
| `viii-c-22-1/` | Verordnung über den Vollzug des Bundesgesetzes über die Heimarbeit (GS VIII C/22/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-c-23-1/` | Verordnung über den Vollzug des Bundesgesetzes über Massnahmen zur Bekämpfung der Schwarzarbeit (GS VIII C/23/1) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 September 2014 |
| `viii-c-32-1/` | Verordnung über den Vollzug des Bundesgesetzes über die in die Schweiz entsandten Arbeitnehmerinnen und Arbeitnehmer und flankierende Massnahmen (GS VIII C/32/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-c-32-2-voaa/` | Verordnung über den Vollzug der Bundesgesetzgebung über Zulassung und Erwerbstätigkeit ausländischer Arbeitskräfte (GS VIII C/32/2) | 3 | as enacted, then each consolidated version: 1 July 1990 to 1 July 2015 |
| `viii-c-33-3/` | Verordnung zum Gesetz über die steuerbegünstigten Arbeitsbeschaffungsreserven (GS VIII C/33/3) | 1 | as enacted, 7 May 2006 |
| `viii-d-5-2-vvo-eg-famzg/` | Verordnung über den Vollzug des Einführungsgesetzes zum Bundesgesetz über Familienzulagen (GS VIII D/5/2) | 4 | as enacted, then each consolidated version: 1 January 2009 to 1 January 2017 |
| `viii-d-6-2-1/` | Verordnung über die Gebühren zum Arbeitsvermittlungsgesetz (GS VIII D/6/2/1) | 2 | oldest version available, then each consolidated version: 1 April 2003 to 1 September 2014 |
| `viii-d-6-3/` | Verordnung über die Arbeitslosenkasse des Kantons Glarus (GS VIII D/6/3) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-d-6-5/` | Verordnung über den Vollzug des Einführungsgesetzes zum Bundesgesetz über die Arbeitsvermittlung und den Personalverleih sowie des Einführungsgesetzes zum Bundesgesetz über die obligatorische Arbeitslosenversicherung und die Insolvenzentschädigung (GS VIII D/6/5) | 3 | as enacted, then each consolidated version: 7 May 2006 to 1 July 2023 |
| `viii-d-13-2-kantonale-erganzungsleistungsverordnung-kelv/` | Verordnung über den Vollzug des Einführungsgesetzes zum Bundesgesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (GS VIII D/13/2) | 14 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `viii-d-21-2-pramienverbilligungsvollzugsverordnung-vv-pv/` | Verordnung über den Vollzug der Prämienverbilligung (GS VIII D/21/2) | 4 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2020 |
| `viii-d-21-3-pramienverbilligungsverordnung-pvv/` | Verordnung über die Prämienverbilligung (GS VIII D/21/3) | 3 | as enacted, then each consolidated version: 1 January 2005 to 1 January 2020 |
| `viii-d-21-9-kantonale-hochstzahlenverordnung-khzv/` | Kantonale Verordnung über die Festlegung der Höchstzahlen für Ärztinnen und Ärzte (GS VIII D/21/9) | 1 | as enacted, 1 July 2023 |
| `viii-e-21-4-asyl-und-fluchtlingsverordnung-afv/` | Verordnung über die wirtschaftliche Hilfe und den Zugang zum Arbeitsmarkt im Asyl- und Flüchtlingsbereich (GS VIII E/21/4) | 5 | as enacted, then each consolidated version: 1 October 2016 to 1 January 2026 |
| `viii-e-21-4-1-asylsozialhilfeverordnung-asylshv/` | Verordnung über die reduzierte Sozialhilfe im Asyl- und Flüchtlingsbereich (GS VIII E/21/4/1) | 1 | as enacted, 1 January 2026 |
| `viii-e-21-5-sozialhilfeverordnung-shv/` | Verordnung über die Bemessung der wirtschaftlichen Sozialhilfe und der Hilfe in Notlagen in Ausnahme der Richtlinien der Schweizerischen Konferenz für Sozialhilfe (GS VIII E/21/5) | 2 | as enacted, then each consolidated version: 1 June 2022 to 1 March 2026 |
| `viii-e-21-6/` | Verordnung über die Erteilung von Betriebsbewilligungen für stationäre Einrichtungen und deren Haftung (GS VIII E/21/6) | 5 | as enacted, then each consolidated version: 7 May 2002 to 1 April 2023 |
| `viii-e-21-10-alimentenhilfeverordnung-alvo/` | Verordnung über die Alimentenhilfe (GS VIII E/21/10) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2022 |
| `viii-e-23-2/` | Verordnung über Beiträge an Bauten und Betriebseinrichtungen für Behinderte (GS VIII E/23/2) | 2 | oldest version available, then each consolidated version: 16 November 2010 to 1 September 2014 |
| `viii-e-25-1/` | Verordnung über den Rosa-Hefti-Fonds (GS VIII E/25/1) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-e-25-2/` | Verordnung über den A.-Bremicker-Fonds (GS VIII E/25/2) | 3 | oldest version available, then each consolidated version: 7 May 2006 to 1 October 2017 |
| `viii-e-25-3/` | Verordnung über den Fonds zur ergänzenden Unterstützung von Familien (GS VIII E/25/3) | 3 | as enacted, then each consolidated version: 13 October 2009 to 1 January 2023 |
| `viii-e-25-4/` | Verordnung über den Dr.-Emilia-Mercier-Fonds für Gehörlose (GS VIII E/25/4) | 2 | oldest version available, then each consolidated version: 7 May 2006 to 1 September 2014 |
| `viii-e-25-5/` | Verordnung über die Beiträge aus dem Fonds für psychisch Kranke (GS VIII E/25/5) | 2 | oldest version available, then each consolidated version: 9 August 2011 to 1 September 2014 |
| `viii-e-25-6/` | Sozialfondsverordnung (GS VIII E/25/6) | 1 | as enacted, 1 January 2014 |

## Source

The GS (systematic collection) of the canton, published by the canton at <https://gesetze.gl.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (SBE). Annexes the collection publishes only as separate PDF files are not included.

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

The author of a commit is the amending act, named by its entry in the chronological collection (SBE), with an e-mail address that cannot exist (`<act key>@gesetze.gl.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
