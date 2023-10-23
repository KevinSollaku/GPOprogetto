L'apprendimento delle lingue straniere è spesso inefficace e costoso. Le lezioni tradizionali in aula sono scomode e l'accesso a insegnanti madrelingua è limitato. 
Inoltre, la maggior parte delle piattaforme di apprendimento online sono inefficaci e mirate solo al guadagno.

Specifica dei requisti:
1. Interfaccia per l'utente deve poter registrarsi e fare il login (funzionale)
2. Il sito deve insegnare agli utenti la lingua selezionata (funzionale)
3. Collegare l'utente all'insegnate (funzionale)
4. Pianificare le lezioni tra utente e insegnante (funzionale)
5. Sistema di pagamento (funzionale)
6. Supportare lingue diverse (non funzionale)
7. Certificazione insegnante (di dominio)
8. Rispettare le norme gdpr (di dominio)

![Diagramma UML](http://yuml.me/diagram/scruffy/usecase/[Professore]-(Registrarsi), [Studente]-(Registrarsi), (Registrarsi)<(Scegli, lingua, da, imparare), (Registrarsi)>(Lingue, conosciute), [Professore]-(Log, in), [Studente]-(Log, in), (Log, in)<(Scegli, classe), (Log, in)<(Crea, classe), (Log, in)<(Guarda, classi, prenotate), (Guarda, classi, prenotate)<(Disdici, classe), (Prenota, classe)<(Disdici, classe), (Scegli, classe)>(Pagamento), (Pagamento)<(Successo), (Pagamento)<(Non, successo), (Successo)>(Prenota, classe))



[Professore]-(Registrarsi)
[Studente]-(Registrarsi)
(Registrarsi)<(Scegli lingua da imparare)
(Registrarsi)>(Lingue conosciute)
[Professore]-(Log in)
[Studente]-(Log in)
(Log in)<(Scegli classe)
(Log in)<(Crea classe)
(Log in)<(Guarda classi prenotate)
(Guarda classi prenotate)<(Disdici classe)
(Prenota classe)<(Disdici classe)
(Scegli classe)>(Pagamento)
(Pagamento)<(Successo)
(Pagamento)<(Non successo)
(Successo)>(Prenota classe)
