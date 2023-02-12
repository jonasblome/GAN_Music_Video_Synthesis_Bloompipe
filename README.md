This is a copy of the synthesis module of our Bloompipe web application. The webapp can currently be found at bloompipe.de!

The module reads a .pkl file into the StyleGAN network and feeds an audio float stream into a vector generation algorithm.
This algorithm creates vector for each frame of the final video. Those vectors form a path through the latent space
that represents the movement of the audio material. Those vectors are then fed into the GAN which finally creates the frames.

Each frame is then stored on our server and all frames are compiled into a complete video with the underlying audio.
