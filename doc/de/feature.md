# Funktionalität

Dieses Paket ermöglicht den Versand von Artikeln über die Generic-Interface-Operationen TicketCreate und TicketUpdate.

## Neue Artikelparameter

Um einen Artikel zu versenden, müssen für die Operation TicketCreate oder TicketUpdate folgende Parameter in den Artikeldaten mitgegeben werden:

```
ArticleSend => 1,
To          => 'email@example.com',  # E-Mail-Adresse, an die der Artikel versendet werden soll.
Cc          => 'email2@example.com', # Optional: Cc-E-Mail-Adresse, an die der Artikel versendet werden soll.
Bcc         => 'email3@example.com', # Optional: Bcc-E-Mail-Adresse, an die der Artikel versendet werden soll.
```

Zusätzlich können die so versendeten E-Mails signiert und verschlüsselt werden:

```
# Signing and encryption, only used when ArticleSend is set to 1
Sign => {
    Type    => 'PGP',
    SubType => 'Inline|Detached',
    Key     => '81877F5E',
    Type    => 'SMIME',
    Key     => '3b630c80',
},
Crypt => {
    Type    => 'PGP',
    SubType => 'Inline|Detached',
    Key     => '81877F5E',
    Type    => 'SMIME',
    Key     => '3b630c80',
},
```
