# Book Recommender System

Welcome to the Book Recommender System repository! This project is a web application designed to recommend books based on popularity. The machine learning model is trained to provide book recommendations, and the website is built using Flask for the backend.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Model Training](#model-training)
- [API Endpoints](#api-endpoints)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Features

- Recommend books based on popularity
- Simple and intuitive user interface
- Display book details including title, author, and summary
- Easy-to-use search functionality

## Technologies

- **Backend:** Flask
- **Frontend:** HTML, CSS, JavaScript (with Flask templates)
- **Machine Learning:** Popularity-based recommendation model (using pandas, numpy, scikit-learn)
- **Database:** CSV files for book data
- **Deployment:** Flask

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Python 3.7 or later
- pip (Python package installer)

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/Saifullah00/Book-Recommender-System.git
   cd book-recommender-system
   ```

2. Create a virtual environment:

   ```sh
   python -m venv venv
   ```

3. Activate the virtual environment:

   - On Windows:

     ```sh
     venv\Scripts\activate
     ```

   - On macOS/Linux:

     ```sh
     source venv/bin/activate
     ```

4. Install the required dependencies:

   ```sh
   pip install -r requirements.txt
   ```

## Running the Application

1. Start the Flask application:

   ```sh
   flask run
   ```

   The server will start at `http://localhost:5000`.

2. Open your browser and go to `http://localhost:5000` to access the Book Recommender System.

## Model Training

The machine learning model is based on a popularity-based recommendation system. Here are the steps to train the model:

1. Prepare the dataset (CSV files with book information and ratings).
2. Load and preprocess the data using pandas and numpy.
3. Train the popularity-based model using scikit-learn or custom algorithms.
4. Save the trained model for use in the Flask application.

The training script is located in the `model_training` directory. Run the script to train the model:

```sh
python model_training/train_model.py
```

## API Endpoints

### Book Endpoints

- **GET /api/recommendations**: Retrieve a list of recommended books
- **GET /api/books/{id}**: Retrieve details of a single book by ID

### Example Request and Response

#### GET /api/recommendations

Request:
```sh
curl -X GET http://localhost:5000/api/recommendations
```


## Screenshots

![Home Page](screenshots/home.png)
*Home page showing recommended books*

![Book Details](screenshots/book-details.png)
*Detailed view of a selected book*

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Thank you for checking out the Book Recommender System! If you have any questions or feedback, feel free to open an issue or contact the repository owner. Happy coding!
