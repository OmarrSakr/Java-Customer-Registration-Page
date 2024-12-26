# Customer Registration Page (Java) 💻🖱️

A **desktop application** built using *`Java`*, designed to **streamline the process of registering customers**. The application features **a clean and user-friendly interface for creating, managing, and storing customer information effectively.**

## 🛠 Technologies Used:

- `Java (Swing)`: Used for building the graphical user interface and implementing the business logic.

- `File Handling`: Utilized to save and retrieve customer data via `.txt` files for persistent storage.

## 📂 Features:

*`1. Customer Registration`*

- Add new customer details such as name, contact number, email, and address.

- Validate user input to ensure data integrity (e.g., proper email format, non-empty fields).

*`2. Search and Edit Customer Records`*

- Search for existing customers using their ID or name.

- Update customer details easily to maintain accurate records.

*`3. File-Based Data Storage`*

- Save customer information into a .txt file for long-term storage.

- Load and display customer details from the file upon application startup.

*`4. Responsive UI`*

- A desktop-friendly user interface built using Java Swing, ensuring seamless navigation and interaction.

**⚠ Current Status:**

- The project is fully functional and uses file handling for data storage instead of a database. It is currently optimized for desktop environments.

## 🔑 Example Code Snippet for Saving Data:
Below is a sample of how customer data is saved to a file:
```
// Define the file path
String fileName = "customerData.txt";
try (FileWriter fileWriter = new FileWriter(fileName, true); BufferedWriter bufferedWriter = new BufferedWriter(fileWriter)) {
    bufferedWriter.write("Customer ID: " + customerId + ", Name: " + customerName + ", Email: " + customerEmail);
    bufferedWriter.newLine();
    JOptionPane.showMessageDialog(null, "Customer details saved successfully!");
} catch (IOException e) {
    JOptionPane.showMessageDialog(null, "Error saving customer details: " + e.getMessage());
}
```
---
## How to Use 🚀  

We welcome `contributions` to **Customer Registration Page (Java)**! Here’s how you can help:
1. *Fork the repository* - Click the "Fork" button at the top right of the repository page.
2. *Clone your fork* - Use the command:
   
   ```bash
   https://github.com/OmarrSakr/Java-Customer-Registration-Page.git

---
## 💡 How to Run the Project:

1. Open the project in *`NetBeans`* Program or your favorite Java IDE (e.g., IntelliJ IDEA, Eclipse).

2. Compile and run the application.

## 🔄 Future Enhancements:

- Integrate a database system (e.g., MySQL or SQLite) for better scalability and performance.
- Implement role-based user authentication for enhanced security.
- Add support for exporting customer data to Excel or PDF.
