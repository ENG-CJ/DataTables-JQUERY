# DataTables-JQUERY
DataTables is a table enhancing plug-in for the jQuery Javascript library, adding sorting, paging and filtering abilities to plain HTML tables with minimal.

## Use Bootstrap
Creating Table Using <kbd>HTML</kbd><br>
```html
<html>
 <head>
<!--     Add Boottrap link -->
  </head>
 <body>
<!--     table-->
    <table class="table" id="data">
      <thead>
        <tr>
          <th>ID</th>
          <th>Name</th>
          <th>Course</th>
        </tr>
      </thead>
     
     <tbody>
                <tr>
                    <td>100</td>
                    <td>Mohamed Ali</td>
                    <td>Python</td>

                </tr>
                <tr>
                    <td>101</td>
                    <td>geedi farah</td>
                    <td>C#</td>

                </tr>
            </tbody> 
   
  </body>
</html>

```


## Add DataTable CDN (Css File and JQUERY FILE) 
Copy this Link And Past To the HTML File<br>
```html
 <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.11.3/css/jquery.dataTables.css">
 <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.11.3/js/jquery.dataTables.js"></script>

```

<br>
Click Here To Download The JUQERY CDN<br>
(https://code.jquery.com/)


## Convert The Table Into DataTable
Toggle The Table ID by Using JQUERY use This Syntax To Convert HTML table Into DataTable Make Sure You have JQUERY CDN<br>

```javascript
$(document).ready(()=>{
    
     // toggle table id
     $('#data').DataTable()
     
     // them automatically converts

});

```


## Using Json Or API
To Convert HTML Table Into dataTable using <kbd>JSON</kbd> or <kbd> API</kbd><br>
the data may be json or fetch from api use this syntax<br>

```javascript
 
  $(document).ready(()=>{
      
      $('#data').DataTable({
        
        // this object takes 2 argument one is ajax (where data comes from) and other is column
        
        // "ajax" : "./api/file_name.json" or "./folder/file_name.json"
        
        "ajax" : "./students/data.json",
        "columns" : [
            {"students" : "id"},
            {"students" : "name"},
            {"students" : "course"}
          ]
          
   
      });
  });


```
<br>
To Load The Data from file or api use <kbd>AJAX</kbd>
<kbd>./students/data.json</kbd> stduents is the path_name where data.json is the file_name wh<br>
<kbd>Columns</kbd> is the columns where <kbd>students</kbd> under the column is the identifier column from the json file <br>

This is How to Make <kbd>DataTable()</kbd>
