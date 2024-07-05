# Calorie Counter

Welcome to the **Calorie Counter** repository! This project is a simple web application written in HTML, CSS, and JavaScript. The application helps users track their daily calorie intake.

## Features

- **Add Meals**: Log meals with their respective calorie counts.
- **Track Total Calories**: Automatically calculate and display the total calories consumed.
- **Interactive Interface**: Simple and intuitive user interface for easy meal logging.
- **Responsive Design**: Works seamlessly on both desktop and mobile devices.

## Technologies

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla JS)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/calorie-counter.git
   cd calorie-counter
   ```

2. **Open the index.html file**:
   - You can open the `index.html` file directly in your web browser to use the Calorie Counter.

## Usage

1. Open the Calorie Counter in your web browser.
2. Log your meals by entering the meal name and its calorie count.
3. The application will automatically calculate and display the total calories consumed.

## Project Structure

- `index.html`: The main HTML file for the Calorie Counter.
- `style.css`: CSS file for styling the application.
- `script.js`: JavaScript file for handling the calorie tracking functionality.

## Example

Here’s a simple example of the JavaScript code used to log meals and calculate total calories:

```javascript
// Example of adding a meal and updating total calories
let totalCalories = 0;

document.getElementById('addMeal').addEventListener('click', function() {
  const mealName = document.getElementById('mealName').value;
  const mealCalories = parseInt(document.getElementById('mealCalories').value);
  
  if (mealName && !isNaN(mealCalories)) {
    totalCalories += mealCalories;
    document.getElementById('totalCalories').textContent = `Total Calories: ${totalCalories}`;
    
    const mealList = document.getElementById('mealList');
    const mealItem = document.createElement('li');
    mealItem.textContent = `${mealName}: ${mealCalories} calories`;
    mealList.appendChild(mealItem);
  }
});
```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to submit a pull request. Please ensure your changes align with the project goals and maintain code quality.

## License

This project is licensed under the MIT License – see the [LICENSE.md](LICENSE.md) file for details.
