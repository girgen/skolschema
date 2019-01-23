# Skolschema

Denna standard syftar till att beskriva den informationsöverföring mellan olika system som krävs för att skapa skolans schema, och även för att göra schemainformationen åtkomlig för mottagande system. För att skapa ett skolschema krävs information om exempelvis klasser, grupper, lärare och undervisningstid i olika ämnen. Arbetet som leder fram till det färdiga schemat kan beskrivas som ett antal processer, vilka alla bidrar med olika delmängder av den information som behövs i schemat.

Standarden ges ut och underhålls av SIS, Swedish Standards Institute, och finns att köpa från https://www.sis.se/produkter/informationsteknik-kontorsutrustning/ittillampningar/ittillampningar-inom-utbildning/ss-120002018/.

Standarden baseras på en öppen standard för informationsutbyte från Internet Engineering Task Force (IETF). Den öppna standarden som används heter System for Cross-domain Identity Management (SCIM) och finns redogjord för i IETF-dokumenten RFC7642, RFC7643 och RFC7644. 

I schema finns SCIM-schema för de tillägg som gjorts. I mappen exempel finns exempel för samtliga objekt.

En del mindre justeringar har gjorts efter releasen av standarden. Ändringar i exempel dokumenteras bara via _commit-loggen_. Errata för standarddokumentet listas **enbart** här.

Errata för schemat och standarddokumentet:
- **schema/SchoolUnit.json:** lagt till referensen till _organisation_. Det är korrekt i standarddokumentet.
- **schema/StudentGroup.json:** korrigerat referensen till elever så att read-only-attributet för elevens namn heter "display". Det är korrekt i standarddokumentet.
- **enrolments:** på en User finns en lista med _"enrolments"_. Det attributet ska stavas med enbart gemener. Se [schemat](https://github.com/girgen/skolschema/blob/f214c070d3ee5ece2819f50e118ec438c20fc3dc/schema/User.json#L113)
