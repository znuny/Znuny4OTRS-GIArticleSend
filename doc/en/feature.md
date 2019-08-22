# Functionality

In OTRS it's not possible to send articles via the Generic Interface operations TicketCreate and TicketUpdate.
This package extends OTRS to make this possible.

## New article parameters
To send an article via operation TicketCreate or TicketUpdate, you have to set the following new parameters within the article data:

```
ArticleSend => 1,
To          => 'email@example.com', # Email address to send article to.
```

E-Mails can also be signed and encrypted:

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
