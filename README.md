# skolschema

course *eller* subject används i Activity. Course för gymnasiet och annan verksamhet baserat på kurser (exempelvis komvux). Subject syftar på grundskoleämnen (är ju redundant för gymnasiet)

*Frågor:*

hostas schemat någonstans? URI / URL?

om "start" = "", är det invalid data eller?

Finns det en tjänst för att validera? Eric W?

comment på calendarevent, finns bättre namn? vad används den till?

Vi tycker exceptions är för komplicerade. Även om det kan beskrivas i källan, behöver det verkligen kommuniceras? En enklare variant vore att inte ha tid eller length, undantag betyder bara att "objektet" *inte* deltar? Resten borde handla om frånvaro snarare än schema? Om en elev ska gå litet tidigare på måndagar, skrivs det verkligen i schemat? Har vi nytta av detta?

Varför finns teachingLength för Group och Teacher men inte för elever?

Behövs flera parentactivity? Vi tycker inte det. NO-exemplet?

Courses och subjects på grupper. Kan det vara flera? Kan det vara både och?

activity.type sätter egentligen lärarens roll. behövs flera lärarroller i samma activity?

datumintervall som gått ur tiden ska väl inte behöva kommuniceras i evighet? Men hur får man då fram historisk data? Var går gränsen, eller hur avgränsar man?

Tjänstgöringsgrad - årsarbetstid är kanske bättre?

Var är man anställd? Skola? Kommun? Skolenhet? "Skola + skolform"?

Många frågor kring anställning. Olika antal timmar över tid?

Lärare hör inte till skolenhet, utan normalt sett till skola+skolform. I LifeCare kan man välja att koppla anställningen till en Skola eller till kommunen.

Skolenhet kopplar *bara* ihop elever och rektor.

Kommun
 Förvaltning
        anställning musik
  Skola 1
  Skola 2
     Skola 1 Sär
        anställning asdfsadf

Lärarroll på grupp? Klasslärare? 


för grupper med olika typer, hur spärrar vi  olika typers attribut?

Employeegroup, oklart, ska den verkligen gruppera anställningar? Onödigt komplicerat och oklart syfte?

Course och subject ska väl också ha UUID om det är egna objekt och kan ha olika värdeförråd i skolformer, vissa helt fria.

behöver vi ha historik på årskurs?

Skolenhet / Skola på anställning, funkar det med ref till grupp?

Grupper kan väl inte ha skolform, bara elever?

Behövs flera responsible (ändring över tid?) för klasser?

Behövs flera kurskoder för en grupp?

Enklare att ha gruppmodell för skolor och skolenheter. Ibland kan skolan innehålla flera skolenheter, en det omvända borde kunna finnas, att flera skolor bildar en skolenhet.

Skolenhet, municipality code, gäller det även friskolor?
Skolenhet: vad är "ownerType"?


Ägare: hur gör vi? utökare meta-taggen?

Telefon i core-schemat, vi förutsätter att "mobile" innebär att det går att SMS:a. Det bör noteras i dokumentet?

schoolYear på grupp är inte optimalt, kan vi ta bort det? kanske?

nativelanguage? behövs det alls? i så fall på person-objektet.

student har vi problem med: årskurs program skolform är alla tidbundna. var är egentligen "student"objektet ? Tidigare har det *bara* innehållit kontaktpersoner.

student kopplas till activity både direkt och via studentassignment, varför? vad tillförs i studentassignment som gör att det behöver vara ett relationsobjekt?


Varför skola: 
- schemaläggning avser just lokaler, dvs skola...
- lärare som jobbar på ett gymnasium med flera enheter så bestäms fördelningen i tjänstefördelningen, om alls. så var är läraren anställd?
- grupper som gäller flera skolenheter? egentligen tillhör *enbart* personer en enhet. grupperna tillhör ingen enhet, och bara utfallet av vilka elever som till slut fanns i gruppen ligger till grund för rapporteringen.


Employeegroup, är det verkligen något som finns och i så fall vad används det till?

2016-11-23
kan personnummer få vara globlat unikt?

kontaktpersoner har tappats bort i diagrammet, har alltid funnits i diskussionen och i det svartvita arket.

Pilarna från StudentAssignment och StudentException ska till User.

canonicalvalues på årskurs i enrolment och studengroup?

vi har hoppat fram och tillbaka med om studentgrupper behöver ha en lista med ämnen eller kurser som de är ämnade för. alltså om en studengrupp är skapade för att ha matematik, ska det listas, eller måste schemaprogrammet/schemaläggaren gissa det från namnet?