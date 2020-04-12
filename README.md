# Kode - Kallas


  

## Modules

|Name  | Progress |
|--|--|
|  Github-Crawler| In-Progress|
| Github-Analyser|In-Progress|
|Dashboard-backend||
|Dashboard-Frontend||


    Github-Crawler Setup

 1) Install and keep following software
 

 - Docker
 - Python-Flask
 - Python3
 - ElasticSearch
 - 

2) Run Below Comands after starting Docker

		docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.5.2
	```
	docker run -d --name kibana --net somenetwork -p 5601:5601 kibana:tag
	```
3) Set-up ElasticSearch (Important)
   navigate to [http://localhost:5601/app/kibana#/dev_tools/console?_g=()](http://localhost:5601/app/kibana#/dev_tools/console?_g=())
   copy and past each and every file from **github-crawler/Templates_commands** into above console (list of files is given below)

         * comments_command.txt
         * repos_cammand.txt
         * put_org_index.txt
    

3) Starting github-crawler and usage

		git clone https://github.com/CUBigDataClass/Kode-Kallas.git
		cd Kode-Kallas/github-crawler
	    python3 app.py
navigate to
-  http://127.0.0.1:5000  -- you will be able to see proper message
- http://127.0.0.1:5000/org/<!orgname_should be added here>  - Just check server logs  

4) Below some Documentation

		 Work Under progress

|**Module**  | **Usage** | **Requirements**|
|--|--|--|
|Github-Crawler|Used to get Github organization info |Docker and Python3|
