
<h1 align="center">Welcome COVID-19 Dashboard👋</h1>

<img alt="COVID-19" src="http://covid19-angular-express.s3-website.us-east-2.amazonaws.com/assets/images/covid-19.png" />

### 🏠 [Homepage](https://github.com/richcheng/covid19-angular)

### ✨ [Demo](https://richcheng.com/covid19)


## Screenshots

<img alt="COVID-19 Dashboard Screenshot-world" src="http://covid19-angular-express.s3-website.us-east-2.amazonaws.com/assets/screenshots/sc1.png" />
<img alt="COVID-19 Dashboard Screenshot-USA" src="http://covid19-angular-express.s3-website.us-east-2.amazonaws.com/assets/screenshots/sc2.png" />

## Build the Angular project

```sh
npm install
```

```sh
ng build
```


## Run the Angular Project

```sh
npm install
```

```sh
ng serve
```

## Run the Node.js Project (open server folder)

Rename config.example.json to config.json and fill in the details

```
{
  "redis": {
    "host": "host",
    "password": "1234"
  },
  "keys": {
    "all": "coronastatistics:all",
    "countries": "coronastatistics:countries",
    "timeline": "coronastatistics:timeline",
    "timelineglobal": "coronastatistics:timelineglobal"
  },
  "interval": 600000
}
```

```sh
npm install
```

```sh
node server.js
```
Edit src/app/core/services/getdata.service.ts and replace with your own api url.

```
  private host = "https://api.coronastatistics.live"
```

# API Endpoints

* http://api.coronastatistics.live/all
* http://api.coronastatistics.live/countries
* http://api.coronastatistics.live/countries?sort={parameter}
* http://api.coronastatistics.live/countries/{country_name}
* http://api.coronastatistics.live/timeline
* http://api.coronastatistics.live/timeline/global
* http://api.coronastatistics.live/timeline/{country_name}

