//Problem 1: Task Management System
// Array to store tasks
let tasks = [];

// 1. Add Task: Arrow function to add a new task
const addTask = (title, status, priority) => {
    tasks.push({ title, status, priority });
};

// 2. Filter by Status: Return tasks based on their status
const filterByStatus = (status) => tasks.filter(task => task.status === status);

// 3. Find High Priority Task: Get the first task with priority 5
const findHighPriorityTask = () => tasks.find(task => task.priority === 5);

// 4. Map Task Titles: Format task titles with their status
const mapTaskTitles = () => tasks.map(task => `Task: ${task.title}, Status: ${task.status}`);

// Log task details in a readable format
const logTasks = () => {
    tasks.forEach(task => {
        console.log(`Task: ${task.title}, Status: ${task.status}, Priority: ${task.priority}`);
    });
};

// Example Usage
addTask("Buy Groceries", "Pending", 3);
addTask("Clean Room", "Completed", 2);
addTask("Finish Assignment", "Pending", 5);
console.log(filterByStatus("Pending"));
console.log(findHighPriorityTask());
console.log(mapTaskTitles());
logTasks();


//Problem 2: Online Shopping Cart
// Array to store cart products
let cart = [];

// 1. Add Product: Add a new product to the cart
function addProduct(productName, price, quantity) {
    cart.push({ productName, price, quantity });
}

// 2. Calculate Total: Calculate total cost of items in the cart
const calculateTotal = () => cart.reduce((total, product) => total + product.price * product.quantity, 0);

// 3. Remove Product: Remove a product by name
const removeProduct = (productName) => {
    cart = cart.filter(product => product.productName !== productName);
};

// 4. Log product details
const logCart = () => {
    cart.forEach(({ productName, price, quantity }) => {
        console.log(`Product: ${productName}, Price: $${price}, Quantity: ${quantity}`);
    });
};

// Example Usage
addProduct("Laptop", 1000, 1);
addProduct("Mouse", 50, 2);
console.log(`Total: $${calculateTotal()}`);
removeProduct("Mouse");
logCart();


//Problem 3: Weather Forecast Tracker
// Array to store city weather data
let cityWeather = [];

// 1. Add City Weather: Add a new city weather object
function addCityWeather(cityName, temperature, condition) {
    cityWeather.push({ cityName, temperature, condition });
}

// 2. Find Hottest City: Identify city with the highest temperature
const findHottestCity = () => cityWeather.reduce((hottest, city) => city.temperature > hottest.temperature ? city : hottest, cityWeather[0]);

// 3. Filter by Condition: List all cities with a specific condition
const filterByCondition = (condition) => cityWeather.filter(city => city.condition === condition);

// 4. Map City Names with Temperatures
const mapCityNames = () => cityWeather.map(({ cityName, temperature }) => `City: ${cityName}, Temp: ${temperature}°C`);

// 5. Log all city details
const logWeather = () => {
    cityWeather.forEach(({ cityName, temperature, condition }) => {
        console.log(`City: ${cityName}, Temp: ${temperature}°C, Condition: ${condition}`);
    });
};

// Bonus: Convert temperature between Celsius and Fahrenheit
const convertTemperature = (temp, unit) => unit === "F" ? (temp * 9/5) + 32 : (temp - 32) * 5/9;

// Example Usage
addCityWeather("New York", 25, "Sunny");
addCityWeather("London", 15, "Cloudy");
addCityWeather("Mumbai", 35, "Rainy");
console.log(findHottestCity());
console.log(filterByCondition("Sunny"));
console.log(mapCityNames());
logWeather();
console.log(`Temp in Fahrenheit: ${convertTemperature(25, "F").toFixed(2)}°F`);

