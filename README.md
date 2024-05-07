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

## Final practice
<details>

### Цель проекта: разработать конвеер машинного обучения data-продукта (Web или API приложение).

Команда проекта. Проект выполняется в команде из 3-4 человека.

Требования к реализации проекта:
1. Исходные коды проекта должны находиться в репозитории GitHub.
2. Проект оркестируется с помощью ci/cd (jenkins или gitlab).
3. Датасеты версионируются с помощью dvc и синхронизируются с удалённым хранилищем.
4. Разработка возможностей приложения должна проводиться в отдельных ветках, наборы фичей и версии данных тоже.
5. В коневеере запускаются не только модульные тесты, но и проверка тестами на качество данных.
6. Итоговое приложение реализуется в виде образа docker. Сборка образа происходит в конвеере.
7. В проекте может использоваться предварительно обученная модель. Обучать собственную модель не требуется.

</details>
