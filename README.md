# machine-learning-challenge
too bad it won't do my homework for me


Four models initally fit and tested (score)
    1. Logistic regression (.885)
    2. Random forest (.901)
    3. K nearest neighbors (.832)
    4. Supply vector machine (.860)
    
Grid Search
    1. LogReg: used following grid @ 8000 max_iter
        param_grid = {'C': [1, 5, 10],
                      'solver' :['lbfgs', 'saga']}
        Best fit and score: {'C': 1, 'solver': 'saga'}
                            0.8865129640006113
    2. RanFor: tuned n_estimators to 64 (.900)
               tuned max_depth: 18.0, Train/Test Score: 0.993/0.902


        source: https://medium.com/all-things-ai/in-depth-parameter-tuning-for-random-forest-d67bb7e920d

