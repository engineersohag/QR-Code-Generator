# QR Code Generator

A simple QR code generator using HTML, CSS, and JavaScript. Enter any text or URL, and generate a QR code instantly!

## Features
- Enter any text or URL to generate a QR code.
- Visual feedback if the input is empty.
- Easy to use and lightweight.

## Demo
![QR Code Generator Screenshot](https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=https://www.fiverr.com/engineer_sohag)

## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/qr-code-generator.git
    ```

2. Navigate to the project directory:
    ```bash
    cd qr-code-generator
    ```

3. Open `index.html` in your web browser.

## Code
        let imgBox = document.getElementById("imgBox");
        let qrImg = document.getElementById("qrImg");
        let qrText = document.getElementById("qrText");

        // QR Code API: https://goqr.me/api/

        function generateQR(){ 
          qrImg.src = "https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=" + qrText.value;
          imgBox.classList.add("show-img");
