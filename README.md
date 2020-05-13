# HoujinBangou source data (for SQLite)

corporate number for Japanese.



## Usage

```
$ unzip hb.db.zip

$ sqlite3 hb.db "SELECT * FROM sqlite_master"
table|corporations|corporations|2|CREATE TABLE corporations(
    corporateNumber TEXT PRIMARY KEY,
    process TEXT,
    correct TEXT,
    updateDate TEXT,
    changeDate TEXT,
    name TEXT,
    nameImageId TEXT,
    kind TEXT,
    prefectureName TEXT,
    cityName TEXT,
    streetNumber TEXT,
    addressImageId TEXT,
    prefectureCode TEXT,
    cityCode TEXT,
    postCode TEXT,
    addressOutside TEXT,
    addressOutsideImageId TEXT,
    closeDate TEXT,
    closeCause TEXT,
    successorCorporateNumber TEXT,
    changeCause TEXT,
    assignmentDate TEXT )
index|sqlite_autoindex_corporations_1|corporations|3|

$ sqlite3 hb.db "SELECT COUNT(*) FROM corporations"
4316845
```



## Acknowledgment

Source data by http://www.houjin-bangou.nta.go.jp/



## License

This repository is available as open source under the terms of the MIT License.
