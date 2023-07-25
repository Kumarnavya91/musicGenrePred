# musicGenrePred
Music Genre predictor using knn
The dataset used here is the GTZAN dataset which contains 1000 audio files that belong to 10 different classes.
Each audio file is in wav format.The classes to which audio files belong are Blues, Hip-hop, classical, pop, Disco, Country, Metal, Jazz, Reggae, and Rock.
It can be downloaded from Kaggle
MFCC provides 32 features 
Feature extraction is a process to extract important features from data. It includes identifying linguistic data and avoiding any kind of noise. Audio features are classified into 3 categories high-level, mid-level, and low-level audio features.

High-level features are related to music lyrics like chords, rhythm, melody, etc.
Mid-level features include beat level attributes, pitch-like fluctuation patterns, and MFCCs.
Low-level features include energy, a zero-crossing rate which are statistical measures that get extracted from audio during feature extraction.
So to generate these features we use a certain set of steps and are combined under a single name as MFCC that helps extract mid-level and low-level audio features. below are the steps discussed for the working of MFCCs in feature extraction.

Audio files are of a certain length(duration) in seconds or as long as in minutes. And the pitch or frequency is continuously changing so to understand this we first divide the audio file into small-small frames which are near about 20 to 40 ms long.
After dividing into frames we try to identify and extract different frequencies from each frame. When we divide in such a small frame so assume that one frame divides down in a single frequency.
separate linguistic frequencies from the noise
To discard any type of noise, take discrete cosine transform (DCT) of the frequencies.


