![@azulkipli/kodepos](https://socialify.git.ci/azulkipli/postal/image?description=1&descriptionEditable=Indonesian%20postal%20code%20search%20API%20by%20place%20name%2C%20village%20or%20city.&font=Raleway&forks=1&issues=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2Ftwitter%2Ftwemoji%2Fmaster%2Fassets%2Fsvg%2F1f4ee.svg&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Dark)

## Requirements

- Node.js `>= 18.18.0`
- Yarn `>= 1.22.0`

## Getting Started

1. Clone this repository

   ```bash
   git clone https://github.com/azulkipli/postal.git
   ```

2. Move to the repository directory

   ```bash
   cd kodepos
   ```

3. Install dependencies

   ```bash
   yarn install
   ```

4. Run locally

   - Development mode

     ```bash
     yarn dev
     ```

   - Production mode

     1. Build first

        ```bash
        yarn build
        ```

     2. Start the app

        ```bash
        yarn start
        ```


## Basic Usage

Base URL : [`http://localhost:3000`](https://flik-postal.vercel.app)

| Endpoint                                       | Description                     | Parameter | Method |
| ---------------------------------------------- | ------------------------------- | --------- | ------ |
| [`/search`](https://flik-postal.vercel.app/search) | To find postcode using keywords | `q`       | `GET`  |

### Example of Use

#### Request

<pre>
curl -XGET '<a href="https://flik-postal.app/?q=bojong">http://localhost:3000/search/?q=bojong</a>'
</pre>

#### Response

```json
{
  "statusCode": 200,
  "code": "OK",
  "data": [
    {
      "province": "Jawa Tengah",
      "regency": "Purbalingga",
      "district": "Karangjambu",
      "village": "Danasari",
      "code": "53357"
    },
    {
      "province": "Jawa Tengah",
      "regency": "Tegal",
      "district": "Bojong",
      "village": "Danasari",
      "code": "52465"
    },
    {
      "province": "Jawa Tengah",
      "regency": "Pemalang",
      "district": "Pemalang",
      "village": "Danasari",
      "code": "52314"
    },
    {
      "province": "Jawa Barat",
      "regency": "Ciamis",
      "district": "Cisaga",
      "village": "Danasari",
      "code": "46386"
    }
  ]
}
```


### License

This project is licensed under [Apache 2.0 License](https://github.com/azulkipli/postal/blob/main/LICENSE).
