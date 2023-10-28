# TalkMasters

## Indice
- [Introduzione](#introduzione)
- [Requisiti funzionali](#requisiti-funzionali)
- [Requisiti non funzionali](#requisiti-non-funzionali)
- [Requisiti di dominio](#requisiti-di-dominio)
- [Diagrammi UML](#diagrammi-uml)

## Introduzione
Imparare le lingue straniere è spesso difficile e costoso. Le lezioni tradizionali in aula sono scomode e l'accesso ad insegnanti madrelingua è limitato. 
Inoltre, la maggior parte delle piattaforme di apprendimento online sono inefficaci e mirate solo al guadagno.

## Requisiti funzionali:
1. Interfaccia per l'utente deve poter registrarsi e fare il login nella quale:
   - dovrà scegliere se essere studente o insegnante
   - dovrà impostare le lingue che vuole insegnare o imparare

2. Permettere allo Studente di scegliere una classe della lingua da voler imparare:
   - prenotare un posto nella classe
   - una volta finita la classe poter lasciare una recensione all'insegnante

3. Permettere all'Insegnante di creare una classe della lingua che conosce:
   - impostare un prezzo per la classe e quanti posti disponibili

4. Sistema di pagamento:
   - se si ha un successo prenota correttamente il posto
   - se non si ha successo ritorna alla scelta della classe

## Requisiti non funzionali
1. Supportare lingue diverse:
   - non avrebbe senso se supportasse solo una lingua

## Requisiti di dominio
1. insegnanti dovranno avere una certificazione:
   - verrà controllata da un amministratore

2. Rispettare le norme gdpr

## Diagrammi uml

### Caso d'uso Professore
![Diagramma professore](https://yuml.me/diagram/scruffy/usecase/[Professore]%5E[Utente],%20[Utente]-(Registrarsi),%20[Utente]-(Log%20in),%20(Registrarsi)%3E(Lingue%20conosciute),%20(Lingue%20conosciute)%3E(Verifica%20delle%20conoscienze),%20[Amministratore]-(Verifica%20delle%20conoscienze),%20(Log%20in)%3C(Crea%20classe),%20(Log%20in)%3C(Guarda%20classi%20create),%20(Guarda%20classi%20create)%3C(Disdici%20classe),(Guarda%20classi%20create)%3C(Visualizza%20dettagli%20classe))

### Caso d'uso Studente
![Diagramma Studente](https://yuml.me/diagram/scruffy/usecase/[Studente]%5E[Utente],%20[Utente]-(Registrarsi),%20[Utente]-(Log%20in),%20(Registrarsi)%3E(Lingua%20che%20si%20vuole%20imparare),%20(Log%20in)%3E(Prenota%20una%20classe),(Log%20in)%3C(Guarda%20classi%20prenotate),(Guarda%20classi%20prenotate)%3C(Disdici%20classe),%20(Prenota%20una%20classe)%3E(Pagamento),%20(Pagamento)%3C(Successo),%20(Pagamento)%3C(Non%20successo),%20(Non%20successo)%3E(Prenota%20una%20classe),%20(Successo)%3E(Classe%20prenotata),%20(Classe%20prenotata)%3E(Inviare%20email),%20[Sistema]-(Inviare%20email))

### Diagramma completo
![Diagramma UML](https://yuml.me/diagram/scruffy/usecase/[Amminstratore]-(Verifica%20delle%20conoscienze),%20[Studente]%5E[Utente],(Registrarsi)%3E(Lingua%20che%20si%20vuole%20imparare),(Log%20in)%3C(Guarda%20classi%20prenotate),%20(Lingue%20conosciute)%3E(Verifica%20delle%20conoscienze),(Guarda%20classi%20prenotate)%3C(Disdici%20classe),%20(Prenota%20una%20classe)%3E(Pagamento),%20(Pagamento)%3C(Successo),%20(Pagamento)%3C(Non%20successo),%20(Non%20successo)%3E(Prenota%20una%20classe),%20(Successo)%3E(Classe%20prenotata),%20(Classe%20prenotata)%3E(Inviare%20email),%20[Sistema]-(Inviare%20email),%20[Professore]%5E[Utente],%20[Utente]-(Registrarsi),%20[Utente]-(Log%20in),%20(Registrarsi)%3E(Lingue%20conosciute),%20(Log%20in)%3C(Crea%20classe),%20(Log%20in)%3C(Guarda%20classi%20create),%20(Log%20in)%3E(Prenota%20una%20classe),%20(Guarda%20classi%20create)%3C(Disdici%20classe),(Guarda%20classi%20create)%3C(Visualizza%20dettagli%20classe))
