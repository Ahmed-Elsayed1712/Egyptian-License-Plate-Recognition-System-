🚗 Egyptian License Plate Recognition (Streamlit App)

A Streamlit-based web application for detecting and recognizing Egyptian vehicle license plates using YOLO models and custom OCR logic.

 🔍 Features

- Upload or capture an image using a camera
- Detect license plates in images using YOLO
- Perform OCR to extract Arabic characters and numbers
- Convert detected elements to Arabic format
- Automatically classify the governorate based on plate structure
- Bilingual interface: English and Arabic
- Download processed results as images
- python version >> 3.11

 🗂 Project Structure

```
project/
│
├── web/
│   ├── web.py              ← Main Streamlit app
│   ├── depiweb.py          ← Plate detection + OCR logic
│   ├── best.pt             ← OCR model
│   ├── plate.pt            ← License plate detector
│   ├── yolo11n.pt          ← Optional general object detector
│   └── requirements.txt    ← Dependencies
│
└── README.md
```

🚀 How to Run

1. Open a terminal and navigate to the `web` folder:

   ```bash
   cd web
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the following model files are in the same folder:
   - `best.pt`
   - `plate.pt`
   - `yolo11n.pt` (optional)

4. Start the app:

   ```bash
   python -m streamlit run web.py
   ```

5. The web app will open in your browser.

 📝 Notes

- Make sure your webcam permissions are allowed when using the "Use Camera" option.
- The app supports both English and Arabic interface (selectable at the top).
- Governorate classification is based on the recognized plate letters.

📄 License

MIT License.

🧪 Try It Out
You can test the license plate recognition system directly through the app:

Upload an Image

Use the sidebar or main interface to upload a clear photo of an Egyptian vehicle license plate.
Supported formats: .jpg, .png, .jpeg.
Use Camera (Optional)

If your device has a webcam, click the "Use Camera" button to capture a live image.
Allow camera permissions when prompted by your browser.
Process the Image

After uploading or capturing the image, click the "Detect and Recognize" button.
The app will:
Detect the license plate in the image
Run OCR to extract Arabic letters and digits
Display the recognized license plate
Show the corresponding governorate (if available)
Download Result

Click the download button to save the image with annotations locally.
[![image](https://github.com/user-attachments/assets/e29c3af8-16ed-4735-aaa1-ac1cd49d5ac9)](https://private-user-images.githubusercontent.com/189232387/443765121-d096f474-ef59-4dcf-9bac-4d5e0f881780.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDc1NzA0MjksIm5iZiI6MTc0NzU3MDEyOSwicGF0aCI6Ii8xODkyMzIzODcvNDQzNzY1MTIxLWQwOTZmNDc0LWVmNTktNGRjZi05YmFjLTRkNWUwZjg4MTc4MC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNTE4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDUxOFQxMjA4NDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04ZmE0YTFlNDA1OWUyYzcyZDNiNWRmZDVkODk0MzE5MWJiZDFmMDFmOTU3NDQ4YzEyYTEyOGM0M2QxMzEwZGVjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.-CQrzWIZQgMjyn2C6bKZiD8_I0FOtcipYUYHAU2VxHo)
[![Uploading image.png…]()](https://private-user-images.githubusercontent.com/189232387/444777617-a94404a4-976f-4dea-9003-3edacc8826d6.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDc1NzA0MjksIm5iZiI6MTc0NzU3MDEyOSwicGF0aCI6Ii8xODkyMzIzODcvNDQ0Nzc3NjE3LWE5NDQwNGE0LTk3NmYtNGRlYS05MDAzLTNlZGFjYzg4MjZkNi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNTE4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDUxOFQxMjA4NDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00MjE2YWE3YWQ5MjMwODA4MzZlMjZmNDYzMTU5YWE2NDAwMjc0NmY1YjM4YmZjZGMyMzNiOTBjMjNjNTM1YWE2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.RFBcj6OFsAqIHzyHd3MoINuOJcbeUYYb08qE_Qr5HlA)

 


