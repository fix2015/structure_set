# Set Data Structure in JavaScript 🚀  

A simple implementation of the **Set** data structure in JavaScript. This repository demonstrates how to create a set class with essential methods and explains its functionality with practical examples.  

---

## What is a Set?  
A **Set** is a collection of unique elements, meaning no duplicates are allowed. It is an unordered data structure that allows efficient membership tests, additions, and deletions. Sets are often used when you need to ensure that no duplicates exist in a collection.  

---

## Features  
- **Add**: Add a new element to the set.  
- **Delete**: Remove an element from the set.  
- **Has**: Check if an element exists in the set.  
- **Size**: Get the number of elements in the set.  
- **Clear**: Remove all elements from the set.  

---

## Code Implementation  

Here’s the JavaScript implementation of the set:  

```javascript
class Set {
    constructor() {
        this.items = {}; // Store elements as object keys
    }

    // Add an element to the set
    add(element) {
        if (!this.has(element)) {
            this.items[element] = element;
        }
    }

    // Remove an element from the set
    delete(element) {
        if (this.has(element)) {
            delete this.items[element];
        }
    }

    // Check if an element exists in the set
    has(element) {
        return this.items.hasOwnProperty(element);
    }

    // Get the size of the set
    size() {
        return Object.keys(this.items).length;
    }

    // Clear all elements from the set
    clear() {
        this.items = {};
    }
}
```

---

## Example Usage  

```javascript
// Initialize the set
const set = new Set();

// Add elements to the set
set.add(1);
set.add(2);
set.add(3);

// Check if an element exists
console.log(set.has(2)); // Output: true
console.log(set.has(4)); // Output: false

// Get the size of the set
console.log(set.size()); // Output: 3

// Remove an element from the set
set.delete(2);
console.log(set.has(2)); // Output: false

// Clear the set
set.clear();
console.log(set.size()); // Output: 0
```

---

## Real-World Applications  
1. **Removing Duplicates**: Ensuring unique elements in collections such as arrays.  
2. **Membership Testing**: Efficiently checking if an element exists in a collection.  
3. **Set Operations**: Performing union, intersection, and difference between sets.  
4. **Data Validation**: Ensuring that data doesn't contain duplicates before processing.  

---

## TikTok Tutorial 🎥  
Want to see a quick tutorial on how to build this? Check out this TikTok video:  
[]()  

---

## How to Run the Code  
1. Clone the repository:  
   ```bash
   git clone https://github.com/fix2015/structure_set
   cd structure_set
   ```
2. Open the file `index.js` in your favorite code editor.  
3. Run the file using Node.js:  
   ```bash
   node index.js
   ```

---

## Contributing  
Contributions are welcome! If you have suggestions or want to add new features, feel free to create a pull request.  

---

## License  
This project is licensed under the MIT License.  

---

## Connect with Me:
- [LinkedIn - Vitalii Semianchuk](https://www.linkedin.com/in/vitalii-semianchuk-9812a786/)
- [Telegram - @jsmentorfree](https://t.me/jsmentorfree) - We do a lot of free teaching on this channel! Join us to learn and grow in web development.
- [Tiktok - @jsmentoring](https://www.tiktok.com/@jsmentoring) Everyday new videos
- [Youtube - @jsmentor-uk](https://www.youtube.com/@jsmentor-uk) Mentor live streams
- [Dev.to - fix2015](https://dev.to/fix2015) Javascript featured, live, experience but about Set
