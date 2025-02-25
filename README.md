# **Efficient Goods Loading System for Hanoi Roadways**  

## **Project Overview**  
This project aims to develop an **optimized goods loading system** for **Hanoi Roadways** to improve efficiency in truck parcel loading and delivery. The system uses **data structures and algorithms** to systematically arrange and pack parcels into trucks, ensuring **optimized space utilization, easy unloading, and reduced delivery time**.  

## **Key Features**  

- **Efficient Truck Loading Algorithm:** Implements **Best Fit Decreasing (BFD)** from the **Bin Packing Problem** to optimize space utilization.  
- **Systematic Parcel Organization:** Sorts parcels by **weight and destination**, ensuring easy unloading.  
- **Data Structures Used:**  
  - **Stack:** Ensures last-in-first-out (LIFO) unloading.  
  - **List:** Stores parcels in trucks.  
  - **Set:** Tracks destinations.  
  - **Dictionary:** Maps destinations to distances.  
- **Automated Invoice Generation:** Each parcel gets an invoice with details like **Parcel ID, weight, destination, and cost**.  
- **Graphical User Interface (GUI):** Allows users to **add parcels, pack trucks, and generate reports**.  

## **Project Structure**  

```
📁 Efficient-Goods-Loading-System  
 ┣ 📂 invoices/         # Sample output data  
 ┣ 📜 README.md         # Project documentation  
 ┣ 📜 input_data.xlsx   # Sample parcel data  
 ┣ 📜 assignment.py     # Core implementation of the loading algorithm  

## **Setup Instructions**  

### **1. Prerequisites**  
Ensure you have the following installed:  
- **Python 3.x**  
- **Pandas & OpenPyxl (for Excel file handling)**  
- **Tkinter (for GUI interface)**  

### **2. Run the Application**  
To start the truck loading system, execute:  
```sh
python assignment.py
```  

## **Algorithm Overview**  

The project utilizes the **Best Fit Decreasing (BFD) algorithm** to optimize truck loading:  

1. **Sort parcels** by weight in **descending order**.  
2. **Allocate parcels** to trucks using **best fit** (smallest remaining space).  
3. **Pack trucks** systematically, placing **last-to-deliver parcels first** for easy unloading.  
4. **Generate invoices** automatically with relevant parcel details.  

## **Sample Data**  

### **Input Data Example**  

| Parcel ID | Weight (kg) | Destination | Customer Name |  
|-----------|------------|-------------|---------------|  
| P564814   | 23         | HCMC        | Hikaru        |  
| P132493   | 62         | HCMC        | Hwee          |  
| P987007   | 34         | Dalat       | Ngoc          |  
| P212457   | 123        | Da Nang     | Diep          |  

### **Output Data Example** (Generated Invoice)  

| Parcel ID | Destination | Weight (kg) | Distance (km) | Cost ($) | Customer Name |  
|-----------|------------|------------|--------------|---------|---------------|  
| P987007   | Dalat      | 34         | 250          | 80.5    | Ngoc          |  

## **Contributors**  
- **Hikaru2035** (Project Owner)  
