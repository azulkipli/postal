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
curl -XGET '<a href="https://flik-postal.app/?q=bojongsoang">http://localhost:3000/search/?q=bojongsoang</a>'
</pre>

#### Response

```json
{
  "statusCode": 200,
  "code": "OK",
  "data": [
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Bojongsoang",
      "village": "Bojongsoang",
      "postalcode": "40288",
      "code": "40288"
    },
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Tegalluar",
      "village": "Tegalluar",
      "postalcode": "40287",
      "code": "40287"
    },
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Bojongsari",
      "village": "Bojongsari",
      "postalcode": "40288",
      "code": "40288"
    },
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Lengkong",
      "village": "Lengkong",
      "postalcode": "40287",
      "code": "40287"
    },
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Cipagalo",
      "village": "Cipagalo",
      "postalcode": "40287",
      "code": "40287"
    },
    {
      "province": "Jawa Barat",
      "city": "Bandung",
      "regency": "Bandung",
      "subdistrict": "Bojongsoang",
      "district": "Bojongsoang",
      "urban": "Buahbatu",
      "village": "Buahbatu",
      "postalcode": "40287",
      "code": "40287"
    }
  ]
}
```


### License

This project is licensed under [Apache 2.0 License](https://github.com/azulkipli/postal/blob/main/LICENSE).
