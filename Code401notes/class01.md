# Class 01 Read

1. Describe (in plain English) what Array.map() does

- array.map loops over an array and returns a new array of the same length. Results could be anything we want based on the function set in the parameter.

2. Describe (in plain English) what Array.reduce() does

- array.reduce reduces an array to a single value. It uses a callback function called a "reducer" on each element of the array and results in the single output value

### Examples: 
- Use when you want to add the amounts of numbers in the array
- Finding an average
- Flattening an array of arrays

3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

- With normal Promise .then() syntax

````javascript
superagent
      .get(url)
      .query(query)
      .then(superagentResults => {
        const movieResults = superagentResults.body.results;
        const movieArray = movieResults.map(movie => new Movie (movie));
        cache[movie] = movieArray;
        response.status(200).send(movieArray);
      })
      .catch(error => {
        console.log(error);
        response.status(404).send('page not found');
      });
````


- Again with async / await syntax

````javascript
Data.handleAPICall = async (req, res) => {
  const url = `https://rws-cards-api.herokuapp.com/api/v1/cards/random?n=3`;
  const cardResults = await superagent.get(url)
      const cardResults = superagentResults.body.cards;
      console.log('card results: ', cardResults);
      res.status(200).send(cardResults);
    })
    .catch(function (error) {
      console.log('something went wrong with superagent call in movies');
      res.status(500).send('we messed up');
    })
}
````

4. Explain promises as though you were mentoring a Code 301 level student

- Javascript is single threaded meaning it executes code in order and must finish executing one code block before moving on to the next. Promises is the eventual completion (or failure) of an asynchronous operation and its resulting value.

5. Are all callback functions considered to be Asynchronous? Why or Why Not?

- Callbacks are not considered asynchronous. It can be asynchronous if the function returns a promise
