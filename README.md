# Chai aur Streamlit ☕

A comprehensive learning project demonstrating interactive data visualization and dashboard development using **Streamlit**. This project showcases the journey from basic interactive applications to professional-grade sales dashboards, with a delightful focus on Indian tea (chai) sales analytics.

## Overview

This repository contains a structured tutorial series that progressively teaches Streamlit fundamentals through practical examples. Each chapter builds upon the previous one, introducing new concepts and features while maintaining a consistent theme around chai sales and beverage analytics.

## Features

✨ **Learning-Focused Structure**
- Progressive chapters from beginner to intermediate level
- Hands-on examples with real-world business context
- Clean, well-commented code for easy understanding

📊 **Data Visualization**
- Interactive sales dashboards with real-time filtering
- Multi-metric KPI displays
- Regional and product-based analytics
- Revenue and unit sales tracking

🎯 **Streamlit Concepts Covered**
- Page configuration and layout management
- Interactive widgets (selectbox, multiselect, sliders)
- Data caching and performance optimization
- Sidebar navigation and filters
- Metrics display and formatting
- Responsive column layouts

## Prerequisites

Before you begin, ensure you have the following installed:

- **Python** >= 3.10
- **uv** (Fast Python package installer) - [Installation guide](https://docs.astral.sh/uv/getting-started/installation/)
- **Git** (for version control)

## Installation

This project uses **uv** for fast and reliable dependency management.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Piyush-Sarkar/Chai-aur-Streamlit.git
   cd Chai-aur-Streamlit
   ```

2. **Install dependencies with uv:**
   ```bash
   uv sync
   ```

3. **Activate the virtual environment:**
   
   **On Windows:**
   ```bash
   .venv\Scripts\activate
   ```
   
   **On macOS/Linux:**
   ```bash
   source .venv/bin/activate
   ```

**Alternative: Using pip**

If you prefer traditional pip installation:
```bash
python -m venv .venv
# Activate as shown above
pip install streamlit>=1.58.0 openpyxl>=3.1.5 pandas numpy
```

## Project Structure

```
Chai-aur-Streamlit/
├── README.md                 # Project documentation
├── pyproject.toml           # Project configuration
├── requirements.txt         # Python dependencies
├── chai_sales.csv           # Sample dataset
├── chapter-one.py           # Basic Streamlit widgets
├── chapter-two.py           # Data display and dataframes
├── chapter-three.py         # Interactive filters and layouts
├── chapter-four.py          # Advanced visualizations
├── chapter-five.py          # Complex dashboard features
└── demo-dashboard.py        # Complete sales dashboard example
```

## Getting Started

### Running Individual Chapters

Each chapter file is independent and demonstrates specific Streamlit concepts:

```bash
# Run Chapter 1 - Introduction to Streamlit
streamlit run chapter-one.py

# Run Chapter 2 - Data handling
streamlit run chapter-two.py

# Run Chapter 3 - Interactive features
streamlit run chapter-three.py

# Run Chapter 4 - Advanced features
streamlit run chapter-four.py

# Run Chapter 5 - Complex interactions
streamlit run chapter-five.py
```

### Running the Demo Dashboard

The complete example showcasing all features together:

```bash
streamlit run demo-dashboard.py
```

The app will open in your default web browser at `http://localhost:8501`

## Chapter Breakdown

### 📖 Chapter 1: Hello Chai App
**Topics:** Basic widgets, text rendering, selectbox
- Create your first interactive Streamlit app
- Learn about st.title(), st.subheader(), st.write()
- Implement simple user interactions with selectbox
- Display success messages and alerts

### 📖 Chapter 2: Data Fundamentals
**Topics:** DataFrames, data display, formatting
- Load and display tabular data
- Format and style data presentation
- Work with pandas DataFrames
- Basic data aggregations

### 📖 Chapter 3: Interactive Filtering
**Topics:** Sidebar navigation, multiselect, filtering
- Create interactive sidebar controls
- Implement multi-select filtering
- Filter datasets based on user inputs
- Build responsive layouts with columns

### 📖 Chapter 4: Data Visualization
**Topics:** Charts, graphs, visual analytics
- Create meaningful visualizations
- Display metrics and KPIs
- Build comparative analysis views
- Implement interactive chart controls

### 📖 Chapter 5: Advanced Features
**Topics:** Caching, state management, complex interactions
- Optimize performance with st.cache_data
- Manage application state
- Build complex multi-filter dashboards
- Handle large datasets efficiently

## Dataset

The project includes `chai_sales.csv` containing sales data for various chai types across Indian cities:

**Columns:**
- `Date` - Transaction date
- `City` - City name (Delhi, Mumbai, Bangalore, etc.)
- `Chai_Type` - Type of chai (Masala, Adrak, Kesar, etc.)
- `Cups_Sold` - Number of cups sold
- `Revenue` - Revenue generated in rupees (₹)

**Sample Data:**
```
Date       | City      | Chai_Type | Cups_Sold | Revenue
2024-01-01 | Delhi     | Masala    | 120       | 1800
2024-01-01 | Mumbai    | Adrak     | 100       | 1500
2024-01-02 | Delhi     | Kesar     | 80        | 1600
2024-01-02 | Bangalore | Masala    | 90        | 1350
```

## Demo Dashboard Features

The `demo-dashboard.py` provides a complete example including:

- 📌 **KPI Metrics** - Total revenue, units sold, and averages
- 🎚️ **Dynamic Filters** - Region and product selection
- 📊 **Wide Layout** - Optimized for different screen sizes
- ⚡ **Performance** - Data caching for quick load times
- 💹 **Real-time Updates** - Instant dashboard refresh on filter changes

## Technologies Used

- **[uv](https://docs.astral.sh/uv/)** - Fast Python package installer and resolver
- **[Streamlit](https://streamlit.io/)** - Web framework for data apps
- **[Pandas](https://pandas.pydata.org/)** - Data manipulation and analysis
- **[NumPy](https://numpy.org/)** - Numerical computing
- **[OpenPyXL](https://openpyxl.readthedocs.io/)** - Excel file handling
- **Python** - Programming language

## Usage Tips

### Best Practices

1. **Always use virtual environments** to avoid dependency conflicts
2. **Enable caching** with `@st.cache_data` for frequently used data operations
3. **Organize filters in the sidebar** for better UX
4. **Use columns for layout** to create responsive designs
5. **Test thoroughly** with various data scenarios

### Performance Optimization

- Use `st.cache_data` for expensive computations
- Minimize re-renders by using session state
- Filter data at the source when possible
- Use appropriate chart types for your data

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the branch (`git push origin feature/AmazingFeature`)
6. Open a Pull Request

## Troubleshooting

### Port Already in Use
```bash
streamlit run app.py --server.port 8502
```

### Module Not Found
Ensure you've activated the virtual environment and installed all dependencies:
```bash
pip install -r requirements.txt
```

### Data File Not Found
Ensure `chai_sales.csv` is in the same directory as your script.

## Learning Resources

- [Streamlit Documentation](https://docs.streamlit.io/)
- [Streamlit Cheat Sheet](https://docs.streamlit.io/library/cheatsheet)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Python Documentation](https://docs.python.org/3/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Piyush Sarkar**
- GitHub: [@Piyush-Sarkar](https://github.com/Piyush-Sarkar)
- Email: [Your Email]

## Acknowledgments

- Inspired by Indian chai culture and e-commerce analytics
- Built with ❤️ for the Streamlit community
- Special thanks to all contributors and learners

## Changelog

### v0.1.0 (Initial Release)
- 5 progressive chapters covering Streamlit fundamentals
- Complete sales dashboard example
- Sample chai sales dataset
- Comprehensive documentation

---

**Happy Coding! Enjoy your Chai aur Streamlit journey! ☕📊**
