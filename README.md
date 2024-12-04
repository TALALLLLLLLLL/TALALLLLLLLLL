async function analyzeImage() {
    const fileInput = document.getElementById('fileInput');
    const resultText = document.getElementById('result');
    if (fileInput.files.length === 0) {
        resultText.innerText = 'Please upload a photo!';
        return;
    }

    const file = fileInput.files[0];
    resultText.innerText = 'Analyzing...';

    // Mock result since AI isn't set up yet.
    setTimeout(() => {
        resultText.innerText = 'This looks like plastic. Please recycle i
