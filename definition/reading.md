# Reading CSV Files

The reader function is formed to take each line of the file and make the list of all columns. Then, you choose the column you want a variable data for.
The CSV file is opened as the text file with Python’s built-in open() function, which returns the file object. This is then passed to the reader, which does the heavy lifting.
In python, we use csv.reader() module to read the csv file. Below is an example of how the csv file is read: 

#### Normal CSV file
We have a csv file called people.csv having default delimiter comma(,) with following data:

SN, Name, City
1, John, Washington
2, Eric, Los Angeles
3, Brad, Texas
Example 1: Read people.csv file, where delimiter is comma (,)
import csv
with open('people.csv', 'r') as csvFile:
    reader = csv.reader(csvFile)
    for row in reader:
        print(row)
csvFile.close()
When we run the above program, the output will be

['SN', ' Name', ' City']
['1', ' John', ' Washington']
['2', ' Eric', ' Los Angeles']
['3', ' Brad', ' Texas']