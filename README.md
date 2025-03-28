# Calculator Microservice
This is a simple calculator microservice built using Node.js and Express.js, with logging implementation using Winston.

## Things we need to install before we start this task: 
- Node.js 
- NPM 

## Installation:
1. Clone the repository:
   git clone https://github.com/Deakin-Rohit-Radhakrishnan/sit737-2025-prac4p.git
   cd sit737-2025-prac4p
2. Install dependencies:
   npm install

### To Run the program:
Run the following command to start the microservice:
node calculator.js

### API Endpoints:
Use the following HTTP endpoints to perform calculations:
Addition - `GET /add` 
Subtraction - `GET /sub` 
Multiplication - `GET /mul` 
Division - `GET /div` 

### To test if the application is running:
Open a new browser andd type in the URL:
http://localhost:3040/add?n1=10&n2=5

Output:

{
    "statuscode": 200,
    "result": 15
}


### Logging:
- All operations are logged in `logs/combined.log`.
- All errors are logged in `logs/error.log`.

### To view logs in real-time:
tail -f logs/combined.log
tail -f logs/error.log

## Error Handling:
- If division by zero is attempted, an error is logged and returned.
- If non-numeric values are provided, an error is logged and returned.