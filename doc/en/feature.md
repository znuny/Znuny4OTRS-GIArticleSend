# Functionality

This package enables OTRS to send articles via the generic interface operations TicketCreate and TicketUpdate.

## New article parameters

To send an article via operation TicketCreate or TicketUpdate, you have to set the following new parameters within the article data:

```
ArticleSend => 1,
To          => 'email@example.com',  # Email address to send article to.
Cc          => 'email2@example.com', # Optional: Cc email address to send article to.
Bcc         => 'email3@example.com', # Optional: Bcc email address to send article to.
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
