# event_planning_system


### event date defination
| event date | evwnt name | event location | guest list | budget | notes |
| ---------- | ---------- | -------------- | ---------- | ------ | ----- |
| 2023-10-28 | marriage   | tollychowki    |    600     | 1000000|  dj   | 
| 2024-01-11 | birthday   |  flim_city     |    300     | 500000 | music |
| 2024-04-22 |  party     |   city_club    |    150     | 100000 |  dj   |
| 2024-06-15 |  event     |     club       |    200     | 150000 | dance,music |
| 2024-11-10 | get_together|    hall       |    150     | 100000 |  stage |


## creating table in sql command in database



```sql
CREATE TABLE event_planning (
          event_date        DATE,
          event_ name        varchar(200),
          event_location    varchar(200),
          guest_list        int,
          budget            FLOAT,
          notes             text
          )
```
```sql
INSERT INTO event_planning (
          event_date,        
          event_ name,        
          event_location,   
          guest_list,       
          budget,            
          notes 
) values (
          '2023-10-28',
           'marriage',
           'tollychowki',
           '600',
           '1000000',
           'dj'
           )
 ```
        
        
## if we want to insert multiple rows in the table
        
        
        
  ```sql
  INSERT INTO event_planning (
            )  values  (
            '2024-01-11',
            'birthday',
            'flim_city',
            '300',
            '500000',
            'music'
            ), (
            '2024-04-22',
            'party',
            'city_club',
            '150',
            '100000'
            'dj'
            ) , (
            '2024-06-15',
            ' event',
            'club',
            '200',
            '150000',
            'dance_music'
            )
```

## if we want to read all columns
 
           
```sql
        SELECT * from event_planning
```        
        
        
## if we want to see rows in the column



```sql
      SELECT * FROM event_planning
      WHERE event_date="date"
```

## if we want to update data in the table

```sql
      UPDATE event_planning
      SET
         guest_list=400,
         budget=600000
      where
           event_name='party'
```           
           
## if we want to delete perticular row in the column


```sql
      DELETE FORM event_planning
      WHERE event_name='marriage'
```
