# sitedigest
Website analysis tool

SiteDigest is a website analysis command line tool, it designed to provide the basic information about the website and hosting enviroment.

SiteDigest while establishing connection prints informations such as encountered redirections or return code. 
Once when content is returned, SD does DOM search to extract a basic information about the website.
SiteDigest can be used to check over all server and site health, website setup or for do SEO analysis.
SD is not designed to render the page, or crawl to linked pages or resources.

```
$ sitedigest teafs.org
Sat May 12 2018 23:15:00 GMT+0200 (CEST): rewriting "teafs.org" to: http://teafs.org/
                digesting http://teafs.org/
Sat May 12 2018 23:15:00 GMT+0200 (CEST): http://teafs.org/ digested.
======= SERVER RESPONCE CHECK =======
StatusCode: 200
Got any cookies?: 0
======= ===================== =======
========= WEB CONTENT CHECK =========
CMS: not detected
lang: "en"
title: "TeaFS filesystem"
meta description: "TeaFS - no hierarchical, but tags based filesystem"
========= ================= =========
====== EXTERNAL LINK STRUCTURE ======
http://en.wikipedia.org/wiki/Filesystem_in_Userspace: FUSE
http://xkcd.com/744/: http://xkcd.com/744/
http://validator.w3.org/check?uri=referer: 
====== ======================= ======
```

```
$ sitedigest divercity.earth
Sat May 12 2018 23:15:33 GMT+0200 (CEST): rewriting "divercity.earth" to: http://divercity.earth/
                digesting http://divercity.earth/
Sat May 12 2018 23:15:35 GMT+0200 (CEST): https://divercity.earth/ digested.
======= SERVER RESPONCE CHECK =======
StatusCode: 200
 ---> Redirected to (1): https://divercity.earth/
Got any cookies?: 1
======= ===================== =======
========= WEB CONTENT CHECK =========
CMS: "WordPress 4.9.5"
lang: "en"
title: "DIVERCITY EARTH market place – Women clothing & Accesories…"
meta description: not detected
========= ================= =========
====== EXTERNAL LINK STRUCTURE ======
https://woocommerce.com: Built with Storefront & WooCommerce
====== ======================= ======
```
