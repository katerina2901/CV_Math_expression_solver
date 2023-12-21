# CV_Math_expression_solver

Problem description

 The problem is to develop a system that can recognize and solve basic handwritten mathematical equations. This includes the ability to accurately identify and understand symbols such as numbers, and operators (addition, subtraction, multiplication, and division), as well as the arrangement and relationship between these elements. 
 The problem with handwritten equations is that they can be written in different styles, sizes, and orientations. Also, the handwriting of different individuals can vary significantly, making it difficult to recognize the symbols accurately. The expected value of CV  is the accurate recognition of handwritten letters and symbols, as well as the accurate analysis and solution of equations.

## Dataset description 

  The [dataset](https://www.kaggle.com/datasets/michelheusser/handwritten-digits-and-operators/data) contains digits [0-9] and operation characters: +, -, * , /, (, ).
Each character was isolated and fit in a 28x28 grayscale .png file. Each image was transformed using all possible combinations: rotation (-15°, -8°, 0°, 8°, 15°), stretching on each axis (1, 1.2, 1.3). Each transformed image was saved in .png format.
  What makes this dataset different from existing ones, is that it lays emphasis on the actual strokes of handwritten signs, instead of just being a compilation of scanned images of existing records (the way, for example, the MNIST dataset was created). Each pixel is strictly full black, or full white (no greytones), and the strokes are rather thin.
CompleteDataSet - List of tuples with all datapoints. (ca. 300'000 Datapoints)
Training dataset (60% of CompleteDataSet.npy)
Validation dataset (20% of CompleteDataSet.npy)
Testing dataset (20% of CompleteDataSet.npy)


## Pipline

  1. Data analysis and preprocessing
  2. CNN model selection and training for multiclass classification
  3. OCR models selection
  4. Crop and classification
  5. Solver and analysis of the result ([Current solution also for comparing]
(https://webdemo.myscript.com/views/math/index.html))

## Project Organization
  ├── project-cv.ipynb        <- Jupyter notebooks. (Train models & EasyOCR & PyTesseract)
   ├── README.md               <- The top-level README
   ├── resnet.ipynb            <- upyter notebooks. (Train model ResNet & CV2 find conturs)
   ├── lenet.pth               <- weights for LeNet18
   │
   ├── mobilenet.pth           <- weights for MobileNet
   │
   ├── resnet.pth              <- weights for ResNet (for resnet.ipynb, for [project-cv.ipynb](https://drive.google.com/file/d/19KQOwUfYnX3LJafsa-oT_E3hqA9s0HHP/view?usp=sharing))
   │
   ├── test.zip                <- Jupyter notebooks. (Visualization & metrics)
   |
   ├── CV_project.pdf          <- Jupyter notebooks. (Visualization & metrics)


