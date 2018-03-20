# itday-18
Adaptive &amp; Self-Learning Street Lightning Control

Points:

- Smart City based solution for Street Lighting Control & Automation
- Specifically on IoT. Implements Machine Learning.
- Scalable solution with ESP costing less than 500. A single ESP can connect to 2048 lamps.
- No need to change existing infrastructure and internal coding. Lamps can be added online in a CLUSTER.
- Set up represents GOOGLE MAP+FIREBASE. 
- logged in as ADMIN. Live status
- Three phases: AUTO mode: controls via LDR; MASTER CONTROL: admin control lamps+auto mode; LEARNING: ML learns via API
- Weather API (live).
- LDR optimizes intensity

current:
- control & diagnose individual bulbs, automate street, see status of a locality
- automate via LDR (no human input, research 2016)
- collect area data like intensity + weather (ex: sensor data, send bugs, panic mode)

Why ML:
- LDR may not be optimal everytime (bird sitting on sensor on BRIGHT DAY, headlight towards sensor at NIGHT).
- parameter like time -> daytime; temp (season), cloud (cloud cover), visibility (primary);
- will learn from collective data; for now visibility is the O/P for learning
- can learn from nearby lights (in the cluster).
- Master control will help callibrating real output (not calculated) as HUMAN can judge better.

Tech: Linear Regression for intensity output, Naive Bayes for classification (ON/OFF, HIGH MED LOW).

