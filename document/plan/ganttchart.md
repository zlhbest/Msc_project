## MSc project Plan
Based on the research work at https://github.com/yongsen/SignFi, the project is reproduced and machine learning related algorithms improve accuracy based on the project.
### Project parts
* Doing Research and prepare 
  * Learn about analysis and parsing CSI data using python or matlab **(2024-06-10 - 2024-06-16)**
  * Learn deep learning algorithms and try programming using matlab or python **(2024-06-17 - 2024-06-30)**
* Reproduce the SignFi project
  * Learn about the project **(2024-06-24 - 2024-07-03)**
  * Use this dataset to reproduce the project  **(2024-07-01 - 2024-07-28)**
  * Test the accuracy and precision of this project **(2024-07-24 - 2024-08-04)**
* Find suitable algorithms to improve accuracy   **(2024-08-01 - 2024-08-25)**
* Write documentation **(2024-06-24 - 2024-09-05)**


### Plan 

#### Official timetable
* Monday 10th June 2024 : Start date of project 
* Monday 24th June 2024 :  Project brief
* Monday 19th August 2024: Start date of demonstrations
* Thursday 5th September 2024 : Dissertation handin
* Monday 23rd September 2024 : MSc Project viva scheduled during the week of
* Last week of November 2024 : Projects results and feedback

#### Gantt chart

```Mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       Longhao Zhu Msc project
    tickInterval 1week
    weekday monday


    %%  until 10th june, i need to read 20 articles at least
    section Literature Review
    reading 20 articles and learn        :active,pre_task1, 2024-04-29,2024-06-10
    reading 2 articles          : active,read1, 2024-04-29,1w
    reading 3 articles          : read2, 2024-05-06,1w
    reading 3 articles          : read3,2024-05-13,1w
    reading 3 articles          : read3,2024-05-20,1w
    reading 3 articles          : read3,2024-05-27,1w
    Summarize learning content  : sum,2024-06-03,1w
    submit project plan         : milestone, m1, 2024-05-15,


    section Research
    start project         : milestone, m2, 2024-06-10,
    Data Acquisition and Preprocessing  : task1,2024-06-03,3w
    Model Selection and Design          : task2, after task1,2w
    Dataset Splitting and Training      : task3, 2024-07-01,3w
    Model Evaluation                    : task4, 2024-07-08,3w
    Results Interpretation and Analysis : task5, after task4,2w
    Start date of demonstrations        : milestone,m3,2024-08-19,
    Dissertation handin                 : milestone,m4,2024-09-05,

    section document
    write project plan : active, plan,2024-04-29,until m1
    make literature matrix: active,pre_task1, 2024-04-29,2024-06-10
    write report : report_task, 2024-06-24,2024-09-05
```