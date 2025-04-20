# khalliha_3ala_el_lah
🌿 Olive Patch Classification  
This project uses deep learning to classify drone or satellite images of large olive tree patches into different olive types (e.g., Chemlali, Sbeitli, etc.). It leverages convolutional neural networks (CNNs) using TensorFlow and Keras.

## 📁 Project Structure
```
olive-classifier/
├── dataset/              # Folder where you place olive patch images (not on GitHub)
├── src/
│   └── train.py          # Main training script
├── sample_dataset/       # (Optional) Contains a few dummy images
├── olive_model.h5        # Saved model (optional)
├── requirements.txt      # Dependencies
├── README.md             # Project description and instructions
└── .gitignore
```

## 🧠 Objective
The goal is to automatically identify the type of olive patch from aerial images. This can help in:
- Mapping olive cultivation zones
- Agricultural monitoring
- Optimizing irrigation or treatment strategies

## 🗂️ Dataset
⚠️ Note: The full dataset is not included in this repository due to size and privacy considerations.

### 📦 Folder Structure
Please organize your olive patch dataset like this:
```
dataset/
├── chemlali/
│   ├── img1.jpg
│   └── ...
├── sbeitli/
│   └── ...
├── improved_chemchali/
│   └── ...
```
Each subfolder name represents a class or olive type.

## 🛠️ How to Run
1. Clone the repository
```bash
git clone https://github.com/yourusername/olive-classifier.git
cd olive-classifier
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Prepare your dataset  
Put your data in the `dataset/` folder following the structure above.

4. Train the model
```bash
python src/train.py
```

## ⚙️ Model Parameters
- Image size: 128x128
- Batch size: 32
- Epochs: 20
- Augmentations: horizontal flip, rotation, zoom, shift, etc.
- Model is saved to `olive_model.h5`

## 🧪 Example Output
During training, the script shows class indices and logs accuracy/loss. The model will be saved after training.

## ✍️ Author
Team KHALLIHA 3ALA LAHH – AI Engineering Students @ HIDE (Higher Institute of Digital Engineering), Tunis 

## 📜 License
This project is open source under the MIT License. You may adapt it for academic or research purposes.
