#### *Let's Practice Making API Requests with cURL*  

✅ **Task 1: Fetch a Random Cat Fact**  
   - Use the **Cat Facts API** to fetch a random fact:  
     ```bash
     curl https://catfact.ninja/fact
     ```  
   - **Response Example:**  
     ```json
     {
         "fact": "Cats sleep for 70% of their lives.",
         "length": 37
     }
     ```  

✅ **Task 2: Fetch London’s Weather Data**  
   - Use the **OpenWeather API** with your API key:  
     ```bash
     curl -X GET "https://api.openweathermap.org/data/2.5/weather?q=London&appid=YOUR_API_KEY&units=metric"
     ```  
   - **Response Example:**  
     ```json
     {
         "main": {
             "temp": 10.5,
             "humidity": 75
         },
         "weather": [
             {
                 "description": "overcast clouds"
             }
         ]
     }
     ```  

✅ **Task 3: Use Parameters to Customize the Request**  
   - Example: Change the city to Tokyo and add units in Fahrenheit:  
     ```bash
     curl -X GET "https://api.openweathermap.org/data/2.5/weather?q=Tokyo&appid=YOUR_API_KEY&units=imperial"
     ```  

✅ **Task 4: Debug an API Error**  
   - Use a **wrong API key** and observe the error response:  
     ```bash
     curl -X GET "https://api.openweathermap.org/data/2.5/weather?q=London&appid=INVALID_KEY"
     ```  
   - Example Error Response:  
     ```json
     {
         "cod": 401,
         "message": "Invalid API key."
     }
     ```  

#### **Activity:**  
🛠️ Students test these commands on their terminals and share their results.  
