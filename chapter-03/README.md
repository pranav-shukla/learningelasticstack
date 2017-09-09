# Import product data into Elasticsearch

1. Download the latest 5.x version of logstash for your operating system from https://www.elastic.co/downloads/logstash
2. Extract logstash on your system.
3. Copy the <b>files</b> directory in your logstash home folder. If logstash was installed at /usr/share/logstash, after copying the files, the structure of files should look like -

```shell
/usr/share/logstash/files/products.csv
/usr/share/logstash/files/logstash_products.conf
```

4. Make sure that the logstash_products.conf file has the correct absolute path of products.csv file on your system.
5. Ensure that the index amazon_products is created as per the instructions given in chapter 3.
6. Run logstash from command line, using the following commands

```shell
cd /usr/share/logstash
bin/logstash -f files/logstash_products.conf
```

