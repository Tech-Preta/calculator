# Simple Calculator

This is a simple calculator implemented using HTML, CSS, and JavaScript. It is served using Nginx in a Docker container.

## Project Structure

```
/
├── docker/
│   ├── Dockerfile
│   └── nginx.conf
├── src/
│   ├── index.html
│   ├── style.css
│   └── script.js
└── README.md
```

## How to Build and Run

1. Clone this repository.
2. Navigate to the `docker/` directory.
3. Build the Docker image:

   ```sh
   docker build -t simple-calculator .
   ```

4. Run the Docker container:

   ```sh
   docker run -d -p 8080:80 simple-calculator
   ```

5. Open your browser and navigate to `http://localhost:8080` to see the calculator.

## Acknowledgements

This project was created as a simple example to demonstrate the use of HTML, CSS, JavaScript, and Docker.
