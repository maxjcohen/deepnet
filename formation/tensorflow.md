Tensorflow installation - Ubuntu
======================================

1. Installation without GPU - pyton3 virtualenv
2. Installation with GPU - pyton3 virtualenv
3. Any other configuration

## 1. Installation without GPU - pyton3 virtualenv
We expect the user to be using on Ubuntu along with pyton3 installed with virtualenv. Start by entering your virtualenv :
```bash
$ workon tensorflow
```

The installation is very simple :
```bash
(tensorflow) $ pip install tensorflow
```
## 2. Installation with GPU - pyton3 virtualenv
*This part is more complicated, as it involves installing third party software. This may also take a while.*

Check the [tensorflow installation page](https://www.tensorflow.org/install/install_linux#nvidia_requirements_to_run_tensorflow_with_gpu_support) to get the list of requirements. Pay close attention to the required version for each package.

You can then pop into your virtualenv and install tensorflow with GPU support :
```bash
$ workon tf-gpu
(tf-gpu) $ pip install tensorflow-gpu
```

If the installation is succesfull, you can test  that tensorflow can use your GPU :
```python
>>> import tensorflow as tf
>>> tf.Session()
>>>...
```

The result should have information about your GPU.

## 3. Any other configuration

The [tensorflow installation page](https://www.tensorflow.org/install/) is pretty clear, if your used to installing software, you should be fine.
