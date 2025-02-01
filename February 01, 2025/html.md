## **What is HTML?** 🖥️  

**HTML (HyperText Markup Language)** is the standard language used to create web pages. It **structures** the content on a webpage using **elements** like headings, paragraphs, images, links, and more.  

---

### **1. Basic Structure of an HTML Page**  
```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph of text.</p>
    <a href="https://example.com">Click here</a>
</body>
</html>
```
#### **Explanation:**
- `<!DOCTYPE html>` – Defines the document as HTML5.  
- `<html>` – The root of the webpage.  
- `<head>` – Contains metadata (title, links to stylesheets, etc.).  
- `<title>` – Sets the page title (appears in the browser tab).  
- `<body>` – The visible content of the webpage.  
- `<h1>` – A heading.  
- `<p>` – A paragraph.  
- `<a>` – A hyperlink.  

---

### **2. Common HTML Elements**
| **Element** | **Description** |
|------------|---------------|
| `<h1> to <h6>` | Headings (largest to smallest). |
| `<p>` | Paragraphs. |
| `<a href="">` | Links to other pages. |
| `<img src="" alt="">` | Displays images. |
| `<ul>, <ol>, <li>` | Unordered & ordered lists. |
| `<table>` | Creates tables. |
| `<div>` | A container for organizing content. |
| `<form>` | Creates input forms. |

---

### **3. Why Use HTML?**
✅ **Structures web pages**  
✅ **Works with CSS & JavaScript** to style and add interactivity  
✅ **Used in web development, blogs, e-commerce, and more**  


## Here's an overview of the core elements in HTML:

### Basic Structure:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Page Title</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

### Basic Tags:

1. **Headings** (`<h1>` to `<h6>`):
   Used for titles or section headings, with `<h1>` being the most important.
   ```html
   <h1>This is a level 1 heading</h1>
   <h2>This is a level 2 heading</h2>
   ```

2. **Paragraph** (`<p>`):
   Defines a paragraph of text.
   ```html
   <p>This is a paragraph of text.</p>
   ```

3. **Links** (`<a>`):
   Used to create hyperlinks.
   ```html
   <a href="https://www.example.com">Visit Example</a>
   ```

4. **Images** (`<img>`):
   Embeds an image in the page.
   ```html
   <img src="image.jpg" alt="Description of the image">
   ```

5. **Lists**:
   - **Unordered list** (`<ul>`):
     ```html
     <ul>
         <li>Item 1</li>
         <li>Item 2</li>
     </ul>
     ```
   - **Ordered list** (`<ol>`):
     ```html
     <ol>
         <li>First item</li>
         <li>Second item</li>
     </ol>
     ```

6. **Divisions** (`<div>`):
   Used to group content together.
   ```html
   <div>
       <h2>Section Title</h2>
       <p>Some content.</p>
   </div>
   ```

7. **Semantic HTML Tags**:
   These tags help define the structure of the document and make it more accessible:
   - `<header>`: Represents the header of a page or section.
   - `<footer>`: Represents the footer of a page or section.
   - `<article>`: Represents a self-contained piece of content.
   - `<section>`: Represents a section of related content.
   - `<nav>`: Represents a navigation block (e.g., menu links).
   - `<aside>`: Represents content that is tangentially related to the content around it.

### Example of a Simple Webpage:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Home Section</h2>
            <p>This is the home section of the webpage.</p>
        </section>
        <section id="about">
            <h2>About Section</h2>
            <p>This is the about section of the webpage.</p>
        </section>
        <section id="contact">
            <h2>Contact Section</h2>
            <p>Feel free to contact us!</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Website</p>
    </footer>
</body>
</html>
```

### Practice with Semantic HTML:
You can practice creating your webpage structure using these elements. Start by creating a layout for a simple website like a portfolio or blog, organizing your content using the appropriate semantic tags. 


