# nbamatchups
 
Required packages: tensorflow, jupyterlab, pandas

ANN to select which of two NBA players is better, based on selected data from basketballreference.com.
Trained using data from the 2020-2021 NBA season.

Methodology:
1. Import every player's per 100 possessions stats for the 2020-2021 season from basketballreference.com, while trimming derived statistics such as shooting percentages, which are already accounted for in shooting attempts and makes.
2. Manually label players as either good (1) or bad (0). I was as vague as possible when considering whether a player was "good", to avoid bias. For example I tried to include players that were considered good defensively but bad offensively, like Gobert and Covington, while also having the opposite such as Harden and Trae Young.
3. Create matchups by pairing good players with bad players, then randomize them so that the matchups aren't always good player on right, bad player on left.
4. Separate the data into test and training sets, and also separate the labels from the actual data.
5. Train the neural network with this data.

Note: This project is a work in progress. There are still many things I would like to do with this, such as incorporate Offensive and Defensive rating, test if the network can compare accross eras, etc.
