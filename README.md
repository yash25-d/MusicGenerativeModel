# MusicGenerativeModel
This Repository contains the LSTM based Music Generation models.
The model result as audio output is stored in the midi audio files.

TO PROCESS THE AUDIO FILES, A DATASET OF FOLK TRADITIONAL SONGS OF EUROPE HAVE BEEN CONSIDERED.
THE DATASET HAS .KRN FILES AND MUSESCORE IS DEPLOYED TO STUDY THE VARIOUS PATTERNS OF AUDIO QUALITIES IF THE TEST DATASET.
THE SYMBOLIC REPRESENTATION OF TUNES IS AN ESSENTIAL PART OF UNDERSTANDING HOW THE QUALITIES OF MUSIC LIKE:
PITCH
DURATION
KEY

FLAT PITCH
REST INTERVALS,etc.

THE FIRST STEP IN THE EVALUATION OF THE MODEL IS PREPROCESSING AND CLEANING OF THE PROVIDED DATASET.
NOTE: CONSIDERING THE COMPLEXITY OF MODEL, THE KEYS HAVE BEEN SCALED TO A LESSER NUMBER OF CHORDS DURING THE INITIAL PROCESS OF ANALYSING THE DATA.

FOR THE PREPROCESSING THE MUSIC PRODUCED HAS BEEN STANDARDISED AND TRANSPOSED TO PROVIDE A UNIFORM DISTRIBUTION FOR THE MODEL INPUT.

THE SECOND STEP IN PREPROCESSING THE DATA INCLUDES MAPPING THE UNIQUE KEY VALUE PAIRS IN AUDIO AND USING 
ENCODING TO TRANSFORM THE AUDIO PATTERN DATASET TO BE FED TO THE GENERATIVE DL MODEL.
TO DO SO, A MAPPING OF THE VOCABULARY IS USED WITH ENCODING VALUE PAIRS AND THE ENTIRE DATASET IS THEN USED TO 
MAP THE KEY PATTERNS TO NUMERICAL VECTORS.


THE NEXT STEP USES THE SELECTION OF DL MODEL TO USE TIMES SERIES FORECASTING AND TO RETAIN THE PAST OCCURENCES OF PITCH, DURATION IN THE MUSIC.
TO ACHEIVE THIS A RNN(RECURRENT NEURAL NETWORK) AND LSTM(LONG SHORT TERM MEMORY) UNITS HAVE BEEN DEPLOYED TO STUDY THE
SIMILARITIES AND REPETETIVE FEATURES OF THE GIVEN VECTOR ENCODINGS.


THE THIRD STEP IN BUILDING THE PROJECT INCLUDES FINE TUNING THE MODEL FOR ACHIEVING A BETTER ACCURACY.

A CROSS ENTROPY LOSS FUNCTION IS USED TO DETERMINE THE DEVIATION OF ACTUAL MODEL WITH THE TUNES GENERATED.
FOR FINE TUNING, A NUMBER OF HYPERPARAMETERS LIKE INPUT AND OUTPUT SHAPE OF PARAMETERS HAVE BEEN STUDIED.

THE FINAL ACCURACY OF THE MODEL ACHIEVED IS 96.24% AFTER SPECIFIED EPOCHS.


THE MOST IMPORTANT STEP OF BUILDING THE MODEL IS TO PROVIDE A SAMPLE OUTPUT AND THEN DECODE THE OUTPUT VECTOR
THEN THE OUTPUT VECTOR HAS TO BE CHANGED ANDTRANSFORMED TO ANY AUDIO SPECIFIED PROTOCOL FILE.

FOR THIS PROJECT THE OUTPUT AUDIO FILE IS OF A .MIDI FORMAT.
FOR THE AUDIO OUTPUT FILES, THE SEED SONGS AND GENERATED SONGS HAVE BEEN STORED IN A DRIVE LINK FOR USERS TO ACCESS THE RESULT.

