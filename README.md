# Dropdown
A reusable React Dropdown component that allows customizable menu selections, ideal for forms and settings.

This React Dropdown component provides a customizable and reusable menu selection element for web applications. It accepts a label, options, the current value, and an onChange handler as props. The options prop is an array of objects with label and value properties, which populate the dropdown menu. The component is lightweight, easily integrable, and ensures a consistent user interface across your application. Ideal for forms and settings where dropdown selections are required.

Key features:

Customizable options
Simple integration
Reusable in multiple contexts

## FOR USE IT
To integrate the Dropdown component in your React project, create the Dropdown component, import it into your main component, and use it with appropriate props (label, options, value, onChange). 
Ensure React is set up and your application is running correctly.

### EXEMPLE
In your main component file, for example, App.js, import and use the Dropdown component:
import React, { useState } from 'react';
import Dropdown from './Dropdown';

const App = () => {
  const [selectedOption, setSelectedOption] = useState('');
  const options = [
    { label: 'Option 1', value: 'option1' },
    { label: 'Option 2', value: 'option2' },
    { label: 'Option 3', value: 'option3' },
  ];

  return (
    <div>
      <h1>Welcome to My App</h1>
      <Dropdown
        label="Choose an option"
        options={options}
        value={selectedOption}
        onChange={(e) => setSelectedOption(e.target.value)}
      />
    </div>
  );
};

export default App;
