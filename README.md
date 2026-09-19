# AcquaConto

Personal web app (PWA) to split a shared water bill among housemates by meter reading.

- Enter the bill amount, the estimated consumption (m³), and each person's current meter reading.
- The previous reading auto-fills from the last saved month.
- Price per m³ = bill ÷ real consumption (togglable to ÷ estimated).
- Each person pays their consumption × price, at exact cents.
- Shows the refund expected from the water company.
- Bilingual Italian / English, light & dark themes, monthly history.

All data is stored locally in the browser on the device. Nothing is sent anywhere.

## Run locally
Serve the folder over http (service workers need http/https, not file://):

```
python3 -m http.server 8123
```

Then open http://localhost:8123/

## Deploy
Static site — host the folder as-is (e.g. GitHub Pages).
