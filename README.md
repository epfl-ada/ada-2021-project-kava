## Title:
Why did Brexit occur?

## Abstract:
The UK's withdrawal from the EU, known as Brexit, is one of the most significant events of the 21st century. It has changed the whole life to a greater or lesser degree of millions of people, with political, economic, and social consequences, among other things. Nevertheless, how could this happen?

In this study, we intend to clarify why Brexit has won over permanence in the EU, based on an analysis of quotations from the Quotebank dataset. The main objective is to provide the arguments used by those who support or oppose it during the period 2015-2020. To achieve this, the project first classifies citations in favor or against Brexit and then analyses the main arguments for each group. Finally, the data is supplemented with the information of the speakers, and the opinions are examined over time.

## Research Questions:
A list of research questions you would like to address during the project:
- Which percentage of the speakers supported or was against Brexit?
- What arguments did the members of each category use to support their beliefs? (i.e., “historical reasons” or “immigration” in favor; i.e., “economy” or “travel” against).
- Who were the main supporters of each of the categories? Analyze them according to age, nationality, gender, occupation, place of residence.  
- How did the opinion towards Brexit change during the 5 year span? Did the arguments of each group also change?*

## Proposed additional datasets (if any):
- Wikidata: open and free knowledge base that collects structured data to provide support to services such as Wikipedia. The repository contains mainly items, and each of them has a unique item identifier (QID). Quotebank (out main dataset), also contains this unique identifier (QID) for each of the speakers, so the connection between both datasets can be made easily through this common identifier. Specifically, the project is using the speaker_attributes.parquet dataset provided by the professors, which contains ~9M unique Wikidata entities. Each entity has the following information: id, aliases, date_of_birth, nationality, gender, lastrevid, ethnic_group, US_congress_bio_ID, occupation, party, academic_degree, label, candidacy, type, and religion, each identified by a QID. The dataset is loaded as a Pandas dataframe using the read_parquet function (using PyArrow). Then, the wikidata_labels_descriptions_quotebank.csv is used in order to map each QID with its value.

## Methods:
¿Mathematical methods?

## Organization within the team:
- [Alvaro] Introduction of the project (README, context, project idea, project motivation, feasibility)
- [Kamil] Load Quotebank and Wikidata datasets. First cleaning data.
- [Alicia] Clean data (identify valid speakers and quotes).
- [Victor] 

## Proposed timeline:
1.  Definition of project description, goals, and feasibility.
2.  Load the data (Quotebank and Wikidata datasets) and merge datasets.
3.  Collect all possible quotations related to the subject of Brexit.
4.  Identify and filter which quotes are valid for our analysis.
5.  Examine and clean the data (generic and NLP cleaning)
6.  Categorize the opinions of speakers supporting or opposing Brexit.
7.  Find other terms that appear in quotations, get commonalities for those who are in favor (i.e., "historical reasons" or "immigration") and against (i.e., "economy" or "travel"). These terms will be possible arguments for why speakers support or not Brexit.
8.  Enrich the data with Wikidata (additional dataset), linking speakers’ quotes with more information (age, nationality, gender, profession...). This information could be used to enrich the analysis (i.e., show the opinion and the arguments of the speakers on a map depending on their birthplace).
9.  Explore and visualize the data.
10.  Model and interpret data, draw conclusions and address key project issues.
11.  Add the time variable in the analysis, studying the change in the opinion and arguments of the speakers during the time, and especially due to important events related to Brexit.*
13.  Storytelling and communication.
14.  Final conclusions (summary, results, and probelems encountered during the project).

## Questions for TAs (optional):
- What kind of problems can we expect?
- Is it feasible in our project to show the changes in the opinions and arguments of the speakers during time?

## Additional notes:
*This point will be subsequently evaluated as the project progresses.
