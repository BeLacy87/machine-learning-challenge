# machine-learning-challenge
too bad it won't do my homework for me


Four models initally fit and tested (score)

1. Logistic regression (.885)

2. Random forest (.901)

3. K nearest neighbors (.832)

4. Supply vector machine (.860)
    
Grid Search
1. LogReg: used following grid @ 8000 max_iter
   param_grid = {'C': [1, 5, 10],'solver' :['lbfgs', 'saga']}
   Best fit and score: {'C': 1, 'solver': 'saga'} 0.8865129640006113
        dropped error columns: (.815)

   2. RanFor: tuned n_estimators to 64 (.900)
               tuned max_depth: 18.0, Train/Test Score: 0.993/(0.902)
               source: https://medium.com/all-things-ai/in-depth-parameter-tuning-for-random-forest-d67bb7e920d
        param_grid= {'n_estimators': [32, 64, 100],
              'max_depth': [16,17,18,19,20]}
        Best fit and score:{'max_depth': 18, 'n_estimators': 100}
                            0.892997329335827
        best accuracy is coming from using all default parameters (0.899-0.905)
    

