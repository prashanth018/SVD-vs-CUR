# SVD-vs-CUR

## Design Documentation
### List of Packages Used
- csv
- copy
- mathnumpy 
- pandas 
- random 
- mpl_toolkits.mplot3d 
- matplotlib.pyplot 
- time

### List of Functions Used
- svd 
- pythag 
- randrange 
- dataToMatrix
- frob 
- cur

### Data-Structures used
- Arrays
- Lists
- Dictionaries
- tuples
- DataFrame imported from Pandas

## Functions
### svd (in SVD.py) - 
	Takes a list as an input 
	returns the original matrix by performing u * diagnolized(s) * transpose(v)

### svd (in SVD_VS_CUR.py) -
	Takes a list as an input 
	returns a 2d list(u) and a 1d list(eigen values) and 2d list(v)

### pythag
	It is a utility function for svd
	It avoids overflow or underflow in qr Decomposition

### randrange 
	Utility function to debug the code

### dataToMatrix -
	Takes a list as input
	and returns a matrix 
	it converts the user-item data from the file into a matrix

### frob
	Takes 2 matrices as input
	Returns a floating point value which is the frobenious error

### cur
	Takes a matrix as an input
	Selects m and n values randomly 
	Then selects top m rows and n columns with highest probabilities respectively
	Then computes row and col and u
	and then computes the original matrix by performing col * u * row
