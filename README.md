Image to Painting Effect

This project applies a realistic painting effect to an image using OpenCV and NumPy. The script smooths colors, enhances edges, and blends effects to produce an artistic transformation of the input image.

📌 Features

Bilateral Filtering: Smooths colors while preserving edges.

Adaptive Edge Enhancement: Highlights key details without over-sharpening.

Oil Painting Effect: Simulates brush strokes for an artistic touch.

Edge Blending: Merges edges with painting effect to maintain structure.

📂 Requirements

Ensure you have Python installed along with the required libraries:

pip install opencv-python numpy pillow

🚀 Usage

Place an image in the project folder.

Run the following command in Python:

image_to_painting("your_image.jpg")

The processed painting will be displayed and saved as realistic_painting.jpg.

🖼️ How It Works

Reads the input image.

Applies bilateral filtering to smooth colors while retaining edges.

Converts the image to grayscale and enhances edges using adaptive thresholding.

Applies oil painting stylization to create a painting-like effect.

Blends the enhanced edges with the painting effect for a realistic look.

Saves the final painting as realistic_painting.jpg.

📌 Output

The processed image will be saved in the same directory as realistic_painting.jpg.
Example output:
Input: 
![your_image](https://github.com/user-attachments/assets/5796d194-fcdd-43c3-8109-5aaa47053bf6)
Output: 
![realistic_painting](https://github.com/user-attachments/assets/f606b4d1-42f6-4b7c-8708-a5020af1ea56)


🔧 Customization

You can tweak the parameters in the cv2.stylization() function:

cv2.stylization(smooth_img, sigma_s=150, sigma_r=0.3)

sigma_s: Controls brushstroke size (Higher = stronger effect).

sigma_r: Controls edge sharpness (Lower = more detail).

📜 License

This project is free to use for educational and personal projects.

Enjoy creating artistic transformations! 🎨✨
