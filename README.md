# Indoor/Outdoor Air Quality Dataset - Commercial Campus (May 2023 – May 2025)

This dataset contains anonymized indoor and outdoor air quality data collected from a commercial campus over a 25-month period, from **May 2023 to May 2025**. It is hosted in **Google Cloud Storage (GCS)** at:

[gs://tellus-public-datasets/indoor-outdoor-commercial-campus/](https://console.cloud.google.com/storage/browser/tellus-public-datasets/indoor-outdoor-commercial-campus)


## Contents

Each file in the dataset corresponds to a calendar month and is named in the format:

```
YYYY-MM.csv
```

For example:

- `2023-05.csv`
- `2024-11.csv`
- `2025-05.csv`

## Data Schema

Each CSV file contains the following columns:

| Column      | Type   | Description                                  |
| ----------- | ------ | -------------------------------------------- |
| deviceid    | string | Anonymized ID of the monitoring device (A-Z) |
| timestamp   | string | ISO 8601 formatted timestamp (UTC)           |
| pm2_5       | float  | PM2.5 concentration (μg/m³)                  |
| temperature | float  | Temperature (°C)                             |
| humidity    | float  | Relative Humidity (%)                        |
| co2         | float  | CO2 concentration (ppm)                      |

> **Note:** Data is raw and uncorrected. Some records may contain missing or null values.

## Usage

To access the dataset using Google Cloud CLI:

```bash
gsutil ls gs://tellus-public-datasets/indoor-outdoor-commercial-campus/
```

To download a specific file:

```bash
gsutil cp gs://tellus-public-datasets/indoor-outdoor-commercial-campus/2025-01.csv .
```

## License

This dataset is released under the [MIT License](https://opensource.org/licenses/MIT):

```
MIT License

Copyright (c) 2025 Tellus

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Contact

For questions or feedback, please contact: \[[tom.becnel@tellusensors.com](mailto:tom.becnel@tellusensors.com)]

---

_This dataset is provided for research, analysis, and educational use. Please acknowledge the source when using it in your work._
