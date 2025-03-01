📊Student Result Management System
A comprehensive system for managing and analyzing student results using Python, PySpark, and Streamlit. This project handles data for 10,000 students across 6 subjects, providing detailed analytics and an interactive dashboard.

Dashboard Overview

🌟 Features
1. Data Generation & Management
Generates realistic data for 10,000 students
Creates profiles with student ID, name, age, and batch information
Generates marks for 6 core subjects with automatic grade assignment:
Electronics
Programming
Database
Data Science
Mathematics
DSA
Data Generation

2. Data Analysis (Using PySpark)
Statistical Analysis:

Overall performance metrics
Subject-wise analysis
Grade distribution
Pass/Fail statistics
Performance Metrics:

Average marks with standard deviation
Minimum and maximum marks
Pass percentages by subject
Subject-wise performance trends
Analysis Results

3. Interactive Dashboard
Student Search Features
Search by Student ID or Name
Comprehensive student profile view
Individual performance metrics
Color-coded grade visualization
Subject-wise performance charts
Student Search

Analytics Dashboard
Key Performance Indicators
Overall average marks
Pass rate with distinction percentage
Highest/lowest marks
Total entries and statistics
KPI Dashboard

Performance Analysis
Interactive subject-wise performance charts
Grade distribution pie charts
Detailed statistical tables
Pass/Fail analysis by subject
Performance Charts

🛠️ Technology Stack
Python 3.x
PySpark 3.5.4
Streamlit 1.42.2
Pandas 2.2.3
Plotly 6.0.0
Additional libraries:
Faker (for data generation)
Matplotlib (for visualization)
Seaborn (for statistical plots)
📋 Prerequisites
Python 3.x
Java Runtime Environment (for PySpark)
Required Python packages:
pip install -r requirements.txt
🚀 Installation & Setup
Clone the repository:
git clone https://github.com/ranjitla/student-result-management.git
cd student-result-management
Create required directories:
mkdir data
mkdir analysis_results
Install dependencies:
pip install -r requirements.txt
💻 Usage
Generate student data:
python data_generator.py
This will create:

students.csv (10,000 student profiles)
marks.csv (60,000 mark entries)
Run Spark analysis:
python spark_analysis.py
Generates analysis files:

overall_stats.csv
subject_stats.csv
grade_dist.csv
performance_metrics.csv
subject_performance.csv
Launch the dashboard:
streamlit run dashboard.py
📁 Project Structure
student-result-management/
├── data/                      # Data storage
│   ├── students.csv          # Student profiles
│   └── marks.csv            # Student marks
├── analysis_results/         # Analysis output
│   ├── overall_stats.csv
│   ├── subject_stats.csv
│   ├── grade_dist.csv
│   ├── performance_metrics.csv
│   └── subject_performance.csv
├── screenshots/              # Documentation images
├── src/
│   ├── data_generator.py    # Data generation script
│   ├── spark_analysis.py    # PySpark analysis
│   └── dashboard.py         # Streamlit dashboard
├── requirements.txt         # Dependencies
└── README.md               # Documentation
📊 Dashboard Guide
Student Search Tab
Enter student ID (e.g., STU00001) or name
View comprehensive student profile:
Personal information
Academic performance
Subject-wise marks
Performance visualization
Student Profile

Analysis Tab
Key Metrics View

Overall performance indicators
Quick statistics
Subject Analysis

Interactive performance charts
Detailed subject statistics
Grade Distribution

Visual grade distribution
Percentage breakdowns
Analysis Features

🔧 Customization
You can modify:

Number of students (data_generator.py):
def generate_student_profiles(num_students=10000):
Subject list (data_generator.py):
subjects = ['Electronics', 'Programming', 'Database', 
            'Data_Science', 'Mathematics', 'DSA']
Grade boundaries (data_generator.py):
'A+' if x >= 90 else
'A' if x >= 80 else
# ... etc
🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

👥 Authors
[Your Name]
[Other Contributors]
🙏 Acknowledgments
Built as part of the Data Engineering course project
Thanks to all contributors and testers
Special thanks to [Your Institution/Organization]
📞 Support
For support, please create an issue in the repository or contact [your-email@example.com]
