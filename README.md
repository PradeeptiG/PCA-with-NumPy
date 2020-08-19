# PCA-with-NumPy
The dimensionality of the Iris dataset was reduced using Principal Component Analysis.

Principal Component Analysis (PCA)
This technique reduces the dimensionality of the data.
It gives different directions (principal components) that maximize the variance of the data.
It tries to give linearly unrelated orthogonal axis.
PCA is important because it allows us to visualize our data before choosing and implementing a machine learning algorithm.
Another technique that can be used to achieve the same goal is Linear Discriminant Analysis.

Libraries Imported
Pandas- Used to import, clean, and analyse datasets.
NumPy- Used to perform operations on matrices.
Matplotlib- Used to create plots.
Seaborn- Used to visualize statistical data. It is based on matplotlib.

The Project
We used the Iris dataset. It contains 5 columns- sepal length, sepal width, petal length, petal width and iris species. There are 3 iris species- setosa, versicolor and virginica. There are 150 entries.
Exploratory Data Analysis (EDA)- Initial investigation on data. So that would include seeing the first five or last five entries using head() or tail(),  getting to know the number of rows and columns, checking the data type of  every column, getting the column names, knowing whether entries have missing values using info() and so on.
So each flower is described by 4 features. We will reduce the dimensionality ie we will reduce the number of features required to describe each flower.
In order to understand the data, we visualised it data using a scatterplot using seaborn.
Data standardization is extremely important in PCA. Here, from each feature, we subtract the mean and divide it by standard deviation. This is done so that each feature is given equal importance and PCA (which essentially projects our data into directions that maximize the variance along the axes) makes no errors.
Singular Value Decomposition (SVD) is a way to implement PCA.
Another way is through Eigen Decomposition. First create Co-variance matrix, then decompose it into Eigen vectors and Eigen values. Eigen vectors are the axes and Eigen values are the magnitude to be given to those axes. 
Plot the cumulative explained variance (cumulative of Eigen Values) against the number of principal components. Select those principal components which together describe about 95 percent of the data. Drop the remaining components thereby reducing the dimensionality. 
