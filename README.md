# DMED Test for Tashkent District

This project contains an HTML quiz application that loads questions from text files.

## How to Run

Due to browser security restrictions, opening `index.html` directly from your file system (`file:///.../index.html`) might prevent the quiz from loading the `.txt` files correctly. This is a common security feature in web browsers to prevent unauthorized access to local files.

To run this application, it is recommended to use a simple local web server. Here are a few options:

### Option 1: Using Python's Simple HTTP Server (Recommended)

If you have Python installed, you can easily start a web server from the project directory:

1.  Open your terminal or command prompt.
2.  Navigate to the `test11` directory where `index.html` and the `.txt` files are located:
    ```bash
    cd C:\Users\SUHROB\Desktop\test11
    ```
3.  Run the following command:
    ```bash
    python -m http.server
    ```
    (For Python 2, use `python -m SimpleHTTPServer`)
4.  Open your web browser and go to `http://localhost:8000`.

### Option 2: Using Node.js `serve` package

If you have Node.js and `npm` installed, you can use the `serve` package:

1.  Open your terminal or command prompt.
2.  Navigate to the `test11` directory:
    ```bash
    cd C:\Users\SUHROB\Desktop\test11
    ```
3.  If you don't have `serve` installed, install it globally:
    ```bash
    npm install -g serve
    ```
4.  Run the server:
    ```bash
    serve .
    ```
5.  Open your web browser and go to the address provided by `serve` (e.g., `http://localhost:5000`).

---

Now, you should be able to open `index.html` through the local server, and the quiz should load `1.txt`, `2.txt`, and `3.txt` without any "file not found" errors.
