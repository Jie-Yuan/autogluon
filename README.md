

<div align="left">
  <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
</div>

## AutoML Toolkit for Deep Learning

[![Build Status](http://ci.mxnet.io/view/all/job/autogluon/job/master/badge/icon)](http://ci.mxnet.io/view/all/job/autogluon/job/master/)
[![Pypi Version](https://img.shields.io/pypi/v/autogluon.svg)](https://pypi.org/project/autogluon/#history)

AutoGluon automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications.  With just a few lines of code, you can train and deploy high-accuracy deep learning models on tabular, image, and text data. 

```python
# First install package from terminal:  pip install mxnet autogluon

from autogluon import TabularPrediction as task
train_data = task.Dataset(file_path='https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
test_data = task.Dataset(file_path='https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
predictor = task.fit(train_data=train_data, label='class')
performance = predictor.evaluate(test_data)
```

See the [AutoGluon Website](http://autogluon.mxnet.io/index.html) for instructions on:
- [Installing AutoGluon](http://autogluon.mxnet.io/index.html#installation)
- [Learning with tabular data](http://autogluon.mxnet.io/tutorials/tabular_prediction/tabular-quickstart.html)
- [Learning with image data](http://autogluon.mxnet.io/tutorials/image_classification/beginner.html)
- [Learning with text data](http://autogluon.mxnet.io/tutorials/text_classification/beginner.html)
- More advanced topics such as [Neural Architecture Search](http://autogluon.mxnet.io/tutorials/nas/index.html)

## License

This library is licensed under the Apache 2.0 License.
