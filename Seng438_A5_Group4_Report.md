**SENG 438- Software Testing, Reliability, and Quality**


**Lab. Report \#5 – Software Reliability Assessment**


| Group \#:          | 4 |
|--------------------|---|
| Student Names:     |   |
| Alexander Sembrat  |   |
| Andrew Howe        |   |
| Jenna Vlaar        |   |
| Hajin Kim	         |   |


# Introduction


The objective of this lab is to learn to assess reliability and failure data using two different methods. The first method, Reliability Growth Testing will introduce us to systematically stressing a software system in order to identify flaws in the system. The other method we will cover is a Reliability Assessment using RDC, or a Reliability Demonstration Chart. RDC assessment will involve plotting failure data at certain time points in order to measure the Failure Intensity Objective or failure per natural units. 


# Assessment Using Reliability Growth Testing

We assessed the dataset ‘J1.DAT’ by converting the data into an excel file and inputting it into the C-SFRAT application. By comparing multiple models and comparing to the dataset, we determined that the model ‘S’ was the best fit for the data.  

### All Models
<img width="923" alt="All_models" src="https://user-images.githubusercontent.com/82128497/229909980-0ff7c26b-c11e-4ddd-accd-41134bceef4f.png">
<img width="929" alt="image" src="https://user-images.githubusercontent.com/82128497/229910515-0f826ce2-76ac-48b4-97d6-4497234c520e.png">

### Three Best Models
<img width="934" alt="image" src="https://user-images.githubusercontent.com/82128497/229908965-6563c4c0-1b49-4f3a-9f0d-a8d4271e39ac.png">
<img width="899" alt="image" src="https://user-images.githubusercontent.com/82128497/229910418-c27f4ba2-001e-4c2b-b0cb-51c5e00c9a6e.png">


# Excel Graphs For Growth Testing

We were unable to get the programs to generate graphs for intensity or reliability so they were made in excel instead.

### Insensity Over Time
<img width="314" alt="image" src="https://user-images.githubusercontent.com/82128497/229909506-e5f7b99c-c57c-4a63-9649-d71675e486a0.png">

### Time Between Failiures
<img width="308" alt="image" src="https://user-images.githubusercontent.com/82128497/229909239-6d67335f-2b3a-4f3d-985a-ace7bcb674c4.png">

### Reliability Over Time
<img width="313" alt="image" src="https://user-images.githubusercontent.com/82128497/229909374-86d2bf54-552a-476d-b4ab-a9d3b1c98dfe.png">

# Acceptable Range of Failure Rate for the Test Data
By looking at our failure intensity over time graph we can see that the insensity settles around 2 failures per second, this will be the top end of the range with 0 being the low end (0,2) per second. Any events where greater than 2 failures per second are occuring should be investigated as they are straying from the norm.

# Assessment Using Reliability Demonstration Chart

For the RDC, we used the dataset ‘Failure Data 3’. After inputting this data into the system, it was determined that all of the values fell between the acceptable range. 

### RDC Chart
<img width="316" alt="image" src="https://user-images.githubusercontent.com/82128497/229911319-33e8ce38-5b25-4e81-8ac9-d30d45d857f9.png">

### RDC Data
<img width="392" alt="image" src="https://user-images.githubusercontent.com/82128497/229911513-8a5e6be9-e3c2-489b-bb0f-4be3d1dd225b.png">

### Determining MTTF
For our MTTF we settled on 0.042 after some trail and error. This number was determined by dividing 1 failure by the count of total failiures in our data set (1/24). We found this yeilded good results that did not go far into the reject zone, no further guidance was provided on the best way to determine MTTF and our results were acceptable.

# Comparison of Results

Overall, growth testing is best for a product currently in use to gauge and predict reliability into the future where as RDC is used closer to the end of a product to see if the reliability goals were met. The results from using RDC would be more useful to look back into the past while the results from C-SFRAT are good to predict events in the future. Both results did yeild simmilar statistics and MTTF's so either method is acceptable.

# Discussion on Similarity and Differences of the Two Techniques

The two techniques both yielded a visual representation of the reliability of the system. Reliability growth testing utilized a model to represent the reliability of the system and was able to predict future values because of this. The reliability demonstration chart utilized a sort of classification system where values are either accepted, rejected or should be tested further. Overall, both tools provide some insight into the reliability of the system through varying methods.

# How the team work/effort was divided and managed
Since it is required that all group members are well familiarized with both methods of testing, we decided to work simultaneously on exploring the new testing tools. All four of us downloaded and installed the testing tools and carried out the instructions. Once we finished, we discussed our results and combined our work together.


# Difficulties encountered, challenges overcome, and lessons learned

We had a lot of difficulty getting the tools to run on our systems as well as find a way to input the data into the system. We ended up manually creating our own files by using the data from the provided documents. From this, we managed to be able to test the reliability of the system and learn how to use C-SFRAT and SRTAT.

# Comments/feedback on the lab itself
Since there was no information provided on the version of Python or Java required for the tools, it was extremely difficult to download and install the test tools properly. SRTAT and C-SFRAT would both not open the test files provided. Even after converting to several different file formats, they would not open the files. If there was guidance on how to properly download and install these tools as well as specifically which datasets to input into the tools, this lab would have been completed significantly sooner. 

