Frequent Itemset Mining
Apriori and FP-tree
This project is an assignemnt of the Data Mining Course(COL761) at IIT Delhi.

Apriori Algorithm and FP-tree are used to mine frequent itemsets on this dataset: http://fimi.ua.ac.be/data/retail.dat Details about the dataset can be found at http://fimi.ua.ac.be/data/retail.pdf It is assumed that all items are integers.

Executing the command: sh .sh X -apriori generates a file .txt containing the frequent itemsets at>=X% support threshold with the Apriori algorithm. Similarly, executing the command:sh RollNo.sh X -fptree generates a file.txt containing the frequent itemsets using FP-tree algorithm. Notice that X is in percentage and not the absolute count. Our implementations ensure that the transactions are not loaded into main memory. However, the frequent patterns and candidate sets are stored in memory.

.txt follows the following format: 1. Each frequent itemset is on a new line. 2. The items in each itemset are space separated.

The performance of Apriori algorithm is compared with FP-tree in the report.

Executing the command: sh .sh -plot generates a plot using matplotlib where the x-axis varies the support threshold and y-axis shows the corresponding running times. It plots the running times at support thresholds of 1%, 5%, 10%, 25%, 50%, and 90%. The results obtained are explained in the report.
