<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
 
</head>
<body>
    <h1 style="text-align: center;">MsPacman RL Agent</h1>
    <p>This repository contains a Reinforcement Learning (RL) agent implemented in PyTorch to solve the MsPacmanDeterministic-v0 environment from the OpenAI Gym. The agent utilizes a Deep Q-Network (DQN) to learn how to control Ms. Pac-Man and maximize its score.</p>
    <h2>Overview</h2>
    <p>The MsPacmanDeterministic-v0 environment simulates the classic arcade game Ms. Pac-Man. The agent controls Ms. Pac-Man to navigate through a maze, eat pellets, and avoid ghosts. The goal is to learn a policy that maximizes the cumulative score while avoiding ghosts.</p>
    <h2>Key Concepts and Components</h2>
    <ul>
        <li><strong>Deep Q-Network (DQN):</strong> The agent's neural network architecture is implemented using PyTorch. It consists of convolutional layers followed by fully connected layers with ReLU activation functions.</li>
        <li><strong>Replay Memory:</strong> Experience replay is utilized to store and sample past experiences for efficient training. It helps stabilize and improve the learning process by breaking correlations between consecutive samples.</li>
        <li><strong>Target Network:</strong> A target Q-network is used to stabilize training by providing more stable target values during the learning process. Periodically, the parameters of the target network are updated to match those of the primary network.</li>
        <li><strong>Epsilon-Greedy Exploration:</strong> The agent balances exploration and exploitation using an epsilon-greedy policy. It selects random actions with probability epsilon and greedy actions based on the learned Q-values otherwise.</li>
        <li><strong>Training Loop:</strong> The agent interacts with the environment, collects experiences, and updates its Q-network parameters using mini-batch gradient descent.</li>
    </ul>
    <h2>Metrics</h2>
    <ul>
        <li><strong>Average Score per Episode:</strong> The training process prints the average score achieved by the agent over the last 100 episodes. This metric indicates the agent's learning progress and performance.</li>
        <li><strong>Environment Solving:</strong> The environment is considered solved when the average score over the last 100 episodes exceeds 150. Upon solving, the training process stops, and the model parameters are saved.</li>
    </ul>
    <h2>Installation and Usage</h2>
    <p>To run the RL agent and train it to solve the MsPacmanDeterministic-v0 environment, follow these steps:</p>
    <ol>
        <li>Clone this repository to your local machine.</li>
        <li>Install the required dependencies by executing the following command:</li>
    </ol>
    <pre><code>pip install gym gym[atari,accept-rom-license] box2d torch</code></pre>
    <p>Ensure you have the necessary dependencies installed, including Gym and PyTorch, to execute the code successfully.</p>
    <h2>Getting Started</h2>
    <p>To begin training the RL agent, execute the provided code in your preferred Python environment. Adjust hyperparameters and training settings as needed for your specific requirements.</p>
    <h2>License</h2>
    <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>
</body>
</html>
