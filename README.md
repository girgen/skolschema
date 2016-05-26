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
