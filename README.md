# Go Server with Form Handling

This is a simple Go server that serves static files and handles form submissions. It listens on port 8080 and has two main handlers: one for serving static files and the other for handling form submissions. Additionally, there is a simple "Hello" endpoint for demonstration purposes.

## Installation and Usage

1. Make sure you have Go installed on your machine.

2. Download or clone the repository containing the `main.go` file.

3. Navigate to the project directory.

4. Run the following command to start the server:

   ```bash
   go run main.go
   ```

5. The server will start, and you can access it by opening a web browser and visiting `http://localhost:8080`.

## Endpoints

### Static File Server

The server serves static files from the `./go-server/static` directory. When you visit the root path or any other valid file path, it will try to locate the file in the `static` directory and serve it if found.

### Form Handler

The form handler is accessible at `/form`. It supports POST requests and handles form submissions. It expects two fields, `name` and `address`, to be submitted in the form data. Upon successful submission, it will respond with the data received from the form.

### Hello Endpoint

The "Hello" endpoint is accessible at `/hello`. It only supports GET requests and responds with a simple greeting message: "Hello! Welcome to the server."

## Code Structure

The `main.go` file contains the code for the Go server and its handlers. Here is a brief overview of the functions:

- `formHandler`: Handles form submissions and extracts the `name` and `address` fields from the form data.

- `helloHandler`: Handles GET requests to the `/hello` endpoint and sends a welcome message.

- `main`: The main function sets up the static file server and defines the endpoints for form handling and the "Hello" message. It starts the server and listens for incoming requests on port 8080.

## Contributing

If you find any issues with the server or have suggestions for improvements, feel free to open an issue or submit a pull request on the repository.

## License

This Go server is open-source and distributed under the [MIT License](LICENSE). Feel free to use, modify, and share it according to the terms of the license.
