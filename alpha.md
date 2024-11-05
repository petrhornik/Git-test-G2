# Otázky Alpha / Alpha Questions

## K čemu slouží příkaz 'git pull'? / What does the 'git pull' command do?

Tento příkaz stáhne změny z dálkového repozitáře na lokální repozitář(do předem určené složky) a z branche na které se právě nacházíme(to se dá zjistit pomocí {git status} nebo {git branch --list}(vybraná branch bude označena * a text bude zelený(v případě powershellu))). Používá se hlavě při týmové práci(2 a více), synchronizovaný remote repozitář mezi několika programátory.

## K čemu slouží příkaz 'git log' a co se z něho dá vyčíst? / What does the 'git log' command do and what inforamation does it provide?

Git log slouží pro zobrazení historie commitů(co? kdy? jak?). Jednotlivé informace o provedených commitech obsahují: hash, autora(jmého a mail), datum a čas, a komentář(git commit -m "TUTO ZPRÁVU").