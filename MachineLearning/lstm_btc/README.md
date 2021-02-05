# Machine learning pipeline with tensorflow serving

What I'm thinking is we first try to integrate into the Learning mines with a few scripts: 

* `model.js` which would be a method for the main LSTM model (this one already exists)
* `predict.js` which makes new predictions based on past models, saves a new version of each model in a folder
* `serve.js` which calls the newest version of the model created by `predict.js`

# Dependencies

Install tensorflow as root:
```
sudo npm install @tensorflow/tfjs-node --unsafe-perm=true --allow-root
```

# Credit for LSTM model

This code uses the `model.js` file in the repository https://github.com/jinglescode/time-series-forecasting-tensorflowjs as a baseline for creating the LSTM model