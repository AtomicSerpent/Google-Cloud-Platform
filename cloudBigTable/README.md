### CLoud Big Table

1. Enable API

2. Install and Configure **cbt**

> gcloud components update
> gcloud components install cbt

3. Configure cbt:

   > echo project=<PROJECT_ID> > ~/.cbtrc
   > echo instance=<emample-data-cbt> >> ~/.cbtrc

4. Create Data Table:

   > cbt createtable example-table

5. Verify:

   > cbt ls

6. Create the first column family (a group of columns):

   > cbt createfamily example-table exampleset

7. Create the column qualifier (the column within the column family) and put some data in the first cell:

   > cbt set example-table r1 exampleset:c1=airplanes

8. Review the results so far:

   > cbt read example-table

9. Add a second column qualifier:

   > cbt set example-table r1 exampleset:c2=pilots

10. Review the result:
    > cbt read example-table
