# 🖥️ Memory-Detector 🚀  

## 📌 Overview
This is a **C/C++ Memory Detector** Library. It maintains two databases:

- 📂 **Structure Database** 🏗️  
- 📂 **Object Database** 🗂️  

The **user application** registers all its structures with the MLD Library during initialization.  
Whenever the application **xcalloc()** an object, an **object record entry** is inserted into the object database.  
If there is a **memory leak** in the application code, the **"report_leaked_objects()"** function detects it 🛑.  

---

## ⚙️ Compilation 🛠️  
To compile the Memory Leak Detector Library and user application, run the following commands:

```bash
# Compile MLD Library  
gcc -g -c mld.c -o mld.o  

# Compile User Application  
gcc -g -c app.c -o app.o  

# Link and Create Executable  
gcc -g app.o mld.o -o exe  
```

---

## 🧪 Testing 🧑‍💻  
To test the Memory Leak Detector:

1️⃣ Modify the **app.c** file and introduce some **memory leaks** 💀.  
2️⃣ Compile using the commands above.  
3️⃣ Run the executable:

```bash
./exe
```

🛠️ **Detect and fix memory leaks like a pro!** 🚀

## High Level Design

![hld](https://user-images.githubusercontent.com/47227715/138119173-d18d1baf-ca91-44f9-a1fb-bf096e4aa106.png)


## Testing MLD Library

