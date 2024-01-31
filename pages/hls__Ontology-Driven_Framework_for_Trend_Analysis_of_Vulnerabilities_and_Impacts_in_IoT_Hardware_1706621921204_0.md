file:: [Ontology-Driven_Framework_for_Trend_Analysis_of_Vulnerabilities_and_Impacts_in_IoT_Hardware_1706621921204_0.pdf](../assets/Ontology-Driven_Framework_for_Trend_Analysis_of_Vulnerabilities_and_Impacts_in_IoT_Hardware_1706621921204_0.pdf)
file-path:: ../assets/Ontology-Driven_Framework_for_Trend_Analysis_of_Vulnerabilities_and_Impacts_in_IoT_Hardware_1706621921204_0.pdf

- Thus, herein, we focus on IoT hardware vulnerabilities and develop an Ontology-driven Storytelling Framework (OSF) which aims to identify similar patterns of vulnerabilities over time, to help mitigate the impacts of vulnerabilities or predict and prevent future vulnerabilities.
  ls-type:: annotation
  hl-page:: 1
  hl-color:: blue
  id:: 65b8fbfb-b180-47d8-a8a8-16022821868c
- Most of the emerging vulnerabilities and exposures within IoT systems are due to incomplete or outdated software applications and hardware systems.
  ls-type:: annotation
  hl-page:: 1
  hl-color:: blue
  id:: 65b8fc46-ed8b-4909-81fe-29c907a03300
- Authors in [9] propose a classiﬁcation of device-related hardware vulnerability data for IoT and Industrial IoT equipment. In [9], authors divide the CVE records from NVD database into 7 distinct categories based on market and scope of IoT applications and the database samples were handclassiﬁed by authors based on expert knowledge. After handclassiﬁcation, authors utilize a Support Vector Machine (SVM) classiﬁer on device and vulnerability data to predict and mitigate threats resulting from vulnerabilities. 
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65b8fc83-7d0d-458f-8624-82965fb739d7
- All prior works have chosen the software vulnerabilities as the focus of their study and most prior works despite their valuable effort, fail to provide a storytelling framework that can ﬁnd useful information on the relationship and trends within the CVE and CWE datasets and offer detailed insight as to how a vulnerability and impacts have evolved over time.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65b8fcb7-9fe9-4412-abe6-80b279182707
- We link each CVE to a CWE and calculate the similarity metric of the input description and each CVE description using‘cosine similarity’ between each vector to identify the most relevant topics to the input.
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65b8fd03-70ef-4dab-91ea-3d294fc6e125
- .We consider the following question for our case-study, What kind of possible Attack Impacts can a victim system experience for a particular vulnerability that links to a speciﬁc CWE-ID (hardware weakness)?
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65b8fd22-6a0e-46fc-b9a3-a6a152cd944a
- To validate our proposed OSF, we use “spooﬁng of log data” as the user input to the GUI for an observable vulnerability we are facing. The GUI starts making connections among instances of CVE that are available in our corpus. Then the GUI cleans the string and calculates the relevance among the vulnerabilities using a similarity function such as cosine distance and rank the closest match found from our database.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65b8fd4b-3add-4f4e-9137-cae9dd3d283d