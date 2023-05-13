<h1 align="center">Bird Call Classification</h1>

<h4 align='center'> This project identifies and classify the birds in a mixed cacophony by using a model trained on various audio recordings of individual bird voices using neural networks (CNN's) and various pre-processing techniques is used to reduce noise from the audio files.
</h4>

## File Structure

```
.
├── dataset                             -> Contains Dataset of the birds 
|   ├── crow 
|   ├── cuckoo
|   ├── sparrow
|   ├── test
|   ├── train.csv
|   ├── valid.csv
├── BE_Proj.ipynb                       -> Code file
```

## Block Diagram
![Blank diagram](https://github.com/priyanshmehta986/Bird_Call_Classification/assets/69569703/c3068871-4a7c-4ab9-87f6-f9a4df855c0f)

## Architecture 
![Architecture](https://github.com/priyanshmehta986/Bird_Call_Classification/assets/69569703/4faae8a1-0550-493c-996a-a8954247f5dc)



## Modules Implemented

- Data Collection and Preprocessing: The bird audio dataset is collected from Xeno Canto using its open API for 3 birds namely Sparrow, Crow, and Cuckoo. The collected audio files undergo preprocessing steps to clean and prepare the audio files for analysis, which include:
	- Noise Removal: A Butterworth filter is used as a band-pass filter to remove or attenuate specific frequencies from the audio signals while preserving the frequencies of interest (bird vocalizations).
	- Dominant Audio Clip Identification: The audio files are analyzed to identify the dominant bird audio clips within each file using techniques such as Short-time Fourier transform (STFT), Calculation of Spectral centroid and Bandwidth, Calculation of Mean Spectral Centroid and Bandwidth, Signal-to-Noise Ratio (SNR) Calculation, Time-Varying Power Spectral Density (PSD) Calculation, Power Spectral Density Ratio (PSDR) Calculation, and Extraction of Dominant Bird Sound Clip.
- CNN Model Architecture: The CNN model architecture is designed to classify the bird sound clips into three categories.
- Model Training: The CNN model is trained using the preprocessed bird sound clips.
- Model Evaluation: The CNN model's performance is evaluated on the test set, and the results are reported.
  
## Contributors

- Prem Shah ([GitHub](https://github.com/prem1019))
- Priyansh Mehta ([GitHub](https://github.com/priyanshmehta986))
- Rishi Lakhani ([GitHub](https://github.com/RishiLakhani))


