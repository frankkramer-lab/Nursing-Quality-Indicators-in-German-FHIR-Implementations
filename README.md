# Evaluation of the Availability of Nursing Quality Indicators in German FHIR Implementations

***Steffen NETZBAND, Katharina OTT, Florian AUER and Frank KRAMER***

*IT-Infrastructure for Translational Medical Research, University of Augsburg, Germany*



## Abstract
Standardized nursing data sets facilitate data analysis and help to improve nursing research and quality management in Germany. Recently, governmental standardization approaches have favored the FHIR standard and helped to define it as the state of the art for healthcare interoperability and data exchange. In this study, we identify common data elements used for nursing quality research purposes by analyzing nursing quality data sets and databases. We then compare the results with current FHIR implementations in Germany to find most relevant data fields and overlaps. Our results show that most of the patient focused information has already been modelled in national standardization efforts and FHIR implementations. However, representation of data fields describing nursing staff related information, such as experience, workload or satisfaction, is missing or lacking.
Keywords. FHIR, interoperability, nursing informatics, nursing quality indicators

## Supplementary

### Frequency of nursing indicators in common nursing quality databases and initiatives:

|Indicator | [Stewig et al.](https://jasmin.goeg.at/214/1/Pflege-Ergebnisqualit%C3%A4t.pdf)  | [NDNQI](https://search.ebscohost.com/login.aspx?direct=true&profile=ehost&scope=site&authtype=crawler&jrnl=10913734&AN=29434370&h=ThRHzN3vAbxS1rogj3C%2FehousCwcmyDCddiRwuwrw3hWCvtBgpCGgreyZmLM2P9Hy6ANsM9eHEf4VhgcEg%2FwRA%3D%3D&crl=c) | [CalNOC](https://www.ncbi.nlm.nih.gov/books/NBK43614/?report=printable)  | [MilNOD](https://sigmapubs.onlinelibrary.wiley.com/doi/full/10.1111/j.1547-5069.2010.01364.x) | [NQF](https://www.qualityforum.org/Publications/2004/10/National_Voluntary_Consensus_Standards_for_Nursing-Sensitive_Care__An_Initial_Performance_Measure_Set.aspx) | [VANOD](https://d1wqtxts1xzle7.cloudfront.net/52702059/Towards_a_national_report_card_in_nursin20170419-3216-j8happ-libre.pdf?1492634921=&response-content-disposition=inline%3B+filename%3DTowards_a_National_Report_Card_in_Nursin.pdf&Expires=1679323829&Signature=eFJkNfIogWAQ4T5kudEshT7OkFg3E~145FD70vt~CaWX6vDrn9fHH7HixxtslDJ-3wxQ5bzEVEe6dWj8isyV4waokUC8APtGzTeubdY~cbRcnd9F8H5C1etFVk6XaO1LusfzJCxq7VnpH6jJ2nHzD7Mj9sdAI~qJZPbu6-oPB2QWjfZjBlUUtPi2WEff8-1WKgmdEnGOVD3uI2FRVMQ~xY9aRsRb7Lv5qX~BXeysyLf5wfi0iXr1SZm~l-G2rmHYiDxbfk6ZjWOoE~QHVO~67mStc5MGRcyBK7IcCj0mWNizCXgF0v4-h0G-QZCXpgqqO~1IbslChG9tPQAyMS2v~w__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA) | [CMS](https://f.hubspotusercontent30.net/hubfs/56632/MDS-3_0-QM-USERS-MANUAL-v14_0.pdf) | [C-HOBIC](https://doi.org/10.1197/jamia.M2974) | [C-NNQR](https://doi.org/10.1097/NCQ.0000000000000122) | [Switzerland Art. 59a KVG](https://search.ebscohost.com/login.aspx?direct=true&profile=ehost&scope=site&authtype=crawler&jrnl=09486704&AN=140064840&h=HHXkRFhzjPVz3H9NIdp4uTpX3gESZOETlupUXHQS0SF5sEyM8JwhXhzlH3gxMHM%2BuGNMfn1dvtX9WGSoBtPMsQ%3D%3D&crl=c) | [Wingenfeld et al.](https://www.institut-fernblick.de/wp-content/uploads/2019/01/20180903_Entwicklungsauftrag_station%C3%A4r_Abschlussbericht.pdf)  | Total|
|--------- | -------------- | ----- | ------- | ------ | --- | ----- | --- | ------- | ------ | ------------------------ | ------------------ | -----|
|Pressure Ulcer | x | x | x | x | x | x | x | x | x | x | x | 11|
|Falls | x | x | x | x | x | x | x | x | x |  | x | 10|
|Use of Restraints | x | x |  | x | x |  | x |  | x | x | x | 8|
|Nursing hours |  | x | x | x | x | x |  |  | x |  |  | 6|
|Pain | x |  |  |  |  |  |  | x | x | x | x | 5|
|Staff/Skill mix |  | x | x | x | x | x |  |  |  |  |  | 5|
|Nurse Turnover |  | x | x |  | x | x |  |  | x |  |  | 5|
|Malnutrition/Loss of weight | x |  |  |  |  |  | x |  |  | x | x | 4|
|Instrumental activities of daily living and self-care  | x |  |  |  |  |  | x | x |  |  | x | 4|
|Staff experience, knowledge, skills, expertise |  | x | x | x |  | x |  |  |  |  |  | 4|
|Satisfaction with (nursing) care | x |  |  | x |  | x |  |  |  |  |  | 3|
|Staff satisfaction and well-being |  | x |  | x |  | x |  |  |  |  |  | 3|
|HCAI – Urinary Catheter associated Infection |  | x |  |  | x |  | x |  |  |  |  | 3|
|Medication administration errors | x |  |  | x |  |  |  |  |  |  |  | 2|
|HCAI – Bloodstream |  | x |  |  | x |  |  |  |  |  |  | 2|
|HCAI – Pneumonia |  | x |  |  | x |  |  |  |  |  |  | 2|
|Practice Environment |  |  |  | x | x |  |  |  |  |  |  | 2|
|Mobility |  |  |  |  |  |  | x |  |  |  | x | 2|
|Incontinence |  |  |  |  |  |  | x | x |  |  |  | 2|
|Assessment of Pressure Ulcer |  |  | x |  |  |  |  |  | x |  |  | 2|
|Pain Assessment/Intervention/Reassessment (AIR) |  | x |  |  |  |  |  |  |  |  |  | 1|
|Psychiatric Physical/Sexual Assault Rate |  | x |  |  |  |  |  |  |  |  |  | 1|
|Nurse Vacancy |  | x |  |  |  |  |  |  |  |  |  | 1|
|Nursing self-harm |  |  |  | x |  |  |  |  |  |  |  | 1|
|Patient turnover |  |  |  | x |  |  |  |  |  |  |  | 1|
|Patient acuity |  |  |  | x |  |  |  |  |  |  |  | 1|
|Failure to rescure |  |  |  |  | x |  |  |  |  |  |  | 1|
|Smoking advice |  |  |  |  | x |  |  |  |  |  |  | 1|
|Nursing hours per outpatient encounter |  |  |  |  |  | x |  |  |  |  |  | 1|
|Nursing Staff injuries |  |  |  |  |  | x |  |  |  |  |  | 1|
|Vaccination Rate |  |  |  |  |  |  | x |  |  |  |  | 1|
|Use of antipsychotic medication |  |  |  |  |  |  | x |  |  |  |  | 1|
|Use of indwelling catheter |  |  |  |  |  |  | x |  |  |  |  | 1|
|Patiens with depressive symptoms |  |  |  |  |  |  | x |  |  |  |  | 1|
|residents who have behavior symptoms affecting others  |  |  |  |  |  |  | x |  |  |  |  | 1|
|Paid sick leave of nurses |  |  |  |  |  |  |  |  | x |  |  | 1|
|Assessment of fall risk |  |  |  |  |  |  |  |  | x |  |  | 1|
|Aggressive Behaviour (ABS-Score) |  |  |  |  |  |  |  |  | x |  |  | 1|
|Polymedication |  |  |  |  |  |  |  |  |  | x |  | 1|
|Integration Interview |  |  |  |  |  |  |  |  |  |  | x | 1|
|Nurse-to-Patient Ratio |  |  | x |  |  |  |  |  |  |  |  | 1|
|Contract staff use |  |  | x |  |  |  |  |  |  |  |  | 1|
|Workload |  |  | x |  |  |  |  |  |  |  |  | 1|
|Sitter hours |  |  | x |  |  |  |  |  |  |  |  | 1|
|Risk assessment |  |  | x |  |  |  |  |  |  |  |  | 1|
