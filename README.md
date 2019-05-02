# python-challenge
Python Assignment
#import resource file
import os
import csv

#Set path for file
csvpath = os.path.join('.', 'Resources', 'budget_data.csv')


#Set total_month variable = o
total_months = 0


# Open the CSV
with open(csvpath, newline="") as csvfile:
    csvreader = csv.reader(csvfile, delimiter=",")

def getbudgetdata(budgetdata):



#Use a loop to count total number of months included in the dataset
    for loop in csvreader:
        total_months = total_months + 1

    print(total_months)

#Sum net total amount of "Profit/Losses" over the entire period
    net_total = int(budgetdata[1])
    print(net_total)


#Get average of the changes in "Profit/Losses" over the entire period


#Find greatest increase (largest difference between two consecutive rows) 
# in profits (date and amount) over the entire period


#Find greatest decrease in losses (date and amount) over the entire period
