# Fluid Typography vs Breakpoints

This project demonstrates the differences between **Fluid Typography** and **Breakpoint-based Typography** using HTML, CSS, and JavaScript. It provides practical examples to understand how text scaling behaves across different viewport sizes.

## 📌 Features
- **Navbar with Bootstrap**: A responsive navigation bar with a custom SVG menu icon.
- **Fluid Typography Example**: Uses `clamp()` to dynamically scale text sizes.
- **Breakpoint-based Typography Example**: Uses media queries to set font sizes at specific breakpoints.
- **Live Font Size Display**: Shows the current font sizes of elements dynamically.
- **CSS Best Practices**: Includes comments explaining styling decisions.

## 📂 Folder Structure
```
project-folder/
│-- index.html             # Main file with navbar and typography demo
│-- typography-example-1.html  # Demo using clamp() for responsive typography
│-- typography-example-2.html  # Demo using traditional breakpoints
│-- css/
│   ├── index.css          # Styles for index.html
│-- assets/
│   ├── fonts/             # (Optional) Custom fonts can be added here
│-- README.md              # Documentation file
```

## 🚀 Getting Started
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```
### 2️⃣ Open in a Browser
Simply open `index.html` in your preferred browser.

### 3️⃣ Optional: Run with Live Server
For better development experience, use Live Server in VS Code:
1. Install the **Live Server** extension.
2. Right-click `index.html` → Select **"Open with Live Server"**.

## 🛠️ Technologies Used
- **HTML5** - Markup structure
- **CSS3** - Styling and typography management
- **Bootstrap 5** - Navbar and responsive utilities
- **JavaScript** - Dynamic font size updates

## 📝 Usage
- Resize the browser window to see how typography behaves in each example.
- Compare the effectiveness of `clamp()` vs traditional breakpoints.
- Click on links to external resources for further learning.

## 🌟 References
- [Smashing Magazine: Modern Fluid Typography](https://www.smashingmagazine.com/2022/01/modern-fluid-typography-css-clamp/)
- [Clamp Calculator](https://www.marcbacon.com/tools/clamp-calculator/)

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).

---
💡 *Feel free to contribute by improving the examples or adding new insights!*



# typography-vs-breakpoints

typography vs breakpoints: when to use

![typography vs breakpoints: when to use](screenshots/screencapture-127-0-0-1-8000-Fluid-Typography-vs-Breakpoints-html-2024-12-04-19_00_25.png)

### Example usage 1: Responsive text

![Example with Real time Value: Responsive <p> <a> <h1>](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-1-html-2024-12-04-19_01_52.png)

### Example usage 2: Responsive padding and text

#### The entire text will scale between 1rem at 575px and 1.5rem at 1024px

#### Desktop devices max-width > 1024px

![Example with Real Time Value: Responsive <p> and .container padding](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-2-html-2024-12-04-19_03_18.png)

#### Mobile device max-width == 325px

![Responsive typography for mobile device max-width < 325px](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-2-html-2024-12-04-19_07_06.png)

#### Mobile Device Width == 375px

![Responsive typography for mobile device max-width == 375px](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-2-html-2024-12-04-19_11_09.png)

#### Mobile Device Max-Width == 425px

![Responsive typography for mobile device max-width == 425px](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-2-html-2024-12-04-19_13_06.png)

#### Tablet Screen Size == 768px

![Responsive typography for mobile device max-width == 768px](screenshots/screencapture-127-0-0-1-8000-typograpgy-example-2-html-2024-12-04-19_14_19.png)

### Responsive togglenav-bar for mobile device

```
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Home</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarTogglerDemo02"
          aria-controls="navbarTogglerDemo02"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            x="0px"
            y="0px"
            width="50"
            height="50"
            viewBox="0 0 50 50"
            class="custom-navbar-toggler-icon"
          >
            <!-- Add or rewrite the attribute of fill of every path to fill="currentColor" -->
            <!-- Also you may have to change stroke attributes to stroke="currentColor" -->
            <path
              fill="currentColor"
              stroke="currentColor"
              d="M 0 9 L 0 11 L 50 11 L 50 9 Z M 0 24 L 0 26 L 50 26 L 50 24 Z M 0 39 L 0 41 L 50 41 L 50 39 Z"
            ></path>
          </svg>
        </button>

        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="typograpgy-example-1.html"
                >Example-1</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link active" href="typograpgy-example-2.html">Example-2</a>
            </li>
          </ul>
          <form class="d-flex">
            <input
              class="form-control me-2"
              type="search"
              placeholder="Search"
              aria-label="Search"
            />
            <button class="btn btn-outline-success" type="submit">Search</button>
          </form>
        </div>
      </div>
    </nav>
```

### Add custom nav-toggler-icon added to nav-bar

#### Option-1:

```
<!-- Add or rewrite the attribute of fill of every path to fill="currentColor" -->
    <!-- Also you may have to change stroke attributes to stroke="currentColor" -->
    <path
        fill="currentColor"
        stroke="currentColor"

.custom-navbar-toggler-icon
  {
    width: 24px; /* Adjust size if needed */
    height: 24px;
    color: burlywood;
  }


```

#### Option-2 Use <img> for loading svg and set color in CSS3
