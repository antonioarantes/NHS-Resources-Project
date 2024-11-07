# NHS Resource Allocation & Capacity Analysis Project

This project involved analyzing National Health Service (NHS) data to assess resource utilization, staff capacity, and missed appointment rates across regions. Insights gained through this analysis will help the NHS optimize resource allocation, improve operational efficiency, and reduce costs associated with missed appointments.

## Project Overview

The NHS faces increasing pressure to balance healthcare service demands with limited resources. To support the NHS in making informed decisions on resource allocation and potential infrastructure expansion, this analysis focused on:
1. **Service Utilization**: Evaluating appointment volume trends and utilization patterns.
2. **Missed Appointments**: Identifying factors influencing missed appointments to reduce associated costs.
3. **Staff Capacity**: Assessing doctor workload and regional disparities to inform equitable resource distribution.

Data from internal NHS sources and external public datasets provided a foundation for understanding regional differences, workforce burden, and patient engagement trends.

## Analytical Approach

### Data Preparation and Cleaning
Five datasets were used in this project:
- **actual_duration (AD)** and **national_categories (NC)**: Clean, unduplicated datasets with unique row combinations.
- **appointments_regional (AR)**: Required deduplication of 21,604 rows, aggregating appointments for accurate analysis.
- **nhs_regions** and **nhs_staff**: External datasets providing regional and doctor information for added context.

Key preparation steps included:
- Handling duplicated rows in AR and converting date columns to appropriate data types.
- Retaining high-variance values for outlier analysis.
- Addressing data inconsistencies, such as mismatched appointment counts across datasets.

### Analytical Techniques
The following analyses were conducted to meet the project’s objectives:

- **Time Series Analysis**: Assessed seasonal patterns in appointment counts.
- **Regional Analysis**: Compared appointments and missed appointments across regions.
- **Staff Capacity Analysis**: Created a “appointments per doctor” metric to evaluate regional and overall doctor workloads.
- **Missed Appointment Analysis**: Examined correlations between missed appointments, booking lead times, and appointment type.

In addition, I performed **social media analysis** using Twitter data to understand public sentiment and engage NHS stakeholders in a sentiment analysis project.

## Visualizations and Notebook Structure

The Jupyter notebook is organized for easy navigation and consistent branding using NHS color schemes. Key components include:
- **Univariate Analysis**: Frequency and distribution graphs of categorical data.
- **Time-based Analysis**: Visualization of changes in service utilization over time.
- **Regional and Staff Analysis**: Graphs comparing regional appointment rates, missed appointment trends, and workload distribution.
- **Daily Capacity Analysis**: Comparisons of NHS capacity guidelines to actual appointment loads.

---

## Key Insights

### 1. Service Utilization
- **Seasonal Trends**: Uniform monthly appointment trends across regions, suggesting consistent service demand.
- **Overcapacity**: NHS consistently exceeds the maximum daily capacity guideline (1.2 million appointments), indicating the need for expanded resources or adjusted scheduling.

### 2. Staff Capacity & Workload
- **Decline in Doctors**: A 1.91% reduction in doctor numbers over seven months, increasing workload pressures.
- **Regional Disparities**: Significant differences in appointments per doctor by region (up to 169 per month), highlighting an uneven distribution of staff resources.

### 3. Missed Appointments
- **Missed Appointment Trends**: Increase in missed appointments, especially for those scheduled more than 28 days in advance.
- **Same-day Appointments**: Show lowest missed appointment rates (<2%), suggesting that reducing booking lead time may improve attendance rates.

## Future Recommendations
To optimize NHS resources and improve efficiency:
- **Explore Staffing and Resource Allocation**: Consider reassigning staff based on appointment volumes and regional demand.
- **Address Overcapacity**: Implement strategies to manage high appointment volumes on weekdays.
- **Improve Appointment Attendance**: Offer same-day or short-notice appointment slots to reduce missed appointments.
- **Incorporate Population Density Data**: Assess regional appointment needs relative to population for targeted resource planning.

This README provides an overview of the methodology, analyses, and insights. Refer to the notebook for detailed visualizations, code, and further recommendations.
