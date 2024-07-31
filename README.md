# Mario Level Evolution Project

## Introduction
In this project, we implemented a genetic algorithm to evolve interesting and playable Super Mario Bros. levels. The goal was to explore two different encodings of Mario levels, tweak fitness functions and evolutionary operators, and ultimately find levels that are both fun and challenging.

## Changes Made

### Genetic Algorithm Implementation
1. **Selection Strategy**: Implemented elitist selection and roulette wheel selection in the `generate_successors` function.
2. **Crossover Operator**: Implemented single-point crossover in the `generate_children` function for both `Individual_Grid` and `Individual_DE` encodings.
3. **Mutation Operator**: Implemented a mutation operator in the `mutate` function to introduce random changes in the genomes.
4. **Fitness Function**: Optimized the `calculate_fitness` function to include a combination of metrics such as meaningful jump variance, negative space, path percentage, empty percentage, linearity, and solvability.

### Code Adjustments
- Ensured the `levels` directory is created if it does not exist.
- Added checks for empty genomes to prevent errors during crossover.
- Utilized multiprocessing to parallelize fitness calculations for improved performance.

## Favorite Level

### Level Selection Criteria
1. **Playability**: The level must be beatable and provide a fair challenge.
2. **Visual Appeal**: The level should have an aesthetically pleasing layout.
3. **Fun Factor**: The level should be enjoyable to play and offer interesting gameplay.
4. **Variety**: The level should include diverse elements, such as different types of blocks, enemies, and obstacles.
5. **Creativity**: The level should stand out due to unique design elements or clever use of game mechanics.

### Chosen Level
After evaluating the generated levels, my favorite level is `<level_filename>`. This level was chosen based on the following reasons:
- **Playability**: The level is beatable with a balanced difficulty curve.
- **Visual Appeal**: The layout is visually appealing with a good mix of elements.
- **Fun Factor**: The level offers an engaging and enjoyable experience with well-placed challenges.
- **Variety**: The level includes a variety of elements such as question mark blocks, enemies, and different types of platforms.
- **Creativity**: The design of the level is unique, with creative use of obstacles and power-ups.

### Generation Details
- **Generations**: The level was generated after running the genetic algorithm for `<number_of_generations>` generations.
- **Net Time**: The total time taken to generate this level was approximately `<total_time>` seconds.
