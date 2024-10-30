# Song-Lyrics-Generation-Using-Recurrent-Neural-Networks
## Authors
- **Keren Gorelik**
- **Lior Kobi**

## Project Overview
This project focuses on generating song lyrics that align with given melodies using a Recurrent Neural Network (RNN) architecture. The goal is to combine musical and lyrical data to create lyrics that not only follow melodic flow but also enhance the emotional impact of the music.

## Methodology
1. **Dataset**: We utilized a dataset of song lyrics and MIDI files, containing both text and musical information.
2. **Data Preprocessing**:
   - Lyrics were cleaned, tokenized, and converted into numerical indices to build a vocabulary.
   - MIDI files were analyzed to extract notes, beats, and harmonic features.
3. **Embedding**:
   - **Word Embedding**: Using Word2Vec, each word was represented in a multidimensional space, capturing semantic meaning.
   - **Musical Embedding**: Musical notes and features were encoded to combine with the lyrics in the RNN.

4. **Model Architecture**:
   - The RNN was constructed using Long Short-Term Memory (LSTM) units and Gated Recurrent Units (GRU) to handle sequential dependencies in lyrics.
   - The model was trained on a combination of lyrics and melodic data, aiming to produce coherent and relevant lyrics in response to given musical cues.

5. **Output Generation**:
   - Different word initialization strategies were tested to control the flow and coherence of the generated lyrics.
   - Generated lyrics were evaluated based on their alignment with the given melody and thematic relevance.

## Results
- The model generated lyrics that demonstrated coherent structure and thematic alignment with the melodies, showcasing potential for AI-driven creativity in music generation.
- Evaluations indicated successful integration of musical and lyrical data, with generated lyrics displaying strong relevance to provided melodies.

## Dependencies
- Python 3.x
- PyTorch
- NumPy
- Word2Vec for embeddings

## How to Run
1. Clone the repository.
2. Install required packages:
   ```bash
   pip install torch numpy gensim
   ```
3. Run the training script:
   ```bash
   python main.py
   ```
4. Results and generated lyrics will be saved to the output directory.
