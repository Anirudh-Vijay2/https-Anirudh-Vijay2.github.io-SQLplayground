# **SQL Playground**

A lightweight, interactive, and fully functional SQL playground that runs entirely in your web browser. This tool allows users to practice SQL queries against a real database without needing to set up a server or local environment.

## **🚀 Features**

* **In-Browser SQLite Engine**: Powered by sql.js (SQLite compiled to WebAssembly), providing a real relational database experience in the client.  
* **Interactive Query Editor**: A code-focused editor with support for standard SQL syntax.  
* **Live Schema Explorer**: A dynamic sidebar that displays your current database tables, their column definitions, and live row counts.  
* **One-Click Table View**: Quickly inspect table data using the "Play" icon next to table names in the schema list.  
* **Responsive Design**: Built with Tailwind CSS, ensuring the playground works seamlessly on desktops, tablets, and mobile devices.  
* **Pre-seeded Dummy Data**: Comes pre-populated with Users and Products tables to help you start practicing SELECT, JOIN, and GROUP BY clauses immediately.  
* **Factory Reset**: A robust reset feature that clears the local session and restores the default environment via a page refresh.  
* **Toast Notifications**: Real-time feedback for successful query executions and database resets.

## **🛠️ Tech Stack**

* **HTML5 & CSS3**: Structural layout.  
* **Tailwind CSS**: Modern, utility-first styling for a responsive and clean UI.  
* **sql.js**: The core SQL engine (SQLite WASM).  
* **Google Fonts**: Integrated "Fira Code" for a developer-friendly editor experience.

## **📖 How to Use**

1. **Write Queries**: Enter any valid SQL command (e.g., SELECT, INSERT, UPDATE, CREATE TABLE) into the Query Editor.  
2. **Execute**: Click the **"Run Query"** button or press Ctrl \+ Enter (Windows/Linux) or Cmd \+ Enter (Mac).  
3. **Inspect Results**: View the output in the Results Explorer. Successful queries return a formatted table, while errors are displayed with helpful feedback.  
4. **Explore Schema**: Use the sidebar to expand table definitions or click the play button to instantly run SELECT \* on a specific table.  
5. **Reset**: Use the **"Reset & Refresh"** button to wipe your local changes and bring back the original demo data.

## **💡 Example Queries**

### **Simple Select**

SELECT \* FROM Users;

### **Joining Tables**

SELECT name, price FROM Products WHERE price \> 500;

### **Using the Describe Alias**

You can use the custom DESCRIBE command added to this playground:

DESCRIBE Users;

*(This automatically translates to PRAGMA table\_info(Users);)*

## **📄 License**

This project is open-source and free to use for educational purposes.