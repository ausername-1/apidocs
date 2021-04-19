Discord URL Shortener
===========

Table of contents
=================
hello :ref:`Javascript Example`


Javascript Example
==================
    const fetch = require('node-fetch')
    const params = {url: "url", slug: "slug}
    const data = fetch('/api/shorten', {
    method: 'POST',
    body: JSON.stringify(params)
    }).then((res => res.json()))
