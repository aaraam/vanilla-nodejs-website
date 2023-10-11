# Vanilla Node.JS project - node farms: Product Overview
`Made entirely for self reference`

This project is a basic Node.js application that serves a product overview page, individual product pages, and an API endpoint to fetch product data.

## Topics Covered

1. **Node.js Basics**: Setting up a basic Node.js server using the `http` module.
2. **File System Operations**: Reading files synchronously using the `fs` module.
3. **URL Parsing**: Extracting query parameters and pathnames from URLs using the `url` module.
4. **Template Rendering**: Using a simple templating function to replace placeholders in HTML templates with actual data.
5. **JSON Data Handling**: Reading and parsing JSON data to serve it through the server.
6. **Routing**: Handling different routes like the overview page, product page, and API endpoint.
7. **Response Headers**: Setting up response headers for different content types and custom headers.

## Project Structure

- **Server Setup**: The main server is set up in the root file, where it listens on port 8000.
- **Templates**: HTML templates for the overview and individual product pages are stored in the `templates` directory.
- **Data**: Product data is stored in a JSON file (`data/data.json`).
- **Modules**: Custom modules, like the `replaceTemplate` function, are stored in the `modules` directory.

## How to Run

1. Ensure you have Node.js installed on your machine.
2. Navigate to the project directory.
3. Run the server using the command:
   ```bash
   node index.js
   ```
4. Open a browser and navigate to `http://127.0.0.1:8000/` to view the product overview page.
5. For individual product pages, navigate to `http://127.0.0.1:8000/product?id=<product_id>`. Replace `<product_id>` with the desired product's ID (e.g., 0, 1, 2, etc.).
6. To access the API endpoint and fetch the product data in JSON format, navigate to `http://127.0.0.1:8000/api`.

## Features

- **Overview Page**: Displays a list of all products with brief details.
- **Product Page**: Displays detailed information about a specific product.
- **API Endpoint**: Provides raw product data in JSON format.

## Future Enhancements

- Implement a more robust templating engine like EJS or Handlebars.
- Add error handling for invalid product IDs or missing data.
- Integrate a database for more dynamic data storage and retrieval.

## Dependencies

- Node.js core modules: `fs`, `http`, and `url`.