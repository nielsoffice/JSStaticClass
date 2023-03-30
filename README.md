# JS StaticClass
JavaScript create a static method in JS class

```HTML
<html>
<head>
<style></style>
</head>
  
  <body id="app-id">
  
  <div id="elemTargeta" class="cons">
    <p>Demo Content...</p>
  </div>
  
  <script id="app-data">
    
    class Developer {
      
      constructor(name,specialty) {
        this.settingFullName  = name;
        this.specialty = specialty;
      }
    
      get info() { return this._settingFullName + ' : ' + this.specialty; }

      static newST() {
        console.log('within the class');
      }

    }
     
    const objDev = new Developer('Niel Fernandez','WPDev');
    Developer.newST();

    Developer.staticMethod = function() { console.log('Hello Static Method'); }
    Developer.staticMethod();
     
   </script>
  
  </body>
  </html>
```

```JS
within the class
Hello Static Method
```
