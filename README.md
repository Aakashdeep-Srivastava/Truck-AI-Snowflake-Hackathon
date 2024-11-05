## 🚚 AI for Good Hackathon: Improving Truck Drivers' Lives in India 🇮🇳

This project tackles the **1st AI for Good Hackathon - Infrastructure Theme**, focusing on improving the lives of truck drivers in India. We aim to use cutting-edge AI to analyze relevant data and generate actionable insights, ultimately leading to better working conditions and safer environments for these vital workers. 

### 💪 Our Mission

We believe that by leveraging the power of AI, we can contribute to a more sustainable and equitable future for truck drivers in India.  Our goals include:

* **Uncovering Hidden Challenges:**  Analyzing data to understand the specific difficulties faced by truck drivers, such as low wages, fatigue, and safety hazards.
* **Generating Data-Driven Solutions:**  Developing actionable recommendations based on our analysis, focusing on areas like improving fleet efficiency, promoting driver safety, and advocating for better work-life balance. 
* **Building a User-Friendly Platform:**  Creating an engaging Streamlit app to visualize key insights, share recommendations, and ultimately empower stakeholders to make positive changes.

### 🚀 The Tech Behind It

This project leverages a robust technology stack to achieve its goals:

* **Frontend (Streamlit):**  [https://streamlit.io/](https://streamlit.io/) provides a framework for building interactive dashboards and user interfaces.
* **Backend (Snowflake):**  [https://www.snowflake.com/](https://www.snowflake.com/)  serves as our data warehouse, providing secure storage, powerful SQL capabilities, and advanced analytical tools.
* **Data Sources:** We are using a combination of publicly available datasets from Open Government Data Platform India and specific datasets provided by the hackathon organizers. 

### 🏗️ Architecture Flow

```mermaid
flowchart TB
    subgraph Frontend
        direction LR
        f1[Streamlit]
        f2[Plotly]
        f3[Gradio]
    end

    subgraph Backend
        direction LR
        b1[AWS EC2]
        b2[Snowflake Connector]
        b3[Snowflake Data Warehouse]
        b4[Snowflake Secure Views]
        b5[Snowflake Data Pipelines]
        b6[Snowflake Analytical Functions]
        b7[Snowflake AI/ML Integration]
        b8[Snowflake Prediction Services]
    end

    f1 <--> b1
    f2 <--> b6
    f3 <--> b7

    b1 <--> b2
    b2 <--> b3
    b3 --> b4
    b3 --> b5
    b3 --> b6
    b3 --> b7
    b3 --> b8
