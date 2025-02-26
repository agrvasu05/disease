# EcoScan - Plant Disease Detection & Carbon Footprint Calculator

EcoScan is a web-based platform that helps users identify plant diseases through image analysis and calculate their carbon footprint based on lifestyle factors. This project combines environmental awareness with AI-driven insights.

## Features

### 🌿 Plant Disease Detection
- Upload plant images to detect diseases using an AI-based model.
- Get instant results with the disease name and suggested remedies.
- User-friendly interface with drag-and-drop image uploading.

### 🌎 Carbon Footprint Calculator
- Input transportation, energy, food, and consumption data.
- Get an estimate of your annual CO₂ emissions.
- Compare your footprint with the global average and get personalized reduction tips.

## Technologies Used
- **Frontend**: HTML, CSS, JavaScript
- **API for Plant Detection**: Integrated with `https://susya.onrender.com`
- **Data Processing**: JavaScript-based calculations for carbon footprint estimation

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/ecoscan.git
   ```
2. Navigate to the project directory:
   ```sh
   cd ecoscan
   ```
3. Open `index.html` in your browser.

## Usage
- Click on **Plant Scanner** to upload an image and detect plant diseases.
- Click on **Carbon Calculator** to enter usage data and estimate your carbon footprint.
- Review results and take action based on the suggestions provided.

## API Integration
For plant disease detection, the project interacts with an API:
```js
fetch("https://susya.onrender.com", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ image: uploadedBase64 })
})
.then(response => response.json())
.then(data => {
    console.log(data); // Display detected plant disease info
})
.catch(error => console.error("Error analyzing image:", error));
```

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Added new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For inquiries or collaboration, reach out via:
- GitHub Issues
- Email: your.email@example.com

Happy coding! 🚀🌱
