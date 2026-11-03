# special-octo-spork
Question 2:
Version 1:
When both requests arrive simultaneously, A always gets priority. B has to wait.
req_A   req_B   grant_A   grant_B    
  1       1       1         0         
  1       1       1         0
  1       1       1         0
  1       1       1         0

Version 2:
When both requests arrive simultaneously, pririty alternates between A and B.
req_A   req_B   grant_A   grant_B
  1       1       1         0
  1       1       0         1
  1       1       1         0
  1       1       0         1  
