# MLOPS

## Practice 1.

To run the code, follow these steps:

1. Clone the repository using the command `git clone` and navigate to the project directory `cd mlops-demo`.
2. Install the dependencies from the `requirements.txt` file located in the project root by running `pip install -r requirements.txt`.
3. Navigate to the `lab1` directory using `cd lab1`.
4. Look into the `job.sh` script, and if you need the data generated after running the script in the future, comment out the last line `python3 ./lab1/cleaner.py` since it clears the system of the generated data.
5. Next, run the `job.sh` script with the command `./job.sh`, ensuring it's executable by checking with `ls -la` and using `chmod u+x job.sh` if necessary.

To run individual scripts from the initial directory up to step 4:

1. Run `python3 ./lab1/data_creation.py` to generate data and save them in the respective training and test/validation files.
2. Run `python3 ./lab1/model_preprocessing.py` to prepare the data for further processing.
3. Run `python3 ./lab1/model_preparation.py` to create and train a model on the training data, then save it in a separate file.
4. Run `python3 ./lab1/model_testing.py` to test the model's metrics on the test data.
