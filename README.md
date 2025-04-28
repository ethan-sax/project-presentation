
# Playing Atari Pong with Deep Reinforcement Learning
This project is based off the paper "Playing Atari with Deep Reinforcement Learning", written by various co-authors at DeepMind Technologies. Focusing exclusivley on the Pong environment, we implemented code to test the effectiveness and efficiency of the algorithm, utilizing the core ideas of the Deep Q-Network (DQN).

## Project Structure
The code is provided as a Jupyter Notebook (.ipynb file).

The agent is trained to learn optimal policies via experience replay and deep Q-learning.

## Requirements
 - Python 3.11

 - GPU access isn't necessarily required, but it is highly recommended for training (e.g., Google Colab, or a CUDA-compatible local setup). Running it on a CPU will be extremely slow.

 - Main packages:

    - ```gymnasium[atari, accept-rom-license]```

    - ```torch```

    - ```torchvision```

    - ```numpy```

    - ```ale-py```

    - ```opencv-python (for cv2)```

    - ```matplotlib```

You can install the main dependencies with:

 
  ```bash 
pip install gymnasium[atari,accept-rom-license] torch torchvision numpy ale-py opencv-python matplotlib
  ``` 


## Running the Project
1. Download the DataMiningProject.ipynb file
2. Open [Google Colab](https://colab.research.google.com/)
3. Upload the downloaded notebook
4. [Recommended] Change runtime to GPU (runtime -> change runtime type -> hardware accelerator -> GPU)
5. Run cells to define classes for model training: Pre-processing, Model Network, Replay Memory Class, Model Evaluation, Frame Skipper
6. Run cells to define and train model
7. Run remaining cells to produce model evaluation metrics, training curve plots, and the average episode reward plot.

## Notes
Training an agent from scratch can take several hours even on a GPU. It will depend on the GPU implemented.

## Results
The agent will successfully learns to play Pong competitively against the built-in AI opponent.

## Acknowledgments
Based on [Playing Atari with Deep Reinforcement Learning](https://arxiv.org/pdf/1312.5602).
