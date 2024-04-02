Assignment: Robot Task Optimization Using Genetic Algorithm Objective: The goal of this assignment is to develop and implement a Genetic Algorithm (GA) to optimize the assignment of multiple robots to a set of tasks in a dynamic production environment. Your primary objectives are to minimize the total production time, ensure a balanced workload across robots, and prioritize critical tasks effectively. Additionally, you will create a detailed visualization to illustrate the final task assignments, robot efficiencies, and task priorities.

Assignment Details --. Background: • You have a set of tasks, each with a specified duration and priority. • A pool of robots is available, each with a unique efficiency factor. • The production environment is dynamic, with tasks and priorities potentially changing over time.

some methods in this project: def generate_mock_data(num_tasks=10, num_robots=5): -- generate the background environment

def fitness_function(population, task_durations, task_priorities, robot_efficiencies): -- fitness function to select parent

def select_parents(population, fitness): -- how mating pool is created

def crossover(parents, num_offspring): -- how new generation is developed

def mutation(offspring, mutation_rate, robot_efficiencies): -- how each selected population is mutated

def run_genetic_algorithm(task_durations, task_priorities, robot_efficiencies): -- run from main function and contains all the calls for selection, mutation and crossover

def visualize_assignments_improved(solution, task_durations, task_priorities, robot_efficiencies): -- visualize the grid

run the main function and change some parameter to see different type of result.
