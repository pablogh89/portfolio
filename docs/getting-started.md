# Getting Started

Welcome to my documentation text portfolio.

Here you can find some text samples to review my writing style.

## Installation

Here you can learn how to install the portfolio and run it locally.  

### Prerequisites

Make sure you have the following software installed:

- Python
- Git

### Operation

Follow these steps to install and run the portfolio locally:

1. Open a folder where you want to store the portfolio files.
2. Open a Command Prompt or Terminal on the folder in one of the following ways:

    - Open the Command Prompt or Terminal and navigate to the folder using the ``cd`` command.
    - Type ``cmd`` on the Address Bar of your File Explorer (Windows)
    - Right-click the folder and select **Open in Terminal** (Ubuntu)

3. Run the following command to clone the repository:

    ```shell
    git clone git@github.com:pablogh89/portfolio.git
    ```

4. Run the following command to open the portfolio folder:

    ```shell
    cd  portfolio 
    ```

5. Run the following command to install the project dependencies (Python packages required to run the project on your device):

    ```shell
    pip install -r requirements.txt
    ```

    !!! note
        If this fails due to access denied, add ``--user`` on Windows or start with ``sudo`` on Linux to solve the problem.

6. Run the following command to start the portfolio:

    ```shell
    python mkdocs serve 
    ```

    !!! note
        If this fails, try ``python –m mkdocs serve`` on Windows or ``python3 mkdocs serve`` on Linux to solve the problem.

7. Open a browser and navigate to ``http://localhost:8000/``
