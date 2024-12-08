# Ques2

### Question 1

#### Q1(a)
**Given the brief to design a system for a data collection task, list three (3) important questions you would ask your client and suggest a type of database system to use, giving a reason for your choice.**   
“We are collecting data to use for a marketing campaign by DCU to increase
public transport use when travelling to campus. Data sources include public
surveys, records from Transport Ireland and information from DCU estates.”

1. What specific data attributes need to be collected from the surveys, Transport Ireland records, and DCU estates?
2. How frequently will the data be updated or accessed?
3. What is the expected volume of data, and will it require scalability?

**Suggested Database System:** A relational database system like PostgreSQL is recommended if the data is structured and requires complex querying. Alternatively, a non-relational database like MongoDB could be used if the data is semi-structured or unstructured (e.g., GPS logs) because it handles flexibility in schema well.

---

#### Q1(b)
**(i) Why is it useful to categorise data?**

Categorising data helps in organizing it systematically, making it easier to analyze, retrieve, and derive insights. It also improves efficiency in data processing and ensures consistency.

**(ii) Identify some different category descriptions for the following pieces of data:**
- **A. Athlete profile:** Name, age, gender, nationality.
- **B. List of races:** Race type (sprint/marathon), date, location.
- **C. Gold, Silver, and Bronze winners:** Medal type, athlete name, event.
- **D. Times of the winners from the sprint races:** Time in seconds, athlete name, race ID.

---

#### Q1(c)
**Give two (2) advantages & two (2) disadvantages of non-relational databases and give an example of when a non-relational database would be useful.**

**Advantages:**
1. Flexible schema allows for handling semi-structured or unstructured data.
2. High scalability for large datasets.

**Disadvantages:**
1. Limited support for complex queries compared to relational databases.
2. Potentially inconsistent data due to lack of strong ACID compliance.

**Example Use Case:** A non-relational database like MongoDB would be useful for storing GPS logs from Transport Ireland due to its flexibility in handling semi-structured data.

---

#### Q1(d)
**Describe activities at each stage of a generic data analytics pipeline:**
1. **Gathering:** Collecting raw data from various sources like surveys or sensors.
2. **Processing:** Cleaning and transforming raw data into usable formats.
3. **Analysing:** Applying statistical methods or machine learning models to extract insights.
4. **Presenting:** Visualizing results using charts or dashboards for stakeholders.
5. **Preserving:** Archiving processed datasets for future reference or compliance.

---

### Question 2

#### Q2(a)
**(i) What is metadata?**

Metadata is data that provides information about other data, such as its structure, origin, or purpose.

**(ii) Name three (3) things that metadata is used for:**
1. Data organization and retrieval.
2. Ensuring interoperability between systems.
3. Tracking the provenance of datasets.

**(iii) Examples of different types of metadata:**
- Descriptive metadata: Title, author.
- Structural metadata: File format details.
- Administrative metadata: Access rights or creation date.

---

#### Q2(b)
Give simple example metadata describing the module CA682. Why would a standard
be useful for this type of metadata and identify one (1) problem with enforcing a
standard.
**Simple example metadata describing module CA682:**
- Title: Data Management and Visualisation
- Code: CA682
- Year: 2018/2019

**Why would a standard be useful for this type of metadata?**
Standards ensure consistency and interoperability across systems.

**Problem with enforcing a standard:** It may limit flexibility in capturing unique attributes specific to certain datasets.

---

#### Q2(c)
Big data is characterised by its Volume, Velocity, Variety and recently Veracity.
Veracity refers to how reliable the data is.
**(i) Why does big data have particular issues with uncertainty?**
Big data often comes from diverse sources with varying levels of reliability and accuracy, making it harder to ensure consistency and trustworthiness.

**(ii) Method for checking veracity:** Cross-referencing with trusted datasets or using statistical validation techniques.

---

#### Q2(d)
**Describe the process of scraping data from a website:**
Scraping involves extracting information from web pages by parsing HTML content using tools like BeautifulSoup or Selenium.

**Two rules to remember when scraping:**
1. Adhere to the website's terms of service.
2. Avoid overloading servers by limiting request rates.

---

### Question 3

#### Q3(a)
You are collecting data to for a marketing campaign to increase public transport use
to travel to DCU. You have the following data sources:
A. Survey of current transport patterns of staff and students.
B. Access logs from Transport Ireland app filtered by GPS location for the
Glasnevin Campus.
C. Map of transport options for the DCU campuses.
D. Medical research data showing improved heart health from regular walking
based on user’s wearing fitbit sensors.
For each of these sources, identify one (1) possible cause and consequence of poor
quality data.
ANSWERS******
**Identify one possible cause and consequence of poor quality data for each source:**
- **Survey:** Cause - Biased responses; Consequence - Misleading insights.
- **Access logs:** Cause - Missing GPS entries; Consequence - Incomplete analysis.
- **Map:** Cause - Outdated information; Consequence - Incorrect routing recommendations.
- **Medical research data:** Cause - Sensor inaccuracies; Consequence - Invalid health conclusions.

