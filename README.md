// Define arrays of first names and last names
const firstNames = ['Emma', 'Liam', 'Olivia', 'Noah', 'Ava', 'William', 'Sophia', 'James', 'Isabella', 'Oliver'];
const lastNames = ['Smith', 'Johnson', 'Brown', 'Garcia', 'Miller', 'Davis', 'Rodriguez', 'Martinez', 'Jackson', 'Lee'];

// Function to generate a random name
function generateName() {
  // Select a random first name
  const randomFirstNameIndex = Math.floor(Math.random() * firstNames.length);
  const randomFirstName = firstNames[randomFirstNameIndex];
  
  // Select a random last name
  const randomLastNameIndex = Math.floor(Math.random() * lastNames.length);
  const randomLastName = lastNames[randomLastNameIndex];
  
  // Combine the selected first name and last name
  const randomName = randomFirstName + ' ' + randomLastName;
  
  // Display the random name on the webpage
  const randomNameElement = document.getElementById('random-name');
  randomNameElement.innerText = randomName;
}
