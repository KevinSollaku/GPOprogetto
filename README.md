# TalkMasters

## Problema
Imparare le lingue straniere è spesso difficile e costoso. Le lezioni tradizionali in aula sono scomode e l'accesso ad insegnanti madrelingua è limitato. 
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

### Caso d'uso professore
![Diagramma professore]([https://yuml.me/diagram/scruffy/usecase/[Professore]^[Utente], [Utente]-(Registrarsi), [Utente]-(Log in), (Registrarsi)>(Lingue conosciute), (Log in)<(Crea classe), (Log in)<(Guarda classi create), (Log in)<(Partecipa ad una classe), (Guarda classi create)<(Disdici classe)](https://yuml.me/diagram/scruffy/usecase/[Professore]%5E[Utente],%20[Utente]-(Registrarsi),%20[Utente]-(Log%20in),%20(Registrarsi)%3E(Lingue%20conosciute),%20(Log%20in)%3C(Crea%20classe),%20(Log%20in)%3C(Guarda%20classi%20create),%20(Log%20in)%3C(Partecipa%20ad%20una%20classe),%20(Guarda%20classi%20create)%3C(Disdici%20classe)))


![Diagramma UML](https://yuml.me/diagram/scruffy/usecase/[Professore]-(Registrarsi),%20[Studente]-(Registrarsi),%20(Registrarsi)%3C(Scegli%20lingua%20da%20imparare),%20(Registrarsi)%3E(Lingue%20conosciute),%20[Professore]-(Log%20in),%20[Studente]-(Log%20in),%20(Log%20in)%3C(Scegli%20classe),%20(Log%20in)%3C(Crea%20classe),%20(Log%20in)%3C(Guarda%20classi%20prenotate),%20(Guarda%20classi%20prenotate)%3C(Disdici%20classe),%20(Prenota%20classe)%3C(Disdici%20classe),%20(Scegli%20classe)%3E(Pagamento),%20(Pagamento)%3C(Successo),%20(Pagamento)%3C(Non%20successo),%20(Successo)%3E(Prenota%20classe))


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
