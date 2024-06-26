## Image-Noise-Removal-with-Fourier-Transform

This project demonstrates the application of Fourier Transform techniques for image denoising using Python and the scipy.fftpack library. Fourier Transform is utilized to analyze the frequency components of an image in the frequency domain, allowing for the identification and suppression of noise.

Original Image:

![image](https://github.com/YashaswiniSampath/Image-Noise-Removal-with-Fourier-Transform/assets/44898518/846c8c35-caa5-4c22-849f-8678d1ab6de0)

* Preprocessing: The input image is converted to grayscale to simplify processing.
* Fourier Transform: The Fourier spectrum of the grayscale image is visualized to pinpoint noise frequencies causing distortions.
* Noise Localization: Using Fourier analysis, noisy areas are identified and manually patched to restore the original image integrity.
* <img width="202" alt="Screenshot 2024-06-27 at 1 32 12 AM" src="https://github.com/YashaswiniSampath/Image-Noise-Removal-with-Fourier-Transform/assets/44898518/98d35a81-f18e-460e-b0f3-2200bf3bd642">


Image after denoising:\
![image](https://github.com/YashaswiniSampath/Image-Noise-Removal-with-Fourier-Transform/assets/44898518/f90e372d-60db-4c04-9835-c536444c336a)


Code Explanation: This Python script demonstrates how to apply Fourier Transform techniques for image processing and denoising. It begins by loading an input image and converting it to grayscale. Using the scipy.fftpack library, the script computes the Fourier Transform of the image, shifting the frequency components to the center for clarity. The resulting Fourier spectrum is then saved as an image (fft.png) after logarithmic scaling for better visualization. To illustrate a modification in the frequency domain, a small increment is added to a specific frequency component of the Fourier-transformed image. The script then performs an Inverse Fourier Transform to revert the modified frequency space back to an image format, which is subsequently saved as fft-then-ifft.png. 

