## The task

Participants had to design the most profitable heat network for a given area. The area is a graph: a producer with a maximum capacity, buildings that can be connected, and street intersections. Each potential pipe has a construction cost proportional to its length, and each connected building brings revenue proportional to its demand. The question is which subset of pipes and customers to keep.

## Why it is hard

Heat networks are one of the main levers to decarbonize cities, but they need large upfront investments, so their layout has to make economic sense. On a small neighborhood, the problem can be solved exactly as a mixed-integer linear program. At the scale of a metropolis, with thousands of nodes and tens of thousands of possible pipes, the solver takes far too long, while planners need scenarios in a few minutes.

Teams had less than 2 minutes per instance to get as close as possible to the optimum. They could use heuristics, graph reduction, machine learning to pre-select promising customers or pipes, or relaxed versions of the problem to guide the search. The winner was the team with the highest total profit over all test instances.
