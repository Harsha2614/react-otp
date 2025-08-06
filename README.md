# React OTP Input Component

This project demonstrates a simple and reusable OTP (One-Time Password) input component built using React. It leverages React Hooks like useState, useRef, and useEffect to handle user interactions such as typing digits, navigating between input boxes with arrow keys, deleting with backspace, and pasting the entire OTP at once. The component is dynamic, allowing the OTP length to be customized through props.

The OTP component consists of multiple single-character input fields aligned side by side. When a user types a digit, the focus automatically moves to the next input. Arrow keys (ArrowLeft and ArrowRight) let the user navigate between inputs, while the backspace key clears the digit and moves the focus back when appropriate. Additionally, if a user pastes an OTP, it intelligently fills the input fields from the beginning and adjusts the focus to the next unfilled box.

The project structure is simple, containing a main App.jsx file that renders the OTP component, and a components/OTP.jsx file where the actual logic resides. Basic styling for layout and input appearance is included in index.css, which can be customized as needed. The default OTP length is set to 6, but it can be easily changed by passing a different otpLength prop.

To run the project, clone the repository and install the necessary dependencies using npm install. You can start the development server using npm run dev if using Vite, or npm start if using Create React App. Once the server is running, you will see the OTP input component rendered on the page, fully functional with keyboard and paste interactions.

This component is an excellent example of how to manage focus and user input across multiple fields using React’s useRef and how to control input state using useState. The initial focus is handled via useEffect to ensure the first input is active when the component mounts. The component is designed to be modular and reusable in any project that requires OTP verification functionality.

The project styling is kept minimal and clean with CSS classes for container layout and input field styling. You can easily extend the component’s look and feel to match your application’s theme. For a better understanding of React Hooks, refer to resources like the Daily.dev blog on React Hooks or tutorials explaining React components in depth. This project is open-source and can be freely modified and used in personal or professional projects.

# Commands to Run

## If you are using Vite:


npm create vite@latest react-otp -- --template react

cd otp-react-app

npm install

npm run dev

# If you are using Create React App (CRA):

npx create-react-app otp-react-app
cd otp-react-app
npm install
npm start
