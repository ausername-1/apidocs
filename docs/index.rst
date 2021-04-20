.. include:: ../README.rst
.. include:: ./javascriptexample.rst
.. code-block:: javascript
  :linenos:
   const fetch = require('node-fetch')

   async function makeUrl() {
   const params = {'url': 'https://youtube.com'}
   const data = await fetch('https://dushortener.herokuapp.com/api/shorten', {
   method: 'post',
   body: JSON.stringify(params),
   headers: {'Content-Type': 'application/json'}
   }).then((res => res.json()))

   console.log(data)
   }

   makeUrl();
