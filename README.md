# Search-Engine
Real time search engine using Node.js, Vue.js and ElasticSearch

## Getting Started

- Clone this repository
```
git clone https://github.com/renaissancenerd/Search-Engine.git
```
- Install the required libraries
```
npm install 
```
You will need to install ElasticSearch itself. There are different ways to install Elastic search. If you are using a debian linux operating system, you could just download the ```.deb```file and install using ```dpkg```.
```
//download the deb package
curl -L -O https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-5.6.4.deb
//install the deb package using dpkg
sudo dpkg -i elasticsearch-5.6.4.deb
```
Elasticsearch can be started and stopped using the service command:
```
sudo -i service elasticsearch start
sudo -i service elasticsearch stop
```
To configure Elasticsearch to start automatically when the system boots up, run the following commands:
```
sudo /bin/systemctl daemon-reload
sudo /bin/systemctl enable elasticsearch.service
```
After running the above command, Elasticsearch can be started and stopped as follows:
```
sudo systemctl start elasticsearch.service
sudo systemctl stop elasticsearch.service
```
To check the status of Elasticsearch:
```
sudo service elasticsearch status
```
## Test the Demo

- Serve the app
```
node index.js
```
- test the server side search at ```http://localhost:3001/```
- test the client side search at ```http://localhost:3001/v2```
