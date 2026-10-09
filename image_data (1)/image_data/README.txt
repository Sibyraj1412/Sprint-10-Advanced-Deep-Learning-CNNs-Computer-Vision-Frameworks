IMAGE DATA FOLDER
=================
fashion_mnist/            Fashion-MNIST as PNG files in class folders (ImageFolder layout)
  train/<class>/*.png       60,000 images (6,000 per class), 28x28 grayscale (mode L, values 0-255)
  test/<class>/*.png        10,000 images (1,000 per class), same format
  labels.csv                path, class_name, label (0-9), split
rgb_samples/              two RGB photographs (china.jpg, flower.jpg, 640x427) for colour/channel/resize/crop/augmentation demos

Load with torchvision:
  from torchvision.datasets import ImageFolder
  ds = ImageFolder("image_data/fashion_mnist/train")   # classes are read from the folder names

Fashion-MNIST: Zalando Research, MIT licence (https://github.com/zalandoresearch/fashion-mnist).
Sample photos: bundled with scikit-learn (scikit-learn.org), originally from the scikit-learn sample-image set.
