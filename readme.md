<h1 align="center">Data Pipeline With Databricks</h1>  
<h3 align="center">From API streaming data and CSV batch data to Star Schema and OBT models</h3>  

![Data Pipeline Diagram](https://raw.githubusercontent.com/jmcabreira/DataPipeline-DataBricks/main/Images/Captura%20de%20Tela%202024-12-01%20%C3%A0s%2006.14.01.png)
<h2 align="left">Steps:
</h2>  

- Load API Streaming data and csv bach data to delta tables in bronze zone 

- Build tables in Silver Zone 

	- tb_sales
	
	- tb_user
	
	- tb_calendar
	
	- tb_access
	
	- tb_courses

* Create two data models

	* Star Schema 
 
		* f_sales
  
		* dim_access
  
		* dim_calendar
  
		* dim_courses
  
		* dim_code
  
	* OBT (One Big Table)
 
		* Access OBT

<h3 align="left">Tools:</h3>

* DataBricks

* SparkSQL
  
* Python



<h3 align="left">Tips</h3>  

- We will use Spark Structured Streaming to treat streaming data as batch data, allowing us to process API data in the same way we handle batch data.

- **Structured Streaming in Spark** provides a high-level API for stream processing, which can be used to process both real-time (streaming) and historical (batch) data. By treating streaming data in micro-batches, you make it easier to apply batch-processing techniques to real-time data. This approach simplifies handling API data, enabling you to use the same pipeline and techniques for both data types.

  

