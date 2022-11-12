# Project - College Students Details
## Description
> JsonPowerDB is a Real-time, High Performance, Lightweight and Simple to Use, Rest API based Multi-mode DBMS. JsonPowerDB has ready to use API for Json document DB, RDBMS, Key-value DB, GeoSpatial DB and Time Series DB functionality. JPDB supports and advocates for true serverless and pluggable API development.
> It is basically a Database Server with Developer friendly REST API services.
> JPDB has ready to use API for Json document DB, RDBMS, Key-value DB, GeoSpatial DB and Time Series DB functionality. JPDB supports and advocates for true serverless and pluggable API development.

## Benifits of using JsonPowerDB
- It is realtime and simple to use.
- Easy to maintain the reconds.
- Serverless support - fast development - cuts time to market.
- Build using world's fastest indexing engine PowerIndex which gives unlimited data capacity, supporting unlimited indexes, realtime data processing which makes it fast and secure.
- Give developer friendly Webservices API which reduce the developement cost.
- Multiple Security Layers.
- Schema free - easy to maintain
- A single instance - Million Indexes
- Inbuilt support for querying multiple databases.
- It is light weight.
- It is a serverless database so that you don't have to choose an instance size at all.

## PUT Command
```
{
    "token": "-1935843913|3223940520357615501|-1935843909",
    "cmd": "PUT",
    "dbName": "Colors",
    "rel": "Color-Rel",
    "jsonStr": [
    {
      "color": "black",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,255,255,1],
        "hex": "#000"
      }
    },
    {
      "color": "white",
      "category": "value",
      "code": {
        "rgba": [0,0,0,1],
        "hex": "#FFF"
      }
    },
    {
      "color": "red",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,0,0,1],
        "hex": "#FF0"
      }
    },
    {
      "color": "blue",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [0,0,255,1],
        "hex": "#00F"
      }
    },
    {
      "color": "yellow",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,255,0,1],
        "hex": "#FF0"
      }
    },
    {
      "color": "green",
      "category": "hue",
      "type": "secondary",
      "code": {
        "rgba": [0,255,0,1],
        "hex": "#0F0"
      }
    },
  ]
}
```
##### output
```
{"data":"{\"rec_no\":[7,8,9,10,11,12]}","additionalData":{"processReqType":0,"dbUpdateFlag":true},"message":"DATA INSERTED, Total 6 rows are inserted, Added 0 columns as New Index Columns.","status":200}

```
![PUT](https://user-images.githubusercontent.com/75253788/201490492-56d716f1-5753-4462-9c7c-c62fcf2a697d.png)

## GET Command
```
{
    "token": "-1935843913|3223940520357615501|-1935843909",
    "cmd": "GET",
    "dbName": "Colors",
    "rel": "Color-Rel",
  	"createTime": true,
    "updateTime": true,
    "jsonStr": {
        "category": "value"
    }

}
```
##### output
```
{"data":"{\"code\":{\"rgba\":[0,0,0,1],\"hex\":\"#FFF\"},\"color\":\"white\",\"category\":\"value\"}","message":"DATA RETRIEVED FROM PI","status":200}
```

## Update Command
```
{
    "token": "2134770734|1905622745244281054|2134771272",
    "cmd": "GET",
    "dbName": "Student",
    "rel": "Student-Rel",
    "jsonStr":{
        "stuName": "Akash Prasad"
    }
}
```
##### output
```
{"data":"{\"2\":{\"type\":null},\"NewIndexColumnCreated\":0,\"NewNonIndexColumnCreated\":0}","additionalData":{"processReqType":0,"dbUpdateFlag":true},"message":"Success","status":200}
```

## Remove Command
```
{
    "token": "90938100|-31949268788158014|90953144",
    "cmd": "REMOVE",
    "dbName": "Colors",
    "rel": "Color-Rel",
    "record": 8
}
```
##### output
```
{"data":"{\"removedRecNos\":[8],\"alreadyRemovedRecNos\":[],\"invalidRecNos\":[]}","additionalData":{"processReqType":0,"dbUpdateFlag":true},"message":"Success","status":200}
```
##### Remove Before
![Remove before](https://user-images.githubusercontent.com/75253788/201490758-baef5db0-1eb7-41aa-93ee-614df017f7e5.png)
##### Remove After
![Remove after](https://user-images.githubusercontent.com/75253788/201490762-dd0341ab-9d46-4dea-9090-deab96a0e80c.png)

# Project
## Form
![Form Structure](https://user-images.githubusercontent.com/75253788/201481324-deb60c46-4928-4a58-a6d6-3ae5cee78a34.png)

## Output
![Output](https://user-images.githubusercontent.com/75253788/201481333-1b99e3ba-d601-4360-8651-c9c62ee165fd.png)
