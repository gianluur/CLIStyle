# 🌈 CLIStyle: Style Your Terminal Outputs with Colors and Styles 

### A lightweight, cross-platform C++ library to add **colors**, **backgrounds**, and **styles** to your terminal output. 🚀

## ✨ Features

- 🎨 **Colorful Outputs**: Style text and backgrounds with standard, bright colors and custom RGB colors.
- 💎 **Text Formatting**: Support for **bold**, *italic*, **underline**, and **reverse** text.
- ⚡ **Cross-Platform**: Works seamlessly on Windows, macOS, and Linux.
- 🛠️ **Easy-to-Use**: Intuitive syntax and every function is documented.

## 🎨 Colors
- 🟥 Red / Bright Red
- 🟦 Blue / Bright Blue
- 🟩 Green / Bright Green
- 🟨 Yellow / Bright Yellow
- 🟪 Magenta / Bright Magenta
- 🟦 Cyan / Bright Cyan
- ⬜ White 
- ⬛ Grey
- 🖌️ Custom
  
## 📝 Text Styles
- **Bold**: ✨ Highlight your text
- *Italic*: 🎩 Stylish text
- <ins>Underline</ins>: 📏 Draw attention
- Reverse: 🔄 Swap text and background colors

---

## 📸 Demo
![Screenshot 2024-12-09 150751](https://github.com/user-attachments/assets/e62a71a8-968b-4f56-9538-614388ad0bdb)

## 📌 Usage
### 🎨 Every standard color has 6 dedicated function:
1. Colors text by default, a version for stream usage like in std::cout, and a version that returns the colored string  
2. Colors background by default, a version for stream usage like in std::cout, and a version that returns the colored string  
3. Using templates you can choose where to color ( 0: background or CLIStyle::BACKGROUND, 1: foreground or CLIStyle::TEXT )
   
![Screenshot 2024-12-09 202630](https://github.com/user-attachments/assets/ec9322c0-16b6-4ad2-b9ac-5d4f450a9b11)
![Screenshot 2024-12-09 214927](https://github.com/user-attachments/assets/9e3319d4-edd1-40f8-93d3-6ae4c1480169)

### 🖌️ For creating custom colors there are 6 dedicated functions:
1. Colors text by default, a version for stream usage like in std::cout, and a version that returns the colored string
    - R,G,B: Every argument rappresent a primitive color, that ranges from 0 to 255
2. Colors background by default, a version for stream usage like in std::cout, and a version that returns the colored string
    - R,G,B: Every argument rappresent a primitive color, that ranges from 0 to 255
3. Uses template you can choose where to color:
    - Position: Where should the color be applied ( 0: background or CLIStyle::BACKGROUND, 1: foreground or CLIStyle::TEXT )
    - R,G,B: Every argument rappresent a primitive color, that ranges from 0 to 255
   
![Screenshot 2024-12-09 210424](https://github.com/user-attachments/assets/778e17ac-92aa-4de1-a5c0-84fc968312aa)
![Screenshot 2024-12-09 214939](https://github.com/user-attachments/assets/fff3a5d4-21cf-48d8-9952-6fcfdbaba3c8)
---

### ✒️ Every text style has 2 dedicated function:
A function to styles the stream and a function that returns the styled string

![Screenshot 2024-12-09 214114](https://github.com/user-attachments/assets/9014a12f-95e2-495b-821c-7f781a9b7708)
![Screenshot 2024-12-09 214955](https://github.com/user-attachments/assets/e98dcb19-7852-4cfc-9eed-df1d4f932105)
---

### ⚠️Important

Every function that is used directly in streams, **WILL COLOR THE ENTIRE STREAM**.

After coloring/styling a stream you should use << reset() at the end of it if you want to concatenate other streams.
If you need to use a newline character whether it'll be '\n' or endl(), put it after the reset() function.
The reset function can also be used to return a styled string to remove it's colring/style

---

## 📦 Installation
1. **Clone the repository**
```bash
  git clone https://github.com/gianluur/CLIStyle.git
```
2. **Add to your project**
```cpp
  #include "your/path/to/clistyle.hpp
```

---

## 📜 License
This project is licensed under the MIT License. Feel free to use, modify, and distribute this software as per the license terms.

## 🌟 Support
If you like this project, please give it a ⭐ on GitHub!
For any issues or suggestions, feel free to open an issue.
