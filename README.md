![Znuny logo](https://www.znuny.com/assets/images/logo_small.png)


![Build status](https://badge.proxy.znuny.com/Znuny4OTRS-GIArticleSend/master)

Znuny4OTRS-GIArticleSend
========================
This package enables the standard Generic Interface ticket operations to send articles.

This feature is based on OTRS [pull request #815](https://github.com/OTRS/otrs/pull/815) by github user [fredericve](https://github.com/fredericve).
Also many thanks to [PC-College](https://www.pc-college.de/) who made this package possible.

**Prerequisites**

- Znuny LTS 6, ((OTRS)) Community Edition 6 or OTRS 6
- [Znuny4OTRS-Repo](https://www.znuny.com/add-ons/znuny4otrs-repository)

**Installation**

Download the [package](https://addons.znuny.com/api/addon_repos/public/1092/latest) and install it via admin interface -> package manager or use [Znuny4OTRS-Repo](https://www.znuny.com/add-ons/znuny4otrs-repository).

**Download**

Download the [latest version](https://addons.znuny.com/api/addon_repos/public/1092/latest).


**Usage**
To send an article via operation TicketCreate or TicketUpdate, you have to set the following new parameters within the article data:

```
ArticleSend => 1,
To          => 'email@example.com', # Email address to send article to.
```

**Commercial Support**

For this add-on and for Znuny in general visit [https://www.znuny.com](https://www.znuny.com). Looking forward to hear from you!

Enjoy!

Your Znuny Team!

[https://www.znuny.com](https://www.znuny.com)
