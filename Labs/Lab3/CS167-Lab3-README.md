# Lab 3

## Student information

* Full name: Arun Chacko
* E-mail: achac021@ucr.edu
* UCR NetID: achac021
* Student ID: 862298328

## Answers

1. ***(Q1) Compare `bytesRead` and `length`, are they equal? Use one sentance to explain why.***

Input: 0 4
- Bytes Read = 7; Length = 4;
- No, bytesRead (7) and length (4) are not equal because the program starts reading from the specified offset but includes the entire line if the offset is not aligned with the start of a line, which results in reading more bytes than the specified length.
Input: 3 4
- Bytes Read = 4; Length = 0;
- No, the bytes read and the expected length are not equal because the program skips the partial line at the given offset (3) before starting to read the content, so no bytes are read in the specified length range.
Input: 3 9
- Bytes Read = 9; Length = 9;
- Yes, the actual bytes read and the split length are equal because the program correctly reads the file until the specified length (9 bytes), stopping when it has reached or exceeded that length.


2. ***(Q2) Copy the output of this command.***




3. ***(Q3) How many live datanodes are in this cluster?***



4. ***(Q4) How many replicas are stored on the namenode? How many replicas are stored in the datanodes?***



5. ***(Q5) How many replicas are stored on the datanode uploading the file? How many replicas are stored across other datanodes?***




6. ***(Q6) Compare your results of Q4 and Q5, give one sentence to explain the results you obtained.***



7. ***(Q7) Include the output of the three cases above in your README file.***


  | offset | length | bytesRead  | numMatchingLines |
  | ------ | ------ | ---------- | ---------------- |
  | 500    | 1000   |            |                  |
  | 12000  | 1000   |            |                  |
  | 100095 | 1000   |            |                  |
