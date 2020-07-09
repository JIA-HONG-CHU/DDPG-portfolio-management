# DDPG for portfolio management

# Datasets

## Datasets preprocessing

### Run
```
DRL_Data_Preprocessing.ipynb
```

## Train DDPG model

## Training

### Run

```bash
python stock_trading.py -p lstm  -w 6 -b True -ts 20050301 -te 20161101
```
#### Usage

```
* -d print debug statement, default False
* -p predictor type, cnn or lstm
* -w observation window length, digit
* -b whether to use batch normalization, True or False
* -r rollout steps, default 2
* -s batch size, default 10
* -ts training set start date, betweeen 20050301 and 20161101'
* -te training set end date, betweeen 20050301 and 20161101'

```

## Results 

### Run 
```
ddpg_experiment.ipynb  #Get the portfolio weights during the training time

choose_specific_stocks_train.ipynb  #Get the name of specific stocks

train_choose_stocks.ipynb #Converting specific stocks information to real prices
```

### Then run
```
plot_the_result_of_testing_data_Training.ipynb
```
<img src='./imgs/training.png' width="800px"/>

<img src='./imgs/training_market.png' width="600px"/>

<img src='./imgs/training_specific.png' width="600px"/>

## Testing

## Results

### Run 
```
ddpg_experiment.ipynb  #Get the portfolio weights during the testing time

choose_specific_stocks_test.ipynb  #Get the name of specific stocks

test_choose_stocks.ipynb #Converting specific stocks information to real prices
```
### Then run 
```
plot_the_result_of_testing_data_Testing.ipynb
```
<img src='./imgs/testing.png' width="600px"/>

<img src='./imgs/testing_market.png' width="600px"/>

<img src='./imgs/testing_specific.png' width="600px"/>



# Reference
* Code is from https://github.com/sino30535/DDPG-portfolio-management
