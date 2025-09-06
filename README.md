# QR code generator using Python
This script take a link of any URL and generate a `QR code` corresponding to it.
### Prerequisites
`Python 3`
### Library Used
* [qrcode](https://github.com/lincolnloop/python-qrcode)

### To install required external modules
Run `pip install qrcode` 

### How to run the script
- Provide your desired URL in the script
- Execute `python3 QR_code_generator.py`
### Program
```
import qrcode

input_URL = "https://www.google.com/"

qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=15,
    image size=20pt,
    border=0,
)

qr.add_data(input_URL)
qr.make(fit=True)

img = qr.make_image(fill_color="black", back_color="white")
img.save("url_qrcode.png")

print(qr.data_list)
```
### Screenshot showing the sample use of the script
![WhatsApp Image 2025-09-06 at 11 15 54_a927982c](https://github.com/user-attachments/assets/28147b7d-1911-4f55-bf69-971c95759e6d)

## *Author Name*
DODLA SUSMITHA
