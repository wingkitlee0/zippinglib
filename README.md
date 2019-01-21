# Tests for importing numpy and tensorflow from a zip archive


The ultimate goal is to run tensorflow using Amazon Lambda. However, due to the size restriction, we have to make the packages as small as possible. Since python does allow importing library from a zip archive, I am trying to make a zip for the python libraries used. It turns out that the method does not work directly as python does not import `*.so` from a zip file (see the discussion [here](https://stackoverflow.com/questions/43967630/importing-numpy-from-a-prebuilt-binary-zip))

