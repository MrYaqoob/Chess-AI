# Chess-AI
The goal of this project is to develop a powerful chess AI capable of defeating today's grandmasters. The AI has been trained using real-world chess data sourced from Lichess. Specifically, the dataset used for training was downloaded from lichess.org and consists of games played in November and December 2013.

To facilitate development and experimentation, a dataset will be provided for reference.


### Disclaimer: This project was created as a university assignment and is intended for educational purposes only. If you wish to use this in your own project, please notify the creator (MrYaqoob).


### Key Features & Methodology:
- Hybrid AI Approach: The AI utilizes a combination of heuristic search (alpha-beta pruning) and machine learning models (Random Forest and Gradient Boosting) to predict optimal moves.
- Feature Extraction: The system leverages piece-square tables and other board state evaluation techniques to enhance decision-making.
- Move Prediction & Evaluation: The AI evaluates positions using a heuristic-based evaluation function and a trained model for improved accuracy.
- PGN Data Parsing & Balancing: The dataset is preprocessed, including PGN parsing, feature extraction, oversampling, and balancing to improve training quality.
- Game Modes: Supports both AI vs AI and Human vs AI gameplay, providing an interactive experience for players.
- Fivefold Repetition Handling: The engine correctly detects and addresses fivefold repetition to comply with chess rules.

The ultimate objective is to refine the AI to compete at the highest levels of chess mastery.

### Challenges & Issues:
- Dataset Limitations: The training data is from 2013, meaning it lacks more recent trends, strategies, and refinements in modern grandmaster play. I would suggest you get the latest dataset from Lichess and perform the execution.
- Computational Complexity: The combination of heuristic search and machine learning can be computationally expensive, leading to longer move calculation times.
- Model Generalization: The AI may struggle against novel playstyles or unconventional openings not well-represented in the dataset.
- Overfitting on Historical Data: Since the AI is trained on a specific dataset, there is a risk of overfitting to past games rather than adapting Dynamically to new strategies.
- Endgame Handling: While the AI performs well in the opening and middlegame, improvements are needed for endgame precision, especially in complex endgames without clear heuristics.
- Parameter Tuning: Finding the right balance between heuristic-based search (alpha-beta pruning) and ML-based move prediction requires fine-tuning and optimization.
- Dataset Loading Issue: While loading the dataset, a limitation was set to include only 8,000 games, but this restriction is not being strictly followed. This needs to be optimized to ensure the dataset size remains within the intended limit.
