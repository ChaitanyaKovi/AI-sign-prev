# AI Signature Verification System

This system uses Machine Learning (MLP Neural Network) to detect forged signatures.

## Project Structure
- `backend/` - Python Flask API and Machine Learning Model.
- `frontend/` - Modern HTML/JS User Interface.
- `data/` - Directory for training datasets.

## Setup & Installation

1.  **Install Dependencies**:
    ```bash
    pip install -r backend/requirements.txt
    ```

2.  **Prepare Data** (For training):
    - Collect a dataset of signatures.
    - Organize them into two folders:
        - `data/real/` (Genuine signatures)
        - `data/forged/` (Forged signatures)

3.  **Train the Model**:
    ```bash
    python backend/train.py
    ```
    This will save a `signature_model.pkl` file.

4.  **Run the Application**:
    ```bash
    python backend/app.py
    ```
    The server will start at `http://localhost:5000`.

5.  **Use the Interface**:
    - Open `frontend/index.html` in your browser.
    - Upload a signature image to verify it.

## Technology Stack
- **Frontend**: HTML5, CSS3 (Glassmorphism), JavaScript.
- **Backend**: Python, Flask.
- **AI/ML**: Scikit-Learn (MLPClassifier).
