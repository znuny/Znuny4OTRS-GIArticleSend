# Funktionalität

In OTRS ist es nicht möglich, über die mitgelieferten Generic-Interface-Operationen TicketCreate und TicketUpdate Artikel zu versenden.
Das Paket Znuny4OTRS-GIArticleSend ermöglicht dies.

## Neue Artikelparameter
Um einen Artikel zu versenden, müssen für die Operation TicketCreate oder TicketUpdate folgende Parameter in den Artikeldaten mitgegeben werden:

```
ArticleSend => 1,
To          => 'email@example.com', # E-Mail-Adresse, an die der Artikel versendet werden soll.
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
