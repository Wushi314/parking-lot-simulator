There are three jupyter notebooks in this repo. 
gridlot_gif_generator is responsible for creating the gifs. The gifs allow us to see how the parking schedule looks for each method.
night_runner is the notebook for analyzing how the simulation scales. This is where the .csv and the data comes from. It was designed to run overnight because the IP takes a long time to solve.

Both notebooks have a lot of duplicate code. They were split up for cleanliness purposes. Each follows a similar process at the beginning. They also have the same function definitions for the most part.
First the graph representation of the parking lot is made.
Then the cars are made along with their assigned paths and parking spots.
Then the IP solver is set up.
Then the IP is solved and data is collected or a gif is generated.

There is an old iteration folder. This contains an older version of the project that does not have parking blocking and the queue-like waiting, which made it very arbitary. I kept it as an artifact to show the importance of the realistic solution, even though it blows up the run time. Much of the same code structure is used.