---

#### Q3(b)
**Pick one source (Survey):**
(i) Approach to clean data: Remove incomplete or inconsistent responses using validation rules.
(ii) Enforce better quality: Design surveys with mandatory fields and real-time error checks.

---

#### Q3(c)
(i) What are constraints with respect to Data Quality? Ensure you define and
distinguish between static and dynamic constraints.
(ii) What are two (2) potential problems with enforcing constraints to improve data
quality?

Answers**(i) Constraints with respect to Data Quality:**
Constraints are rules applied to ensure valid and consistent data:
- Static constraints: Fixed rules like unique IDs or specific formats.
- Dynamic constraints: Rules that depend on context or time (e.g., valid date ranges).

**(ii) Two problems with enforcing constraints:**
1. Over-restrictiveness may reject valid but unusual entries.
2. Increased complexity in implementation.

---

#### Q3(d)
**Two potential problems with open datasets:**
1. Privacy concerns if sensitive information is not anonymized properly.
2. Risk of misuse or misinterpretation by unqualified users.

---

### Question 4

#### Q4(a)
Given the following visualisation tasks, suggest an appropriate graph type (specific
chart type not just the category) for each to display the information and give a brief
justification.
A. Summary of voter choices in the Irish Election 2016
B. Annual income for Computer Science students grouped by university
C. Population trend for Ireland over the last decade
D. Average rental prices for each Irish County in 2016

ANSWERS**Suggest appropriate graph types for each task:**
- **A:** Bar chart – Clearly shows voter choice distribution.
- **B:** Box plot – Displays income distribution grouped by university effectively.
- **C:** Line chart – Best for showing population trends over time.
- **D:** Heat map – Highlights average rental prices geographically by county.

---

#### Q4(b) In the appendix, Figure 1 shows a graph. Identify three (3) problems with the design
and suggest a better method for showing the information, giving a specific chart type
that could be used. You do not need to view the appendix in colour.**

Answers**
**Three problems with Figure 1 (3D pie-chart):**
1. Difficult to compare segment sizes accurately due to perspective distortion.
2. Overuse of 3D effects makes it visually cluttered.
3. Lack of clear labels or legends reduces interpretability.

**Better method:** Use a 2D bar chart for precise comparison of proportions.

---

#### Q4(c)
**What is D3.js?**

D3.js is a JavaScript library used for creating dynamic and interactive visualizations based on web standards like SVG, HTML5, and CSS.

**Two things D3.js does not do:**
1. Provide pre-built chart templates.
2. Handle raw data cleaning directly.

**Difference between rules and selectors in CSS (used in D3.js):**
Selectors target specific elements in the DOM (e.g., `.class`), while rules define styling properties applied to those elements (e.g., `color`).

---

#### Q4(d)
**How can design rules improve visualizations?**
Design rules ensure clarity and usability by guiding layout choices (e.g., avoiding clutter). Example: Using consistent color schemes enhances readability.

---

### Question 5

#### Q5(a)
**Visual communication goals evident in Figure 2:**
1. Raising awareness about unhealthy diets among children.
2. Encouraging action through impactful imagery and statistics.

**Two design principles applied:**
1. Contrast – Bold text highlights key messages effectively.
2. Alignment – Structured layout directs attention logically across elements.

---

#### Q5(b)
**Two gestalt principles used in Figure 2:**
1. Proximity – Related items are grouped together for coherence (e.g., statistics near visuals).
2. Continuity – Flowing layout guides the viewer's eye naturally through content.

---

#### Q5(c)
**What is a pre-attentive feature?**
A pre-attentive feature is a visual property (e.g., color or shape) that humans can detect quickly without focused attention.

**Experiment example:** Show participants grids with varying shapes/colors; measure response time to identify anomalies like a red square among blue ones.

---

#### Depth cues matching:
| Cue                  | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Occlusion            | D. Blocking of more distant objects by closer objects                     |
| Convergence          | B. Difference in direction of our eyes when looking at closer objects      |
| Accommodation        | F. Muscle tension from re-focusing the eye                                 |
| Aerial Haze          | E. Objects on the far horizon look hazy due to particles in the air        |
| Binocular Disparity  | C. Images sensed by our two eyes are slightly different                    |
| Motion Parallax      | A. Moving the head slightly creates differences in sensed images           |

The cue mostly used for creating 3D effects in movies is **Binocular Disparity** because it mimics how our two eyes perceive depth differently based on their positions relative to objects.


![image](https://github.com/user-attachments/assets/2c727d19-d5cd-4b00-b32c-f237b6a53c49)
![image](https://github.com/user-attachments/assets/9577242b-dcd5-4300-b491-c09b8ab38a28)



