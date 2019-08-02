# RA_lenovo
Psychtoolbox task scripts used to run the VA_RA_PTB study (PTSD veteran decision making under risk and ambiguity, gains and losses)

To run the study:
  - Run practice: type in the command RA()
  - Run task: type in the command RA(subject ID)


### Brief description: 
Examine risk and ambiguity attitudes in the monetary gain and loss domains (imaging).

### Software:
Practice in e-prime; scan in Matlab Psychtoolbox

### Trial types: Each choice is between $±5 for sure and a risky or ambiguous lottery. 
  - 3 risk levels: 0.25, 0.5, 0.75
  - 3 ambiguity levels: 0.24, 0.5, 0.74
  - 20 amount levels: ±$5, 6, 7, 8, 10, 12, 14, 16, 19, 23, 27, 31, 37, 44, 52, 61, 73, 86, 101, and 120
  - Each combination of risk/ambiguity and amount appears once.
  - Gain and loss trials are in separate blocks.
  - 8 blocks, 31 trials per block.
  - 2 orders (gains first or losses first): 2 gains - 2 losses - 2 losses - 2 gains, or 2 losses – 2 gains – 2 gains – 2 losses
  - 2 sessions on separate days 

### Randomization: 
Trials are created in the Gain1 and Loss1 scripts (basically the first time you run the subject on this corresponding domain). After creating all trials, the order within each gain/loss domain is permuted, and assigned to 4 blocks, so that each block has 30 trials. Also, we add one other trials at the beginning of each block, which make the total trials per block 31. This trial is always ±$5 vs. a lottery giving ±$4, and will be excluded from analysis. Adding this trial is because the signal is not stable at the beginning when scanner start running. 

### Trial structure: 	
  - options are presented on left and right of screen, 6000ms.
  - response cue, and response (< 3500ms) 
  - feedback image (500ms)
  - fixation (jittered 4000, 6000, 8000 ms + (3500ms-response time))

### Response:
Press one of two buttons.

### Payoff:
Real. Subject gets $120 endowment. At the end of the experiment, one trial is randomly selected by rolling a die. Real bags are used as lotteries.  
