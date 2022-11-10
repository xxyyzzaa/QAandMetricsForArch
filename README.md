# QualityMetricsInSoftwareArchitecture

To put into practice the results we found during our research and keep the results up-to-date we propose a Framework which generates informative and aggregated web views of the metrics, quality attributes, quality characteristics, and their relationships. The proposed framework has been implemented with MDE techniques and it is based on a metamodel which allows us to define the quality the quality characteristics, quality attributes and metrics to measure the quality attributes.



Based on this framework we have implemented a Domain Specific Language (DSL) with xText allowing the textual definition for our quality repository. Indeed, this DSL is based on a grammar (derived from the metamodel), allowing software architects, practitioners, and researchers to define quality aspects and their relationships. Moreover, we have integrated rules inspired by the Bibtex grammar {https://slebok.github.io/zoo/markup/textual/bibtex/bibtex/hillairet/extracted/index.html} to allow contributors to directly work with bibtex entries in the DSL, to define research contributions. By using this DSL, contributors can define their own quality attributes and metrics and/or refine those provided by us (we call to the file containing these definitions as quality definition file).

## Step by step guide to install the DSL

### Pre-requisite:

* You should have an Eclipse IDE installed on your machine (in case you don’t have it download and install it from https://www.eclipse.org/downloads/ ).

* Install and Configure a web-server (e.g., MAMP). This web server will allows you to get a visual preview of the generated graph which is composed of quality characteristics, attributes and metrics.


### Steps:
* Download and install the xText plugin install the xtext plug-in into a running Eclipse.
  * Step 1) Eclipse Help > Eclipse Marketplace
  * Step 2) Install the plugin “Eclipse xText"
  * Step 3) Restart Eclipse
Please refer to this link https://www.eclipse.org/Xtext/download.html for  more instructions.

* Run the configuration (upon running the configuration Eclipse will automatically open another Eclipse window which means that you will have two Eclipse running).

<img src="[https://your-image-url.type](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/1.png)" width="250" height="250">

![This is an image](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/1.png =250x250)

* In another Eclipse window create a new project, specify a project name and specify the location where you want to save your project. Untick “User default Location” and set the path pointing to the path of your web server where your files are located. In this way everything you edit, it will be automatically updated on your web browser.
![This is an image](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/2.png =250x250)
![This is an image](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/3.png =250x250)


* Download the quality definition file called "repo.archquality" which is located in the “catalog” folder and paste it in the project you have created. The quality definition file is associated with the .archquality extension, which will make sure that the Eclipse editor recognizes the content of the model instantiation. By using the provided editor, all the developed features will be available, e.g., syntax highlighting, code completion, error quick fixes, etc. as can be seen in this screenshot.

![This is an image](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/4.png =250x250)


* Once everything is installed correctly, go to your browser then point to the address of your web-server and the generated graph similar to this one will be shown. 

![This is an image](https://github.com/xxyyzzaa/QAandMetricsForArch/blob/main/assets/5.png =250x250)


## How to contibute to this Framework

Following the process, a contributor who wants to define new quality attributes and/or metrics or new relationships discovered in his/her studies can create a branch of the repository, even if actually the only file needed is the .archquality definition (up-to-date in the catalog folder). Contributors can then add or edit existing definitions by exploiting the textual syntax. After that, contributor can emit a pull request that will be evaluated by the repository maintainer and in case the provided changes in definitions are legit and supported by the correct linked research contributions, a merge of the .archquality model will be executed. 




