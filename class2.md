Describe (in plain English) what Array.map() does

The map() method creates a new array with the results of calling a function for every array element. The map() method calls the provided function once for each element in an array, in order. map() does not execute the function for empty elements. map() does not change the original array.


Describe (in plain English) what Array.reduce() does

The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.

Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
     
      const superagent = require('superagent');

      superagent
        .post('/api/pet')
        .send({ name: 'Manny', species: 'cat' }) // sends a JSON post body
        .set('X-API-Key', 'foobar')
        .set('accept', 'json')
        .end((err, res) => {
          // Calling the end function will send the request
        });

     


With normal Promise .then() syntax


            const superagent = require('superagent');

            superagent
            .post('/api/pet')
            .send({ name: 'Manny', species: 'cat' }) // sends a JSON post body
            .set('X-API-Key', 'foobar')
            .set('accept', 'json')
            .end((err, res) => {
              // Calling the end function will send the request
            });

          // promise with then/catch
          superagent.post('/api/pet').then(console.log).catch(console.error);
      
Again with async / await syntax


          const superagent = require('superagent');

          // callback
          superagent
            .post('/api/pet')
            .send({ name: 'Manny', species: 'cat' }) // sends a JSON post body
            .set('X-API-Key', 'foobar')
            .set('accept', 'json')
            .end((err, res) => {
              // Calling the end function will send the request
            });

          // promise with then/catch
          superagent.post('/api/pet').then(console.log).catch(console.error);

          // promise with async/await
          (async () => {
            try {
              const res = await superagent.post('/api/pet');
              console.log(res);
            } catch (err) {
              console.error(err);
            }
          })();
          
          
Explain promises as though you were mentoring a Code 301 level student


A promise is an object that may produce a single value some time in the future : either a resolved value, or a reason that it's not resolved (e.g., a network error occurred). A promise may be in one of 3 possible states: fulfilled, rejected, or pending


Are all callback functions considered to be Asynchronous? Why or Why Not?

Callbacks that you call yourself are regular function calls, which are always synchronous. Certain native APIs (eg, AJAX, geolocation, Node. js disk or network APIs) are asynchronous and will execute their callbacks later in the event loop


