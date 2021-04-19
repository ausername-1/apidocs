.. include:: ../README.rst
.. include:: ./javascriptexample.rst
.. code-block:: javascript
  :linenos:

  const fetch = require('node-fetch')

  const params = {url: 'url', slug: ''}
  const data = await fetch('/api/shorten', {
  method: 'post',
  body: JSON.stringify(params)
  }).then((res => res.json()))

  console.log(data)
