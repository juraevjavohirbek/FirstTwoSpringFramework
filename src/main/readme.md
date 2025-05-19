this is simple web application wich shows name which is written in url.
http://localhost:8080/greeting?name=Javohirbek
HelloController receives the request through the @GetMapping("/greeting") method
It extracts the name parameter from the URL (or defaults to "World" if none is provided).
It adds this value to the model as an attribute (model.addAttribute("name", name))
Thymeleaf processes the HTML and replaces ${name} with the actual value from the model (e.g., "Javohirbek").
The final page shows a greeting like:
Hello, Alice!
![Screenshot 2025-05-19 085132.png](Screenshot%202025-05-19%20085132.png)

