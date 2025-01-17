# Hadith API

A API for hadiths in bengali language

From this API you will get:

- Hadith narrator
- Hadith number
- Hadith authenticity

API: https://bn-hadith-api.herokuapp.com/hadiths

To fetch data from this api you can use following examples:

### using Promise:

```
fetch('https://bn-hadith-api.herokuapp.com/hadiths/0')
  .then(response => response.json())
  .then(data => console.log(data));
```

### using Async/Await

```
async function () {
  const fetchAPI = fetch(`https://bn-hadith-api.herokuapp.com/hadiths/0`);
  const response = await fetchAPI;
  const data = await response.json();
  console.log(data);
}
```

**To contribute:**

- Fork the repository
- Clone the repository to your pc
- add hadith data to the following format:

```
{
"id": ,
"name": "",
"description": "",
"numbers": "",
"grade": ""
}

```

- keep track of **id**
- create pull request

**Thanks to [iHadis](http://ihadis.com/) for providing hadiths**
