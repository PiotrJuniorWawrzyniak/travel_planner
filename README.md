# TRAVEL PLANNER

An application for planning and organizing trips with detailed route segmentation.

## Description

- **Plan your trip:** Create a travel plan by defining a route with multiple segments. Each segment can have a different mode of transport (e.g., bus, train, bike, plane).
- **Interactive map:** Use an interactive map powered by OpenStreetMap and Leaflet.js to visualize your trip and manage its segments.
- **Save and manage trips:** Store your planned trips in a local MySQL database for future reference and editing.

This project is built using **Pyramid** (for the backend) and **Angular** (for the frontend). Pyramid handles server-side logic and API endpoints, while Angular powers the user interface. OpenStreetMap and Leaflet.js are used for map rendering and interactivity.

## Requirements

- Python 3.8 or higher
- Node.js (for frontend development)
- MySQL (for data storage)
- A virtual environment (for Python dependencies)
- npm (Node.js package manager)

## Installation

1. Clone the repository:
    ```sh
    git clone <repository_url>
    cd travel_planner
    ```

2. Set up a virtual environment and install the required Python packages:
    ```sh
    python -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    pip install -r requirements.txt
    ```

3. Set up the MySQL database:
    - Create a database named `travel_planner` in your MySQL instance.
    - Update the database configuration in your Pyramid project's `.ini` file (e.g., `development.ini`).

4. Navigate to the `frontend/` folder and install Node.js dependencies:
    ```sh
    cd frontend
    npm install
    ```

5. Run the backend server:
    ```sh
    pserve development.ini --reload
    ```

6. Run the frontend development server:
    ```sh
    npm run start
    ```

7. Access the application:
    - Open your browser and navigate to `http://localhost:6543` for the backend API (Pyramid documentation, if applicable).
    - The frontend (Angular) will be accessible at `http://localhost:4200`.

## Usage

1. **Plan a trip:**
   - Use the map to define your route by adding start, end, and intermediate points.
   - Assign a mode of transport for each segment of your trip.

2. **Save your trip:**
   - Save the planned route to the database for future reference.

3. **View and manage saved trips:**
   - Browse a list of previously saved trips and edit or delete them as needed.

4. **Interactive map:**
   - Visualize your trip on a map, with each segment clearly marked.

## Author

- Piotr Wawrzyniak - [piotrjuniorwawrzyniak@gmail.com](mailto:piotrjuniorwawrzyniak@gmail.com)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
