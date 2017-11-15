![Znuny logo](http://znuny.com/assets/images/logo_small.png)

Znuny4OTRS-GIArticleSend
========================
This package enables the standard Generic Interface ticket operations to send articles.

This feature is based on OTRS [pull request #815](https://github.com/OTRS/otrs/pull/815) by github user [fredericve](https://github.com/fredericve).
Also many thanks to [PC-College](https://www.pc-college.de/) who made this package possible.

**Usage**
To send an article via operation TicketCreate or TicketUpdate, you have to set the following new parameters within the article data:

```
ArticleSend => 1,
To          => 'email@example.com', # Email address to send article to.
```

**Prerequisites**

- Znuny4OTRS-Repo

- OTRS 5

**Installation**

Download the package and install it via admin interface -> package manager or use Znuny4OTRS-Repo.

**Download**

For download see [http://znuny.com/en/#!/addons](http://znuny.com/en/#!/addons)

**Commercial Support**

For this extension and for OTRS in general visit [http://znuny.com](http://znuny.com). Looking forward to hear from you!

Enjoy!

 Your Znuny Team!

 [http://znuny.com/](http://znuny.com/)
