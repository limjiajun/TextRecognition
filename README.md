# Text Recognition Web App

This is a **client-side Optical Character Recognition (OCR) web application** using **Tesseract.js**. It allows users to upload images, extract text, and copy the recognized text to the clipboard.

## Features
- **Multiple Image Uploads**: Users can select and upload multiple images.
- **OCR with Tesseract.js**: Supports text recognition in multiple languages (English, Chinese, Spanish, French, German, etc.).
- **Progress Indicator**: Displays a progress bar while processing images.
- **Copy to Clipboard**: Click on the extracted text to copy it.
- **Image Preview**: Click on an image to view it in a modal along with extracted text.
- **Responsive UI**: Built with Bootstrap 5.

## Technology Stack
- **Frontend**: HTML, CSS (Bootstrap), JavaScript
- **OCR Engine**: [Tesseract.js](https://github.com/naptha/tesseract.js)

## Installation & Usage
### 1. Clone the Repository
```sh
git clone 
cd your-repo-name
```
### 2. Open `index.html`
Simply open the file in a browser:
```sh
open index.html
```
### 3. Upload an Image
- Click the file input to select an image.
- The system will automatically process and display extracted text.

### 4. View & Copy Text
- Click on the extracted text to copy it.
- Click on an image to view it in full screen.

## File Structure
```
/project-folder
│── index.html       # Main UI and OCR logic
```

## Customization
### Modify Supported Languages
You can customize the OCR languages by editing this part of the `index.html` file:
```js
Tesseract.recognize(imageSrc, 'eng+spa+fra+deu+chi_sim+chi_tra', {...});
```
Add or remove languages as needed.

## Known Issues & Limitations
- **OCR Accuracy**: Depends on image clarity.
- **Processing Speed**: Large images may take longer.
- **Browser Support**: Ensure the browser supports `Tesseract.js`.

## Future Enhancements
- Support for handwritten text recognition.
- Export extracted text as a file.
- Backend storage for processed text.

## License
This project is open-source and available under the [MIT License](LICENSE).
