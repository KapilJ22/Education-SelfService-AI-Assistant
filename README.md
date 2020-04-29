

1. Clone (or fork) this repository, and go to the new directory

2. Install [Node.js](https://nodejs.org) (Versions >= 6).

3. In the root directory of your repository, install the dependencies.
```bash
npm install
```

4. Create a `credentials.json` in the top-level directory as below. Replace with your URL and apkikey.

```
{
  "discovery": [
    {
      "name": "Discovery-id",
      "plan": "lite",
      "credentials": {
        "url": <discovery url>,
        "apikey": <your api key>,
        "iam_apikey_name": "Auto-generated service credentials"
      }
    }
  ]
}
```

### Convert each row in the.csv file to .json file
 - Copy contents of csv file to test-data.csv. (test-data.csv file) is present in the top level directory.
 - Run below command
 ```
 node read-file.js 
 ```
- Verify JSON files are created in `./manualdocs` directory.

### Train Watson Services
Run following command to train Discovery services:
``` bash
  npm run train
`
