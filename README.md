# Facial Expression Recognition 😊

## **1. Methodology 📊**
<img src="https://user-images.githubusercontent.com/7460892/207003643-e03c8964-3f16-4a62-9a2d-b1eec5d8691f.png" width="80%" height="80%">

## **2. Description 📖**
<img src="https://user-images.githubusercontent.com/7460892/207003772-ba2061bc-f8fd-4479-ba42-4712328b7085.png" width="80%" height="80%">

## **3. Input / Output 🔄**
<img src="https://user-images.githubusercontent.com/7460892/207004091-8f67548d-50ac-49c3-b7cb-ef8ec18a6491.png" width="40%" height="40%">


## **4. Code Snippet 💻**
```python
!pip install landingai &> /dev/null

from PIL import Image
from landingai.predict import Predictor

# Enter your API Key
endpoint_id = "344238dc-6021-4fdf-bd19-0d472ebea2fb"
api_key = "land_sk_7vbknaaQlplyOwi8TSC5GiFwutFjA6V8oNqfDpwc3lS6C08E8V"

# Load your image
image = Image.open("/content/WIN_20240620_12_06_00_Pro.jpg")

# Run inference
predictor = Predictor(endpoint_id, api_key=api_key)
predictions = predictor.predict(image)
predictions

