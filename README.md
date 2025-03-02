# Text-to-QR-Code Generator API

This API allows you to generate QR codes from text input. It provides a simple HTTP endpoint where you can send a text parameter, and the API will return a QR code image encoded with the provided text.

## Usage

### Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/your-username/your-repo.git
   ```
   
   Install the required dependencies:
  ```shell
  go mod download
  ```
2. Starting The API

1. Navigate to the project directory:
```shell
cd your-repo
```
2. Run the following command to start the API-server 
```shell
go run main.go
```
This will start server on "http://localhost:8080"

### API Endpoint

The API provides a single endpoint for generating QR codes.
    POST /generate: Generates a QR code from the provided text. The text should be sent as a parameter in the request.

### Example

You can use cURL to test the API endpoint:
curl -X POST -d "text=Hello World" http://localhost:8080/generate
The API will respond with the generated QR code image.
Dependencies

This API uses the following dependencies:

    github.com/skip2/go-qrcode: A Go package for generating QR codes.

Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request. Ensure that you follow the existing code style and maintain appropriate documentation.

License

This project is licensed under the MIT License.
