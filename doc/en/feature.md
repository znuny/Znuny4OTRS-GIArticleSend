# Send articles via Generic Interface

In OTRS it's not possible to send articles via the Generic Interface operations TicketCreate and TicketUpdate.
This package extends OTRS to make this possible.

## New parameters "ArticleSend" and "To"

To send an article via operation TicketCreate or TicketUpdate, you have to set the following new parameters within the article data:

```
ArticleSend => 1,
To          => 'email@example.com', # Email address to send article to.
```
