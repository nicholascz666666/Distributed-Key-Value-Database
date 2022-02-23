# Distributed Key-Value Database

## Approach

We tried our best to adhere to the Raft paper when implementing our replicas. 

## Challenges

- We had issues with getting follower replicas to log information correctly following an AppendEntry message
- Following a leader crash, we had difficulty getting the election process to restart
- We faced a lot of issues with quorums and getting all replicas to respond in a timely manner

## Testing

We tested our code by running `sim.py` on each test case individually 3 times and running `sim.py all` 3 times as well. Most of our testing was done with the simulator given; we did not feel the need to write our own additional tests for this project.
