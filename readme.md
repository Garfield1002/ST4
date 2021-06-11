<p align="center">
  <a href="https://us.pg.com/" target="_blank">
    <img width="150" src="https://upload.wikimedia.org/wikipedia/fr/thumb/d/d3/Procter_%26_Gamble_2013_%28logo%29.png/1920px-Procter_%26_Gamble_2013_%28logo%29.png" alt="logo">
  </a>
</p>

<h2 align="center">ST4 data@web, EI P&G</h2>

---

## 🔎 Description

In order to better advertise P&G's new `Fairy Pods`, we will try to determine if users do or do not have a dishwasher based on data collected by P&G.

## 📚 Description

More information about the cleaning process is available [here](Cleaning/readme.md).

More information about the models is available [here](Models/readme.md).

## 🧪 Usage

1. Extract `DS_CentraleSupelec_ST42021.zip` to `DS_CentraleSupelec_ST42021` in the root directory
2. Create an empty `data` folder in the root directory
3. Your project should look like this

```bash
|-- Cleaning
|
|-- data
|
|-- DS_CentraleSupelec_ST42021
|    |-- DS_Centrale_test.csv
|    |-- DS_Centrale_train.csv
|    |-- ...
|
|-- Models
|    |-- ...
|
|-- .gitignore
|-- License
|-- readme.md
|-- requirements.txt
```

5. You can install the required python packages using the `requirements.txt`
6. Run `Cleaning\cleanData.ipynb` it should generate 2 files in the `data` folder: `train.csv` and `test.csv`.
7. You should now be able to run any models in the `Models` directory

## 👋 Our Group 8

| Name  |                      Github                       |
| :---: | :-----------------------------------------------: |
| Paul  |    [paulpacaud](https://github.com/paulpacaud)    |
| Jack  |  [Garfiled1002](https://github.com/Garfield1002)  |
| Anna  |  [AnnaGrigoriu](https://github.com/AnnaGrigoriu)  |
| Mateo | [mateodufresne](https://github.com/mateodufresne) |
| Clea  |   [cleachataig](https://github.com/cleachataig)   |

## ⚖ License

[MIT License](License)
