# grid-universe

## Summary
Developed a Grid Universe AI agent combining heuristic search, CNN image recognition, and SVM objective classification. Gained experience with NumPy, pandas, scikit-learn, and PyTorch through data preprocessing, model training, evaluation, and heuristic tuning.

## About
I developed an AI agent for Grid Universe, a grid-based environment that combines navigation, item collection, portals, hazards, enemies, and power-ups. The project required the agent to interpret visual observations, identify objectives that could be provided as ciphertext, and select actions that balance task completion with movement costs and rewards.

My implementation combined classical search with machine learning. I built an A*-style planner using a priority queue and custom heuristics that considered distances to exits and required items, portal shortcuts, collectible rewards, and available power-ups. I also implemented randomized heuristic-weight tuning to explore configurations based on execution time and failure penalties. This helped me understand the practical trade-offs between search efficiency, solution quality, and computational constraints.

For visual perception, I developed a convolutional neural network using PyTorch to classify image tiles and reconstruct a structured representation of the environment. I used NumPy and Pillow for image manipulation, alongside torchvision for resizing, normalization, and data augmentation. Building the training workflow introduced me to convolutional layers, activation functions, pooling, loss functions, backpropagation, and the Adam optimizer. I also explored an alternative image-classification approach using principal component analysis and support vector machines.

To interpret encrypted objectives, I trained a support vector machine using scikit-learn, with pandas supporting data preparation and feature processing. This provided experience with categorical encoding, feature scaling, train-test splits, and classification evaluation.

Overall, the project strengthened my ability to integrate perception, objective interpretation, and planning into a single agent. It also taught me to distinguish implementing an algorithm from demonstrating its reliability: evaluation must consider unseen inputs, runtime limits, and failure cases rather than success on familiar examples alone. Through experimentation and debugging, I gained practical experience with Python’s scientific computing and machine-learning ecosystem and learned how representations and heuristic choices influence an intelligent system’s behaviour across different tasks and operating conditions.
