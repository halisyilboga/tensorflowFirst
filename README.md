## Synopsis

Derin öğrenme  2016 dersi için örnek tensorflow sunum codları.



## Motivation
 Anlattığım kodların incelenebilir olması için .ipynb  'notebook' formatını da github ekleyip paylaşmayı uygun buldum. Adım adım hem bir filtre oluşturma hemde örnek bir network'ün ağırlıklarını inceleme anlatılmıştır. 

githubtan indirildikten sonra dosyalar jupyter notebookta direk çalıaşcak şekilde ayarlanmıştır. Tensorflow'un öncesinde kurulu olması gerekmektedir. 

gerekli olan network dosyaları da otomatik indirelecektir. Libs klasöründe gerekli yardımcı fonksiyonlar mevcut. 

Anlattığım kodların incelenebilir olması için '.ipynb'  (jupyter notebook) formatını da github eklemeyi ve paylaşmayı uygun buldum. Adım adım hem bir filtre oluşturma hem de sonrasında örnek bir yapay sinir ağının (google inception network) ağırlıklarını incelemenmesi anlatılmıştır. 

github'tan indirildikten sonra dosyalar jupyter notebookta direk çalışacak şekilde ayarlanmıştır. Tensorflow'un öncesinde kurulu olması gerekmektedir. 

gerekli olan Google Inception Ağ dosyası ve etiketler otomatik otomatik ineceği için manuel indirmeye gerek yoktur. 

https://github.com/halisyilboga/tensorflowFirst/tree/master

## Installation
Kütüphanaler ile tektek uğraşmak istenmiyor ise aşağıdaki komut note defterine yapıştrılarak bütün bağlı kütüphanelerin kurulması sağlanabilir. 
```
# First check the Python version
import sys
if sys.version_info < (3,4):
    print('You are running an older version of Python!\n\n',
          'You should consider updating to Python 3.4.0 or',
          'higher as the libraries built for this course',
          'have only been tested in Python 3.4 and higher.\n')
    print('Try installing the Python 3.5 version of anaconda'
          'and then restart `jupyter notebook`:\n',
          'https://www.continuum.io/downloads\n\n')

# Now get necessary libraries
try:
    import os
    import numpy as np
    import matplotlib.pyplot as plt
    from skimage.transform import resize
    from skimage import data
    from scipy.misc import imresize
    from scipy.ndimage.filters import gaussian_filter
    import IPython.display as ipyd
    import tensorflow as tf
    from libs import utils, gif, datasets, dataset_utils, nb_utils
except ImportError as e:
    print("Make sure you have started notebook in the same directory",
          "as the provided zip file which includes the 'libs' folder",
          "and the file 'utils.py' inside of it.  You will NOT be able",
          "to complete this assignment unless you restart jupyter",
          "notebook inside the directory created by extracting",
          "the zip file or cloning the github repo.")
    print(e)

# We'll tell matplotlib to inline any drawn figures like so:
%matplotlib inline
plt.style.use('ggplot')
```

## License

A short snippet describing the license (MIT, Apache, etc.)
