# SS-DiffAge
To make a prediction follow these steps

1. Clone the repo by running: 
    ```
    git clone https://github.com/A-Ijishakin/SS-DiffAge.git
    ```
2. Make a virtual environment either natively in python by running:
    ```
    pip install virtualenv 
    ```
    ```
    virtualenv SS-DiffAge
    ``` 
    Or in conda by running:
    ```
    conda create -n SS-DiffAge
    ```
3. Activate that environment
    Native Python:
    ```
    source ./SS-DiffAge/bin/activate 
    ```
    Conda:
    ```
    conda activate SS-DiffAge
    ```

4. Install all of the neccessary dependencies by running: 
    ```
    pip install -r requirement.txt
    ``` 

5. Change into the SS-DiffAge directory:
    ```
    cd SS-DiffAge
    ``` 
6. Run the prediction script:
    ```
    python3 predict.py --data_dir <directory with niftis> --slice <the slice number that you will predict on> --ext <file extension e.g: .nii or .nii.gz>
    ``` 

The above script will download the model weights and save the predictions to a CSV called: predicted_ages.csv. This file will have two columns: ID and predicted age. 