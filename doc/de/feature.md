# Versand von Artikeln über Generic-Interface

Im OTRS ist es nicht möglich, über die mitgelieferten Generic-Interface-Operationen TicketCreate und TicketUpdate Artikel zu versenden.
Das Paket Znuny4OTRS-GIArticleSend ermöglicht dies.

## Neue Parameter "ArticleSend" und "To"

Um einen Artikel zu versenden, müssen für die Operation TicketCreate oder TicketUpdate folgende Parameter in den Artikeldaten mitgegeben werden:

```
ArticleSend => 1,
To          => 'email@example.com', # E-Mail-Adresse, an die der Artikel versendet werden soll.
```
