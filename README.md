### Handwritten digits for MNIST validation



A couple of handwritten and slightly processed MNIST digits. Currently, there there are **172** digits.

---

To get the dataset already in a numpy array just run (**_note:_** every time the `urlretrieve` is run
it downloads the data and saves it to a temporary location):

```python
import numpy as np
from urllib.request import urlretrieve
filename, headers = urlretrieve(
    'https://github.com/Avatust/my-mnist-digits/raw/master/data/digits.npz')

with np.load(filename) as data:
    x_data = data['input_data']
    y_data = data['target_data']
```

---

Or clone the repo and process them yourself :)
